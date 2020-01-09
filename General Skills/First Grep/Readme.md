# First Grep
**Points:** 100

## Category
General Skills

## Task
Can you find the flag in [file](https://2019shell1.picoctf.com/static/3f6065eec2d3ed644932ada577a74334/file)? This would be really tedious to look through manually, something tells me there is a better way. You can also find the file in /problems/first-grep_0_93be1631acf1a93b98cdcc3e7b9fdc52 on the shell server.

# Solution
When we SSH into the server and open the file after navigating to the folder, there is a lot of (gibberish) text. The name of the challenge gives hint by itself. We have to filter out the text we wanna find from all this. And for that we use the ```grep``` command.
```bash
$ cat file | grep 'picoCTF'
picoCTF{grep_is_good_to_find_things_4b2451ea}
```

# Solution
> picoCTF{grep_is_good_to_find_things_4b2451ea}
