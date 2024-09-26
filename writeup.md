# Team Name: Sate Sate Sate


# Steganography
<hr>

## Message

![image](https://github.com/user-attachments/assets/c49ff38e-f192-4411-95c1-b4dc844426d7)

``` 
┌──(root㉿kali)-[/home/csean_ctf/steg/message]
└─# ls -la
total 36
drwxr-xr-x 2 root      root       4096 Sep 26 17:56 .
drwxr-xr-x 3 root      root       4096 Sep 26 17:49 ..
-rw-r--r-- 1 bl4ck4non bl4ck4non 24969 Sep 26 17:55 image_2.png
```
After downloading, I checked the file type

```
┌──(root㉿kali)-[/home/csean_ctf/steg/message]
└─# file image_2.png 
image_2.png: JPEG image data, JFIF standard 1.01, aspect ratio, density 1x1, segment length 16, comment: "use_what_you_have_to_get_what_you_want", baseline, precision 8, 697x733, components 3
```
That's how I got the flag

FLAG:```csean-ctf{use_what_you_have_to_get_what_you_want}24```
