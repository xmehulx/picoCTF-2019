# 13
**Points:** 100

## Category
Cryptography

## Task
Cryptography can be easy, do you know what ROT13 is? ```cvpbPGS{abg_gbb_onq_bs_n_ceboyrz}```

# Solution
Rot13 is rotating every alphabet 13 places ahead, and for this linux has a very useful ```tr``` command

```console
r00t@linux:~$ echo 'cvpbPGS{abg_gbb_onq_bs_n_ceboyrz}' | tr '[a-zA-Z]' '[n-za-mN-ZA-M]'
picoCTF{not_too_bad_of_a_problem}
```

# Flag
> picoCTF{not_too_bad_of_a_problem}
