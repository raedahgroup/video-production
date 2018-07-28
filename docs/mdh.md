# mdh (markdown helper)

`mdh` is a command line program written in python designed to make creating and editing [storyboards](https://en.wikipedia.org/wiki/Storyboard) in markdown simple.



## Getting Started

`mdh` is written in standard Python3 and has only been tested in Ubuntu.

If you do not have Python3, install it on Ubuntu like so:

```bash
$ sudo apt-get install python3
```



## How It Works

`mdh` is designed for the pre-production workflow and naming conventions __specific to this repository__.

This workflow is as follows.

1. A voice over script is written in paragraph format and saved as `/videoName/videoName_script.md`
2. A storyboard template is generated using `_script.md` as input making each paragraph of voice over an individual shot. The storyboard file saved as `/videoName/videoName_storyboard.md`.
3. `.svg` files are created and named for their corresponding shot to represent the visual sketches of the storyboard. Saved as  `videoName/img/shot_1.svg`



### Proper _script.md File Layout

for `mdh` to work correctly, the `_script.md` files must be formatted in a specific way. `mdh`  breaks them up into two parts, the `header` and the `body`

The `header` consists of two markdown headers and a blank line:

```markdown
## Decred: Proof-of-Stake
### Voice Over Script

```

The `body` of the script begins on the 4th line of the file with paragraphs separated by an empty line:

```markdown
## Decred: Proof-of-Stake
### Voice Over Script

Decred proof-of-stake is an on-chain decision making system where participants purchase tickets for a chance to have their voice heard.

To purchase a ticket, participants must have enough Decred to cover the current ticket price.
```



### _storyboard.md File Layout

a storyboard file is made up of a `header` and a table of rows with rows representing `shots`.

The storyboard header generated from the `_script.md` above would look like so:

```markdown
## Decred: Proof-of-Stake

### Storyboard
**Estimated Runtime:**

No. | VISUAL | AUDIO | TIME
:-: | :----: | :---: | :--:
```

As you can see this header includes the header for the file as well as the header for the storyboard table. The `No.` column in the table represents the `shot` number, the `visual` column is where the `.svg` sketch will go, `audio` is for the corresponding lines from the `_script.md` , and `time` is the length in seconds of the shot. The seconds in the `Time` column add up to the `Estimated Runtime`. 



When a `_storyboard`  file is generated from a `_script.md` file, one row for each paragraph is added to the storyboard table complete with shot number and a link to the corresponding `.svg` sketch.

```markdown
## Decred: Proof-of-Stake

### Storyboard
**Estimated Runtime:**

No. | VISUAL | AUDIO | TIME
:-: | :----: | :---: | :--:
1 | ![Shot 1](../decredPoS/img/shot_1.svg) | Decred proof-of-stake is and on-chain decision making system where participants purchase tickets for a chance to have their voice heard |  
2 | ![Shot 2](../decredPoS/img/shot_2.svg) | To purchase a ticket, participants must have enough Decred to cover the current ticket price. |  
```



#### Editing _storyboard.md files

What if you want to break up the script lines in `shot 1` into two separate shots? Well, to do this you would have to do a few things:

1. Add a new row to the table
2. Increment the `no.` and `visual` columns of all rows after `shot 1` to reflect their new shot numbers.
3. Increment all `.svg` filenames in `/videoName/img/` to reflect their new shot numbers.
4. Copy and paste the section of script lines you want to separate from `shot 1` into the new `shot 2` row.

`mdh` does all of this for you.



## mdh Usage

To use `mdh`, pass command line arguments from the __root directory__ of the repository:

```bash
$ ./mdh Command {args ...}
```

To save time typing, `mdh`  allows the setting of a `working directory`. To set `mdh` to work in the `decredPoS` video directory, pass the `dir` command followed by the _name_ of the directory (__not the path!__).

```bash
$ ./mdh dir decredPoS
```

 To see which directory `mdh` is currently set to work in, use the `dir?` command:

```bash
$ ./mdh dir?
working directory: ./decredPoS
```

With the working directory set, you can generate `decredPoS_storyboard.md` from the already written `decredPoS_script.md` by running the `build` command:

```bash
$ ./mdh build
```

To split `shot 1` into two shots, run the `split` command passing the shot number you want to split with a unique sequence of voice over text after which you would like the split to occur:

```bash
$ ./mdh split 1 system
```

This command would make this:

```markdown
## Decred: Proof-of-Stake

### Storyboard
**Estimated Runtime:**

No. | VISUAL | AUDIO | TIME
:-: | :----: | :---: | :--:
1 | ![Shot 1](../decredPoS/img/shot_1.svg) | Decred proof-of-stake is and on-chain decision making system where participants purchase tickets for a chance to have their voice heard |  
2 | ![Shot 2](../decredPoS/img/shot_2.svg) | To purchase a ticket, participants must have enough Decred to cover the current ticket price. |  
```

Into this:

```markdown
## Decred: Proof-of-Stake

### Storyboard
**Estimated Runtime:**

No. | VISUAL | AUDIO | TIME
:-: | :----: | :---: | :--:
1 | ![Shot 1](../decredPoS/img/shot_1.svg) | Decred proof-of-stake is and on-chain decision making system |  
2 | ![Shot 2](../decredPoS/img/shot_2.svg) | where participants purchase tickets for a chance to have their voice heard. |
3 | ![Shot 3](../decredPoS/img/shot_3.svg) | To purchase a ticket, participants must have enough Decred to cover the current ticket price. |
```

If you have already created the `.svg` sketch files then they will have to be refactored. To instruct `mdh` to refactor the corresponding `.svg` files during the split, use the `--img` flag.

```bash
$ ./mdh split 1 system --img
```

Lastly, to remove a row completely use the `remove` command:

```bash
$ ./mdh remove 1 --img
```



## Questions?

If you have any questions or Ideas concerning `mdh`, please contact @justinsantoro