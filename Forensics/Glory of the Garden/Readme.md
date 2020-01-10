# Glory of the Garden
**Points:** 50

## Category
Forensics

## Task
This [garden](https://2019shell1.picoctf.com/static/86137520022d967547d5a2c99f4231f2/garden.jpg) contains more than it seems. You can also find the file in /problems/glory-of-the-garden_2_258af8e13bd7259207af0b0ee6fab645 on the shell server. 

## Solution
Opening the photo gives nothing but on examining the file contents using ```hexdump``` we get
```console
r00t@linux:~$ hexdump -C garden.jpg
...
...
00230550  a2 bb bd ac 96 87 98 e4  d3 b2 e8 7f ff d9 48 65  |..............He|
00230560  72 65 20 69 73 20 61 20  66 6c 61 67 20 22 70 69  |re is a flag "pi|
00230570  63 6f 43 54 46 7b 6d 6f  72 65 5f 74 68 61 6e 5f  |coCTF{more_than_|
00230580  6d 33 33 74 73 5f 74 68  65 5f 33 79 33 31 65 30  |m33ts_the_3y31e0|
00230590  61 66 35 43 37 7d 22 0a                           |af5C7}".|
00230598

```

## Flag
> picoCTF{more_than_m33ts_the_3y31e0af5C7}
