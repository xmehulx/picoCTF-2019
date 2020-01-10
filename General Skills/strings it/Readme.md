# strings it
**Points:** 100

## Category
General Skills

## Task
Can you find the flag in [file](https://2019shell1.picoctf.com/static/762b9a36a6da791e3f61713fcfaf1721/strings) without running it? You can also find the file in /problems/strings-it_2_865eec66d190ef75386fb14e15972126 on the shell server.

# Solution
As it mentions _not_ to run the file, we can deduce that it is an executable file, and we simply can't print out its contents. For this, we can make use of ```strings``` command.

```console
r00t@linux:~$ file strings
strings: ELF 64-bit LSB pie executable, x86-64, version 1 (SYSV), dynamically linked, interpreter /lib64/ld-linux-x86-64.so.2, for GNU/Linux 3.2.0, BuildID[sha1]=c9fbfa12e19efdabab88839c5e8b931b5e62c503, not stripped
root@linux:~$ cat strings | strings | grep picoCTF
picoCTF{5tRIng5_1T_d5b86184}
```

# Flag
> picoCTF{5tRIng5_1T_d5b86184}
