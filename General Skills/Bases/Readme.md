# Bases
**Points:** 100

## Category
General Skills

## Task
What does this ```bDNhcm5fdGgzX3IwcDM1``` mean? I think it has something to do with bases.

# Solution
The first thing that comes up to mind after looking at the crypted text is **[base64](https://en.wikipedia.org/wiki/Base64)**. So when we decode the base64 text we get:

```bash
$ echo 'bDNhcm5fdGgzX3IwcDM1' | base64 -d
l3arn_th3_r0p35
```

# Flag
> picoCTF{l3arn_th3_r0p35}
