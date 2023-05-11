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
[cs15(sp23bc@ieng6-201] :stringsearch-data:362$ grep-i "CELL FACTOR" •/technical/biomed/*.txt
•/technical/biomed/1471-2091-3-23.txt:
further explored. An insect cell factor, polyhedrin
•/technical/biomed/1471-213X-3-2.txt:
Enhancer Factor/T Cell Factor (LEF/TCF) family of high
./technical/biomed/1471-2164-4-13.txt:
lymphocyte enhancement factor-1 (LEF-1) and T cell factor-1
•/technical/biomed/1472-6874-2-8-txt:
stem cell factor) are encoded at the white spotting (W) and
^[[A[cs15(sp23bc@ieng6-201l :stringsearch-data:363$ grep -i "CALIFORNIA"
./technical/911report/*.txt
•/technical/911report/chapter-11.txt:
•/technical/911report/chapter-13.4.txt:
California went on the watch for his like.
chemistry, from California State University, Sacramento. Sufaat did not start on the
•/technical/911report/chapter-13.4.txt:
reasons for sending Hazmi and Mihdhar to California do not seem especially
•/technical/911report/chapter-13.4-txt:
explanation for the California destination.
The possibility that the two hijackers
/technical/911report/chapter-13.4.txt:
./technical/911report/chapter-13.4.txt:
addresses-one in the United States ("possibly in California") and one in South
./technical/911report/chapter-13.4.txt:
California.'
" Intelligence report, interrogation of KSM, June 15,
•/technical/911report/chapter-13.4.txt:
•/technical/911report/chapter-13.4.txt:
•/technical/911report/chapter-13.5.txt:
•/technical/911report/chapter-3.txt:
California, but Atta told him to discontinue this effort. Intelligence report,
his training in California, see FBI report of investigation, interview of Adnan
85.
• Hazmi and Mihdhar used their true names to obtain California driver's licenses
California (UNOCAL) to build a pipeline across the country.
While there was probably
•/technical/911report/chapter-5.txt:
+/technical/911report/chapter-5.txt:
./technical/911report/chapter-5. txt:
•/technical/911report/chapter-6.txt:
/technical/911report/chapter-6. txt:
•/technical/911report/chapter-6.txt:
•/technical/911report/chapter-7.txt:
./technical/911report/chapter-7.txt:
./technical/911report/chapter-7. txt:
./technical/911report/chapter-7.txt:
•/technical/911report/chapter-7.txt:
•/technical/911report/chapter-7.txt:
•/technical/911report/chapter-7.txt:
•/technical/911report/chapter-7.txt:
./technical/911report/chapter-7.txt:
./technical/911report/chapter-7.txt:
•/technical/911report/chapter-7.txt:
•/technical/911report/chapter-7.txt:
./technical/911report/chapter-7.txt:
•/technical/911report/chapter-7.txt:
•/technical/911report/chapter-8.txt:
•/technical/911report/chapter-8.txt:
California; brochures for schools; and airline
one gpenting:" nil en, tahosa' ah ine Phabite" ease, ne red retural it hortnean-rEti offic,
that Hijazi had lived in California and driven a cab in Boston and that Deek was a
FIRST ARRIVALS IN CALIFORNIA
Why Hazmi and Mihdhar came to California, we do not know for certain. Khalid Sheikh
Mohammed (KSM), the organizer of the planes operation, explains that California was
that al Qaeda had any agents in Southern California. We do not credit this
California, so that they could begin pilot training as soon as possible. KSM claims
Culver City, one of the most prominent mosques in Southern California.
fellow inmates at a California prison in September- October 2003 that he had known
rest of his time in California, until mid-December; he would then leave for Arizona
Translating between English and Arabic, he assisted them in obtaining California
of California declined to prosecute him on charges arising out of his alleged
impression is that soon after arriving in California, Hazmi and Mihdhar sought out
child arrived, he could stand life in California no longer. In late May and early
California, and Arizona; and he briefly started at a couple of them before returning
an English as a second language program in Oakland, California, which he had
In
California in the mid-1990s. A clandestine source said in 1998 that a Bin Ladin
June 2000, Mihdhar left California and returned to Yemen. It is possible that if,
```

## Command-line Option `-l`

In using the command `find -l`, this command prints out the name of the files in which contains the certain word. For instance, in the image below the `find -l` command is being use to find two words "the" and "dead" in certain files like biomed and 911report. When running `find -l`, the terminal prints out lines of files in which contains the word "dead" and "the" depending on which file it looks in. In finding the word "dead" it looks through the file biomed and its text files, then prints out all the text files from biomed that contains "dead". This is useful, when needing to find a input in multiple files.

```
[cs15(sp23bc@ieng6-201] :stringsearch-data:385$ grep -L "dead" ./technical/911report/*. txt
•/technical/911report/chapter-1.txt
•/technical/911report/chapter-12.txt
•/technical/911report/chapter-13.3.txt
•/technical/911report/chapter-13.4.txt
=/technical/911report/chapter-13.5.txt
/technical/911report/chapter-2.txt
/technical/911report/chapter-3.txt
•/technical/911report/chapter-6.txt
[cs15(sp23bc@ieng6-201] :stringsearch-data: 386$ grep-l
"thell
/technical/olomed/*.
• txt
•/technical/biomed/1468-6708-3-
1. txt
./technical/biomed/1468-6708-3-10.txt
•/technical/biomed/1468-6708-3-3.txt
•/technical/biomed/1468-6708-3-4.txt
./technical/biomed/1468-6708-3-7
txt
•/technical/biomed/1471-2091-2-
-10-txt
•/technical/biomed/1471-2091-
./technical/biomed/1471-2091-2-12.txt
./technical/biomed/1471-2091-2-13.txt
•/technical/biomed/1471-2091-2
•/technical/biomed/1471-2091-
•/technical/biomed/1471-2091
•/technical/biomed/1471-2091-
=/technical/biomed/1471-2091-
•/technical/biomed/1471-2091-3
-/technical/biomed/1471-2091-3-15-txt
/technical/biomed/1471-2091-3-16.txt
/technical/biomed/1471-2091-3-17
txt
•/technical/biomed/1471-2091-3-18.txt
/technical/biomed/1471-2091-3-22-txt
•/technical/biomed/1471-2091-3-23.txt
-chnicali1471-291-3-30-
-/technical/biomed/1471-7001-3-31_+
-technical/biomed/1471-2001=3
•4. txt
•/technical/biomed/1471-2091-3-8.txt
./technical/biomed/1471-2091-4-1.txt
•/technical/biomed/1471-2091-4-5.txt
./technical/biomed/1471-2105-1-1.txt
•/technical/biomed/1471-2105-
•/technical/biomed/1471-2105-
•/technical/biomed/1471-2105-
•/technical/biomed/1471-2105-
•/technical/biomed/1471-2105-
•/technical/biomed/1471-2105-3-16.txt
/technical/biomed/1471-2105.
-5-1/ILXT
=/technical/biomed/1471-2105-3-18.txt
/technical/biomed/1471-2105-3-
•/technical/biomed/1471-2105-3-22.txt
/technical/biomed/1471-2105-3-23.txt
•/technical/biomed/1471-2105-3-24.txt
technicalbiomed/1471-2105-3-26-tx1
-technical biomed/1471-2105-3-28-tx1
/technical/biomed/1471
/tecnnical/blomed/1471-2105
-/technical/biomed/1471
•/technical/biomed/1471-2105
•/technical/biomed/1471-210
-/technical/olomed/14/1-216
_/technical/biomed/1471-2105-3-6
- Ext
-cnal14/1-/145
•/technical/biomed/1471-2105-
•/technical/biomed/1471-2105
•/technical/biomed/1471-2105
-26.txt
=/technical/biomed/1471-2105
•/technical/biomed/1471-2105-
-28. txt
/technical/biomed/1471-2121-1-2.txt
/technical/biomed/1471-2
/technical/biomed/1471-2121-2-10.txt
/technical/olomed/14/1-
-technical biomed/1471-
-technical biomed.
-technical/biomed/1471
./technical/biomed/1471-2121
tx
./technical/biomed/1471-2121-2-22.
```

## Command-line Option `-c`

In using the command `find -c`, this command prints out the line number of where the input is. For instance, the image below contains two commands of `find -c` in the search of "the" in the biomed file and "dead" in the 911report file. In finding the word "the" in the biomed file, it gives us the line number in which "the" appears. This also happens in finding "dead" as it prints out the line number in which "dead" appears. This is beneficial when trying to locate a certain input, instead of receiving a bunch of lines in the terminal.

```
[cs15(sp23bc@ieng6-201] :stringsearch-data:382$ grep -c "the"
./technical/biomed/1472-67*.txt
./technical/biomed/1472-6750-1-11.txt:257
•/technical/biomed/1472-6750-1-12.txt:162
•/technical/biomed/1472-6750-1-13.txt:176
•/technical/biomed/1472-6750-1-6.txt:240
•/technical/biomed/1472-6750-1-8.txt:165
•/technical/biomed/1472-6750-2-10.txt:118
•/technical/biomed/1472-6750-2-13.txt:144
/technical/biomed/1472-6750-2-14.txt:354
./technical/biomed/1472-6750-2-2.txt:99
./technical/biomed/1472-6750-2-21.txt:211
•/technical/biomed/1472-6750-3-11.txt:95
./technical/biomed/1472-6750-3-4.txt:209
•/technical/biomed/1472-6750-3-6-txt:316
./technical/biomed/1472-6769-1-1.txt:308
•/technical/biomed/1472-6769-1-2.txt:120
./technical/biomed/1472-6769-1-3.txt:68
•/technical/biomed/1472-6769-1-4-txt:63
•/technical/biomed/1472-6785-1-3.txt:102
•/technical/biomed/1472-6785-1-5.txt:129
./technical/biomed/1472-6785-2-6.txt:184
•/technical/biomed/1472-6785-2-7-txt:265
•/technical/biomed/1472-6793-1-11.txt:187
•/technical/biomed/1472-6793-1-12.txt:142
•/technical/biomed/1472-6793-1-15.txt:235
•/technical/biomed/1472-6793-1-2-txt:217
./technical/biomed/1472-6793-1-6.txt:93
•/technical/biomed/1472-6793-1-8.txt:330
./technical/biomed/1472-6793-2-1-txt:201
•/technical/biomed/1472-6793-2-11.txt:217
•/technical/biomed/1472-6793-2-16.txt:234
•/technical/biomed/1472-6793-2-17.txt:180
•/technical/biomed/1472-6793-2-18-txt:309
•/technical/biomed/1472-6793-2-19.txt:216
•/technical/biomed/1472-6793-2-2.txt:212
/technical/biomed/1472-6793-2-4.txt:150
./technical/biomed/1472-6793-2-5.txt:231
•/technical/biomed/1472-6793-2-8.txt:197
•/technical/biomed/1472-6793-3-3.txt:91
./technical/biomed/1472-6793-3-4.txt:167
•/technical/biomed/1472-6793-3-5-txt:170
/technical/biomed/1472-6793-3-6.txt:149
[cs15(sp23bc@ieng6-201] :stringsearch-data:383$ grep -c "dead"
./technical/911report/*.txt
•/technical/911report/chapter-1.txt:1
•/technical/911report/chapter-10.txt:0
•/technical/911report/chapter-11.txt:0
./technical/911report/chapter-12.txt:1
./technical/911report/chapter-13.1.txt:0
•/technical/911report/chapter-13.2.txt:0
•/technical/911report/chapter-13.3.txt:1
•/technical/911report/chapter-13.4.txt:2
•/technical/911report/chapter-13.5.txt:2
•/technical/911report/chapter-2.txt:1
•/technical/911report/chapter-3.txt:7
•/technical/911report/chapter-5.txt:0
./technical/911report/chapter-6.txt:3
•/technical/911report/chapter-7. txt:0
•/technical/911report/chapter-8.txt:0
•/technical/911report/chapter-9.txt:0
./technical/911report/preface.txt:0
```

## Command-line Option `-L`

In using the command `find -L`, quite similar to `find -l` which prints out the name of the files that contains the certain word. In the image below, the command `find -L` is used to search for the given inputs "the a" and "dead" wihtin the linked files such as biomed or 911report. In running this command in the terminal, it prints out the files in which contains these inputs. The benefits of using `find -L` is simialr to `find -l` when needing to find a input in multiple files.

```
[cs151sp23bc@ieng6-201] :stringsearch-data: 391$ grep-L
•/technical/biomed/1471-2199-3-10.txt
•/technical/biomed/1471-2334-3-13.txt
•/technical/biomed/1471-2474-2-2.txt
•/technical/biomed/1472-6769-1-3.txt
•/technical/biomed/1472-6769-1-4.txt
=/technical/biomed/bcr571.txt
[cs15(sp23bc@ieng6-201] :stringsearch-data: 392$ grep-L
•/technical/911report/chapter-10.txt
•/technical/911report/chapter-11.txt
=/technical/911report/chapter-13.1.txt
•/technical/911report/chapter-13.2.txt
•/technical/911report/chapter-5.txt
•/technical/911report/chapter-7.txt
•/technical/911report/chapter-8.txt
•/technical/911report/chapter-9.txt
•/technical/911report/preface.txt
```
