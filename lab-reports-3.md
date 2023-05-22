# Lab Report 3: Researching Command 'Find'
* The four command-line options that I chosen, were
* `-i`
* `-l`
* `-c`
* `-L`

In finding these command-line options, I used this document: [grep Man Page](https://ss64.com/osx/grep.html)
## Command-line Option `-i`

In using the command `find -i`, this command ignores case disntiction. In the image below, you can see that in the quotation marks the word "CELL FACTOR" and "CALIFORNIA" is in all captials. However, using the command-line option it tells `find` to ignore the upper cases and only access the string value itself. When running `find -i`, the terminal prints out lines with the given input, ignoring the capitalization of the word. This is beneficial when looking for certain words in a text file without needing to worry about the capitalization of a word.

```
[[cs15lsp23bc@ieng6-203]:stringsearch-data:521$ grep -i "CELL FACTOR" ./technical/biomed/*.txt
./technical/biomed/1471-2091-3-23.txt:        further explored. An insect cell factor, polyhedrin
./technical/biomed/1471-213X-3-2.txt:        Enhancer Factor/T Cell Factor (LEF/TCF) family of high
./technical/biomed/1471-2164-4-13.txt:        lymphocyte enhancement factor-1 (LEF-1) and T cell factor-1
./technical/biomed/1472-6874-2-8.txt:        stem cell factor) are encoded at the white spotting (W) and[cs15(sp23bc@ieng6-201l 
```
```
[cs15lsp23bc@ieng6-203]:stringsearch-data:524$ grep -i "DRIVER'S" ./technical/911report/*.txt
./technical/911report/chapter-13.4.txt:                taxi license, or even a driver's license, until months after he could be supposed to
./technical/911report/chapter-13.4.txt:                and Jarrah obtaining driver's licenses, see FBI report, "Hijackers Timeline,"Dec. 5,
./technical/911report/chapter-13.5.txt:            85. Hazmi and Mihdhar used their true names to obtain California driver's licenses
./technical/911report/chapter-13.5.txt:                could have unearthed the driver's licenses, the car registration, and the telephone
./technical/911report/chapter-7.txt:                driver's licenses and with applying to language and flight schools. Abdullah also
./technical/911report/chapter-7.txt:                to Jordan, having been convicted after 9/11 in a fraudulent driver's license
./technical/911report/chapter-7.txt:                just wanted to pick up Atta's international driver's license and some money. This
./technical/911report/chapter-7.txt:                Lakes, Florida, to get Florida driver's licenses. Back in Virginia, Hazmi and
./technical/911report/chapter-8.txt:                few days later. He checked local New York databases for criminal record and driver's
[cs15lsp23bc@ieng6-203]:stringsearch-data:525$ 
```

## Command-line Option `-l`

In using the command `find -l`, this command prints out the name of the files in which contains the certain word. For instance, in the image below the `find -l` command is being use to find two words "the hell" and "dead" in certain files like biomed and 911report. When running `find -l`, the terminal prints out lines of files in which contains the word "dead" and "the hell" depending on which file it looks in. In finding the word "dead" it looks through the file biomed and its text files, then prints out all the text files from biomed that contains "dead". This is useful, when needing to find a input in multiple files.

```
[[cs15lsp23bc@ieng6-203]:stringsearch-data:514$ grep -l "dead" ./technical/911report/*.txt
./technical/911report/chapter-1.txt
./technical/911report/chapter-12.txt
./technical/911report/chapter-13.3.txt
./technical/911report/chapter-13.4.txt
./technical/911report/chapter-13.5.txt
./technical/911report/chapter-2.txt
./technical/911report/chapter-3.txt
./technical/911report/chapter-6.txt
```
```
[cs15lsp23bc@ieng6-203]:stringsearch-data:515$ grep -l "the hell" ./technical/biomed/*.txt
./technical/biomed/1471-2458-2-25.txt
[cs15lsp23bc@ieng6-203]:stringsearch-data:516$ 
```

## Command-line Option `-c`

In using the command `find -c`, this command prints out the line number of where the input is. For instance, the image below contains two commands of `find -c` in the search of "dead" in the biomed file and 911report file. In finding the word "the" in the biomed file, it gives us the line number in which "the" appears. This also happens in finding "dead" as it prints out the line number in which "dead" appears. This is beneficial when trying to locate a certain input, instead of receiving a bunch of lines in the terminal.

```
[cs15lsp23bc@ieng6-203]:stringsearch-data:537$ grep -c "dead" ./technical/biomed/1472-67*.txt
./technical/biomed/1472-6750-1-11.txt:0
./technical/biomed/1472-6750-1-12.txt:0
./technical/biomed/1472-6750-1-13.txt:0
./technical/biomed/1472-6750-1-6.txt:0
./technical/biomed/1472-6750-1-8.txt:0
./technical/biomed/1472-6750-2-10.txt:0
./technical/biomed/1472-6750-2-13.txt:0
./technical/biomed/1472-6750-2-14.txt:0
./technical/biomed/1472-6750-2-2.txt:0
./technical/biomed/1472-6750-2-21.txt:0
./technical/biomed/1472-6750-3-11.txt:0
./technical/biomed/1472-6750-3-4.txt:0
./technical/biomed/1472-6750-3-6.txt:0
./technical/biomed/1472-6769-1-1.txt:0
./technical/biomed/1472-6769-1-2.txt:0
./technical/biomed/1472-6769-1-3.txt:0
./technical/biomed/1472-6769-1-4.txt:0
./technical/biomed/1472-6785-1-3.txt:0
./technical/biomed/1472-6785-1-5.txt:0
./technical/biomed/1472-6785-2-6.txt:2
./technical/biomed/1472-6785-2-7.txt:0
./technical/biomed/1472-6793-1-11.txt:0
./technical/biomed/1472-6793-1-12.txt:0
./technical/biomed/1472-6793-1-15.txt:0
./technical/biomed/1472-6793-1-2.txt:0
./technical/biomed/1472-6793-1-6.txt:0
./technical/biomed/1472-6793-1-8.txt:0
./technical/biomed/1472-6793-2-1.txt:0
./technical/biomed/1472-6793-2-11.txt:0
./technical/biomed/1472-6793-2-16.txt:0
./technical/biomed/1472-6793-2-17.txt:0
./technical/biomed/1472-6793-2-18.txt:0
./technical/biomed/1472-6793-2-19.txt:0
./technical/biomed/1472-6793-2-2.txt:1
./technical/biomed/1472-6793-2-4.txt:0
./technical/biomed/1472-6793-2-5.txt:0
./technical/biomed/1472-6793-2-8.txt:0
./technical/biomed/1472-6793-3-3.txt:0
./technical/biomed/1472-6793-3-4.txt:0
./technical/biomed/1472-6793-3-5.txt:0
./technical/biomed/1472-6793-3-6.txt:0
```
```
[[cs15lsp23bc@ieng6-203]:stringsearch-data:538$ grep -c "dead" ./technical/911report/*.txt
./technical/911report/chapter-1.txt:1
./technical/911report/chapter-10.txt:0
./technical/911report/chapter-11.txt:0
./technical/911report/chapter-12.txt:1
./technical/911report/chapter-13.1.txt:0
./technical/911report/chapter-13.2.txt:0
./technical/911report/chapter-13.3.txt:1
./technical/911report/chapter-13.4.txt:2
./technical/911report/chapter-13.5.txt:2
./technical/911report/chapter-2.txt:1
./technical/911report/chapter-3.txt:7
./technical/911report/chapter-5.txt:0
./technical/911report/chapter-6.txt:3
./technical/911report/chapter-7.txt:0
./technical/911report/chapter-8.txt:0
./technical/911report/chapter-9.txt:0
./technical/911report/preface.txt:0
```

## Command-line Option `-L`

In using the command `find -L`, quite similar to `find -l` which prints out the name of the files that contains the certain word. In the image below, the command `find -L` is used to search for the given inputs "the a" and "dead" wihtin the linked files such as biomed or 911report. In running this command in the terminal, it prints out the files in which contains these inputs. The benefits of using `find -L` is simialr to `find -l` when needing to find a input in multiple files.

```
[cs15lsp23bc@ieng6-203]:stringsearch-data:539$ grep -L "the a" ./technical/biomed/*.txt
./technical/biomed/1471-2199-3-10.txt
./technical/biomed/1471-2334-3-13.txt
./technical/biomed/1471-2474-2-2.txt
./technical/biomed/1472-6769-1-3.txt
./technical/biomed/1472-6769-1-4.txt
./technical/biomed/bcr571.txt
```
```
[cs15lsp23bc@ieng6-203]:stringsearch-data:540$ grep -L "dead" ./technical/911report/*.txt
./technical/911report/chapter-10.txt
./technical/911report/chapter-11.txt
./technical/911report/chapter-13.1.txt
./technical/911report/chapter-13.2.txt
./technical/911report/chapter-5.txt
./technical/911report/chapter-7.txt
./technical/911report/chapter-8.txt
./technical/911report/chapter-9.txt
./technical/911report/preface.txt
```
