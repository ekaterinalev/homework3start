# LING 78100 Homework 3

Please consult the syllabus for detailed instructions regarding how to submit programming assignments and a list of grading criteria. Deadline: Monday, November 6th, 2017

Note: Please submit assignments via the Github Classroom

You may either create individual .py files for each problem or solve each problem in its own cell in an ipython notebook.  If you create individual files, you should also create an ipython notebook that imports each file and demonstrates that the imported functions work on the test cases described below.  If you use one large ipython notebook for everything, you should demonstrate that your functions work on the test cases described below in the same notebook.

## Problem 1: Chapter 6, Programming Exercise 2 (page 206) "Ants go marching"

In order to solve this homework problem, you should write a function that prints a single verse of
the song – when provided with the appropriate inputs. Look closely at the verses of the song, and
determine what changes in each verse and what stays the same. The input to the function should
just be the minimal information needed to print the text for that single verse of the song.
To print the entire song, your program will call this function ten times – once for each verse.
You should demonstrate that your program works by running it to produce the text of the entire
ten-verse song.  If you don’t know the song by heart, you can find the lyrics here:
http://kids.niehs.nih.gov/lyrics/antsgo.htm

## Problem 2: Chapter 6, Programming Exercise 11 (page 207) "squareEach function"
You should demonstrate that your program works by testing it on the following inputs:
```python
[23, -43, 2, 10, 20, 34]
[3]
[54, 54]
```

IMPORTANT: Your function should modify the actual list `nums` that it is passed as input. In
other words, you must modify the parameter that is passed to the function. It should not produce
a new list to be returned. The original list that was passed to the function should be changed
inside of your function.  Remember mutability!

## Problem 3: Chapter 8, Programming Exercise 3 (page 279) "Investment Doubling"
You should demonstrate that your program works by testing it on these two interest rates:
 * 3% (Note: this might be equal to 0.03, depending on how to ask your user for input.)
 * 5%

## Problem 4: Working with Tab-Delimited Files, exported from Excel Files

In this problem, you will work with a file that contains a transcript of a few English sentences.
Open the file `hw3data.xlsx` in this repository using Microsoft Excel. You’ll see that for each word, the file lists
information about the lemma, the part-of-speech, the word’s start-time (in an audio recording that this is a transcript of), and end-time. We’re going to work with this file in this assignment.

Using Microsoft Excel, on the File menu, select “Save As…” to save the file as a Tab Delimited
Text (.txt) file. In this way, you can produce a file called `hw3data.txt`. Now, write a Python program that opens the `hw3data.txt` file, reads the contents of the file, splits the file into lines, splits the lines into items (based on tabs), and examines each of the items on that line to determine if there is a “PREP” in the third column of that row.  Every time there is a “PREP” in the third column, your program should print the word that is in the first column of that row.  In addition, at the end of your program, you should print a count of the total number of “PREP” rows in the file.

Note: If you are using a Mac, you may find that when Excel exports the file, the lines end with `\r` instead of `\n`. So, when you try to read a line of the file, you may get one big line that contains all the contents of the file. You’ll need to split the string at `\r` and then split the resulting strings at `\t` to do your work.
