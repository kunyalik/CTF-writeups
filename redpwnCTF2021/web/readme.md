# Web

## Inspect-me

**Points:** 101

### Solution

The challenge pointed towards checking the source code of a given website.

### Flag

 flag{inspect_me_like_123} 

---

## orm-bad

**Points:** 102


### Solution

It seemed like an SQLi challenge.
Sending the injection :
>username:`' OR 1=1 --` and password: ` 'OR 1=1 --`

gave us the flag

### Flag

flag{sqli_overused_again_0b4f6}

---

## secure

**Points:** 104


### Solution

This one also seemed like an SQLi challenge.
Sending the injection :

>username:`' OR 1=1 --`  password: ` 'OR 1=1 --`

doesn't give us the flag.
Looking at the `index.js` provided,we could see that the input is being converted to base64 using `btoa` function.

Altering the *POST* request in firefox using

>username:`admin` password:`'OR 1=1 --`

This gives us the flag.
### Flag

flag{50m37h1n6_50m37h1n6_cl13n7_n07_600d}

---

