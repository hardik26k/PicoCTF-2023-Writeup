# Description

Try reversing this file? Can ya?

I forgot the password to this file. Please find it for me?

# Solution

```wget https://artifacts.picoctf.net/c/270/ret```

```strings ret | grep pico```

Also just for fun here is a little script that get the flag with nothing else surrounding it.

```strings ret | grep pico | cut -d "H" -f2 | cut -d ":" -f2 | tr -d "\n" | tr -d " " > flag.txt```

Flag: ```picoCTF{3lf_r...f62bc8}```
