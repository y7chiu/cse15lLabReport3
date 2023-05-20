# Lab Report 3

## Researching Commands
Consider the commands less, find, and grep. Choose one of them. Online, find 4 interesting command-line options or alternate ways to use the command you chose. For example, we saw the -name option for find in class. For each of those options, give 2 examples of using it on files and directories from ./technical. Show each example as a code block that shows the command and its output, and write a sentence or two about what it’s doing and why it’s useful.

In this case I choose ```grep``` command line for searching to finish the labreport. I ask ChatGPT to privide interesting "grep" command lines. Let's see what interesting command lines I got!

------------------------------------------------------------------------------------

> **grep -r "Specific string":** **Find all files containing a specific string**

grep -r means **Do recursive search**, which will find out the specific string in all files. If we are doing some academic researches, we can quickly use this command line to find the specific topics in the all potential references. This is difference as the grep command. The grep command is only search for the string in the specified file, but grep -r command is searching the string in all potential files.

For example, when I type grep -r "adults". The terminal will find all the files that have the string "adults". Below is the picture of it.

<img width="1013" alt="截圖 2023-05-07 15 39 56" src="https://user-images.githubusercontent.com/130111605/236705968-6c1e25d5-8841-49cd-8c7e-1e314129eec1.png">

Another example, when I trype grep -r "rescue". The terminal will find all the files that have the string "rescue". Below is the picture of it.

<img width="962" alt="截圖 2023-05-07 15 41 12" src="https://user-images.githubusercontent.com/130111605/236706027-735668e8-54e0-4467-881b-848855141890.png">

------------------------------------------------------------------------------------

> **grep -i "Specific string" fileName.txt:** **Find the specific string and display whole the sentence that includes this string.** 

It enables to search for a string freely in the file, such as upper/lower case, or the other strings that include the string we want to search. For this command, we can use it to find more potential cases of string. Sometimes if there are less sources to find, not restricting the upper/lower case may be help people to find the ley sources to finish the task.

For example, after I use cd to go inside the technical directory and use cd to go inside biomed directory, I type grep -i "adults" rr37.txt. It turns out as below:

<img width="523" alt="截圖 2023-05-07 16 07 37" src="https://user-images.githubusercontent.com/130111605/236707011-6b32d10a-fd5e-4bd1-a60d-916089a72272.png">

Another example, after I use cd to go inside the technical directory and use cd to go inside 911report directory, I type grep -i "find" chapter-13.3.txt. It turns out as below:

<img width="804" alt="截圖 2023-05-07 16 09 42" src="https://user-images.githubusercontent.com/130111605/236707118-5524817f-77b3-48e1-a137-d932f63ab637.png">

------------------------------------------------------------------------------------

> **What if we do not want the specific words that is also included inside the other words but still counts by the terminal?**

> **grep -i -w "Specific String" fileName.txt:**

For example, we want to find the word "live", but if we only use **grep -i "live" CONFIG_STANDARDS.txt:**, the word like "delivery", will also counted as "live". So adding -w behind -i can avoid this problem. It will only print out the string that the user want.
Below is the picture of it.

<img width="677" alt="截圖 2023-05-07 16 16 44" src="https://user-images.githubusercontent.com/130111605/236707587-ee469923-a1d0-427f-846f-bfbd5ccfca77.png">

Another example: grep -i -w "by" ONTARIO_LEGAL_AID_SERIES.txt

<img width="704" alt="截圖 2023-05-07 16 30 07" src="https://user-images.githubusercontent.com/130111605/236707902-91acfb5a-24b9-43be-89df-8a0722c9d1ff.png">

------------------------------------------------------------------------------------

> **The last interesting ```grep``` command line I want to share is grep -i -v [string] [filename].**
If the user want to find the sentences that are not include the specific string, this command line can reverse to find out all the conditional matching sentences.

I would say we can use it for finding the words in the dictionary. limiting the strings that include the specific words can help us find out if there are words match this condtion.

For example, **grep -i -v "in" journal.pbio.0020001.txt**

<img width="770" alt="截圖 2023-05-07 16 37 08" src="https://user-images.githubusercontent.com/130111605/236708186-dd6e14aa-1156-4def-8085-d118e1b5a216.png">

We can see that all the snetences are not included the string "in".

Another example, **grep -i -v "of" journal.pbio.0020010.txt**

<img width="750" alt="截圖 2023-05-07 16 39 43" src="https://user-images.githubusercontent.com/130111605/236708268-767cb20a-6b30-4609-8199-e7a828d17851.png">

---------------------------------------------------------------
Here are four interesting "grep" command line that is found on the website and asking chatgpt for information. I ask chatgpt: "Please give me 10 interesting grep command lines to operate finding the string and finish the task."

And chatgpt said:

Certainly! Here are ten interesting grep command lines that you can use to search for strings and accomplish various tasks:

- Search for a specific string in a file:

```
grep "search_string" filename
```

- Search for a string case-insensitively:

```
grep -i "search_string" filename
```

- Count the number of occurrences of a string in a file:

```
grep -c "search_string" filename
```

- Display lines containing the string and the surrounding lines:

```
grep -A 2 -B 2 "search_string" filename
```

- Search for multiple strings using logical OR:

```
grep -e "string1" -e "string2" filename
```

- Search for lines that match a specific pattern using regular expressions:

```
grep "pattern.*" filename
```

- Search for files containing a specific string in a directory and its subdirectories:

```
grep -r "search_string" directory
```

- Search for files that do not contain a specific string in a directory and its subdirectories:

```
grep -rL "search_string" directory
```

- Print only the matching part of the line using -o option:

```
grep -o "pattern" filename
```

- Search for lines that do not match a specific pattern:

```
grep -v "pattern" filename
```

Remember to replace "search_string", "pattern", "filename", and "directory" with your actual search terms and file/directory paths. These commands will help you perform powerful text searches using grep in various scenarios.


Website reference link: [https://allthings.how/how-to-use-grep-command-in-linux/](https://allthings.how/how-to-use-grep-command-in-linux/)

Thank you so watching!

**-LAB REPORT 3 ENDED-**
