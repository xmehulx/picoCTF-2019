# So Meta
**Points:** 150

## Category
Forensics

## Task
Find the flag in this [picture](https://2019shell1.picoctf.com/static/973cd0e3beea255e6a0b5316aa6287ce/pico_img.png). You can also find the file in /problems/so-meta_5_7c198bd3e228862d97a40316b8a103e4.

# Solution
Once again, as the name suggest, it has to do something with the meta data of the image. We will start by dumping the file contents using `hexdump`.
```console
r00t@linux:~$ hexdump -C pico_img.png
...
...
0001a8c0  57 6c 17 00 00 00 20 74  45 58 74 41 72 74 69 73  |Wl.... tEXtArtis|
0001a8d0  74 00 70 69 63 6f 43 54  46 7b 73 30 5f 6d 33 74  |t.picoCTF{s0_m3t|
0001a8e0  61 5f 66 66 64 30 39 63  30 66 7d 9e bc dc 5b 00  |a_ffd09c0f}...[.|
0001a8f0  00 00 00 49 45 4e 44 ae  42 60 82                 |...IEND.B`.|
0001a8fb
```
and voilà, we get the flag!

# Flag
> picoCTF{s0_m3ta_ffd09c0f}
