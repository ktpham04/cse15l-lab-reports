# Lab Report 3: Researching Command 'Find'
* The four command-line options that I chosen, were
* `-i`
* `-l`
* `-c`
* `-L`

In finding these command-line options, I used this document: [grep Man Page](https://ss64.com/osx/grep.html)
## Command-line Option `-i`

In using the command `find -i`, this command ignores case disntiction. In the image below, you can see that in the quotation marks the word "CELL FACTOR" and "CALIFORNIA" is in all captials. However, using the command-line option it tells `find` to ignore the upper cases and only access the string value itself. When running `find -i`, the terminal prints out lines with the given input, ignoring the capitalization of the word. This is beneficial when looking for certain words in a text file without needing to worry about the capitalization of a word.

[image](-i.png)

## Command-line Option `-l`

In using the command `find -l`, this command prints out the name of the files in which contains the certain word. For instance, in the image below the `find -l` command is being use to find two words "the" and "dead" in certain files like biomed and 911report. When running `find -l`, the terminal prints out lines of files in which contains the word "dead" and "the" depending on which file it looks in. In finding the word "dead" it looks through the file biomed and its text files, then prints out all the text files from biomed that contains "dead". This is useful, when needing to find a input in multiple files.

[image](-c.png)

## Command-line Option `-c`

In using the command `find -c`, this command prints out the line number of where the input is. For instance, the image below contains two commands of `find -c` in the search of "the" in the biomed file and "dead" in the 911report file. In finding the word "the" in the biomed file, it gives us the line number in which "the" appears. This also happens in finding "dead" as it prints out the line number in which "dead" appears. This is beneficial when trying to locate a certain input, instead of receiving a bunch of lines in the terminal.

[image](-l.png)

## Command-line Option `-L`

In using the command `find -L`, quite similar to `find -l` which prints out the name of the files that contains the certain word. In the image below, the command `find -L` is used to search for the given inputs "the a" and "dead" wihtin the linked files such as biomed or 911report. In running this command in the terminal, it prints out the files in which contains these inputs. The benefits of using `find -L` is simialr to `find -l` when needing to find a input in multiple files.

[image](-Ls.png)
