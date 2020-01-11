# vault-door-1
**Points:** 100

## Category
Reverse Engineering

## Task
This vault uses some complicated arrays! I hope you can make sense of it, special agent. The source code for this vault is here: [VaultDoor1.java](https://2019shell1.picoctf.com/static/2e4a9c36c1d51d5de4c82f7507c69bf7/VaultDoor1.java)

# Solution
Upon opening the java file, we can  see the function `checkPassword`
```java
public boolean checkPassword(String password) {
    return password.length() == 32 &&
           password.charAt(0)  == 'd' &&
           password.charAt(29) == '7' &&
           password.charAt(4)  == 'r' &&
           password.charAt(2)  == '5' &&
           password.charAt(23) == 'r' &&
           password.charAt(3)  == 'c' &&
           password.charAt(17) == '4' &&
           password.charAt(1)  == '3' &&
           password.charAt(7)  == 'b' &&
           password.charAt(10) == '_' &&
           password.charAt(5)  == '4' &&
           password.charAt(9)  == '3' &&
           password.charAt(11) == 't' &&
           password.charAt(15) == 'c' &&
           password.charAt(8)  == 'l' &&
           password.charAt(12) == 'H' &&
           password.charAt(20) == 'c' &&
           password.charAt(14) == '_' &&
           password.charAt(6)  == 'm' &&
           password.charAt(24) == '5' &&
           password.charAt(18) == 'r' &&
           password.charAt(13) == '3' &&
           password.charAt(19) == '4' &&
           password.charAt(21) == 'T' &&
           password.charAt(16) == 'H' &&
           password.charAt(27) == '4' &&
           password.charAt(30) == 'f' &&
           password.charAt(25) == '_' &&
           password.charAt(22) == '3' &&
           password.charAt(28) == '8' &&
           password.charAt(26) == '2' &&
           password.charAt(31) == '0';
}
```
Upon rearranging the characters according to their index, we can easily find the flag.

# Flag
> picoCTF{d35cr4mbl3_tH3_cH4r4cT3r5_2487f0}
