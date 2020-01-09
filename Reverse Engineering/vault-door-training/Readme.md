# vault-door-training
**Points:** 50

## Category
Reverse Engineering

## Task
Your mission is to enter Dr. Evil's laboratory and retrieve the blueprints for his Doomsday Project. The laboratory is protected by a series of locked vault doors. Each door is controlled by a computer and requires a password to open. Unfortunately, our undercover agents have not been able to obtain the secret passwords for the vault doors, but one of our junior agents obtained the source code for each vault's computer! You will need to read the source code for each level to figure out what the password is for that vault door. As a warmup, we have created a replica vault in our training facility. The source code for the training vault is here: [VaultDoorTraining.java](https://2019shell1.picoctf.com/static/f0e644817bb3fc5975a7b8e99b8d7cf9/VaultDoorTraining.java)

# Solution
Simply open the java file using any text editor and at the end you'll see something like
```java
...
public boolean checkPassword(String password) {
    return password.equals("w4rm1ng_Up_w1tH_jAv4_c0b141c5e30");
}
```

# Flag
> picoCTF{w4rm1ng_Up_w1tH_jAv4_c0b141c5e30}
