# extensions
**Points:** 150

## Category
Forensics

## Task
This is a really weird text file [TXT](https://2019shell1.picoctf.com/static/45886ed4b6d5d1dc74c4944fcf4b4041/flag.txt)? Can you find the flag?

# Solution
As the text file wasn't opening, we then find what type of file it is using the `file` command.

```console
r00t@linux:~$ file flag.txt
flag.txt: PNG image data, 1697 x 608, 8-bit/color RGB, non-interlaced
```
So, the file is actually an image file. To get the flag we will open it with an image viewer.

# Flag
> picoCTF{now_you_know_about_extensions}
