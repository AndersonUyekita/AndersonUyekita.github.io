# UD595 - Linux Command Line Basics - `Lesson02`

#### Tags

* Author:      : AH Uyekita
* Chapter      : Get Into the Shell
* Start        : 20/12/2018
* End (Planned): 20/12/2018
* Title        : Shell Commands
* COD          : UD595
    * **Instructor:** Philip Mallory
    * **Instructor:** Karl Krueger

********************************************************************************

## Command History

To access the command history in a simple way is just press the <kbd>up arrow key</kbd>.

This site has a good summary of command line: [CodeAcademy][code_website]

[code_website]: https://www.codecademy.com/articles/command-line-commands

## Interrupt

A way to interrupt any command is pressing <kbd>Ctrl</kbd> + <kbd>D</kbd>.

If you want to send the "there is no more entries", just press <kbd>Ctrl</kbd> + <kbd>D</kbd>.

#### `ls`

List all the file inside in the current directory.

```
$ ls
file_1.txt
file_2.pdf
...
```
Bear in mind, all files does not start with `.`. To display the dot files, it is necessary a argument to show them.

* -a: will show all entries starting with `.`;
* --all: show all entries.

```
$ ls -a
```
If you want more details in the `ls` command you can use the `ls -l`, which will display the time modification, size, and others info.

```
$ ls -l
```

#### `unzip`

Unzip the file in the current folder.

```
$ unzip things.zip
inflating: bivalves.txt
inflating: cephalopods.txt
inflating: gastropods.txt
inflating: mustelidae.txt
extracting: .secret
 creating: ocean/
 creating: ocean/stuff/
 creating: ocean/stuff/misc/
extracting: ocean/stuff/otters
extracting: ocean/water
 creating: junk/
 creating: junk/parts/
 creating: junk/parts/a/
extracting: junk/parts/a/apple-cores
 creating: junk/parts/b/
extracting: junk/parts/b/banana-peels
 creating: junk/parts/c/
extracting: junk/parts/c/clam-shells
 creating: globbing/
extracting: globbing/app.css
extracting: globbing/app.html
extracting: globbing/app.js
extracting: globbing/bean.png
extracting: globbing/bear.png
extracting: globbing/beer.png
extracting: globbing/bees.png
extracting: globbing/DAVE.JPG
extracting: globbing/favicon.png
extracting: globbing/index.html
extracting: globbing/JADE.jpg
extracting: globbing/john.jpg
extracting: globbing/rose.JPG
inflating: gastropods_draft.txt
inflating: TheWindintheWillows.txt
```

#### `cat`

Concatenate text files into a single one. It is possible to use with a single file also.

```
$ cat my_text.txt
content of my my_text.txt
```

#### `wc`

It is the word count program.

```
$ wc bivalves.txt
12 393 2483 bivalves.txt
```
* 12 lines
* 393 words
* 2483 bytes

#### `diff`

This command shows the differences between two version of the same file.

```
$ diff gastropods.txt gastropods_draft.txt
5d4
< Sea Angel: Sea angels (clade Gymnosomata) are a large group of small, swimming sea slugs classified into six different families. In this clade, the foot of the gastropodhas developed into wing-like flapping appendages (parapodia) and their shells have been lost. Both adaptations suit their free-swimming oceanic lives.
```
The `<` means a new content in `gastropods.txt`.

#### `curl`

This command is used to download the file using a path.

```
$ curl -o things.zip http://udacity.github.io/ud595-shell/stuff.zip
% Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                               Dload  Upload   Total   Spent    Left  Speed
100  144k  100  144k    0     0   307k      0 --:--:-- --:--:-- --:--:--  307k
```

Do not miss the `-o`.

#### `man`

Shows the manual of a command.

```
$ man cowsay
```

#### `rm`

Remove a file.

```
$ rm my_file.txt
```
#### `bc`

Runs a calculator program.

#### `less`

This program is useful to read (not change/edit) a very large file in Unix environment.

#### `nano`

This is a text editor.

#### `vim`

This an other text editor.
