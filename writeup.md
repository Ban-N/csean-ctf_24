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
Checking the file type showed me that it's a jpeg file, so I just changed the extension

-----------------------------------

## FLakes

![image](https://github.com/user-attachments/assets/92f10346-0921-4147-ab42-1f794f738c08)

I downloaded the file to my kali linux

![image](https://github.com/user-attachments/assets/d97adf26-f3c7-4e04-bfc8-75c585d657cc)

The description actually gave this challenge away, the word "snow" took my mind to "stegsnow"

![image](https://github.com/user-attachments/assets/b15ffbc0-1baa-4de7-9644-ee53ca1e2ad9)

FLAG:```csean-ctf{Just_Sn0w}24```

---------------------------

## Outguest

![image](https://github.com/user-attachments/assets/7a2e3d2c-dce3-4a12-b6ac-c4404ae530d4)

I downloaded the file to my kali linux

![image](https://github.com/user-attachments/assets/5bc57c59-83d2-431c-ac1b-220ef5af1c90)

The descirpiton of this challenge also gave it away, the word "outguess" took my mind to "outguess" (tool used for steganography)

![image](https://github.com/user-attachments/assets/d530cd62-0f5e-43bc-9856-7e79db8f5227)

FLAG:```csean-ctf{You_0ut_gue55ed_we11}24```

-----------------------------

## The Seeker

![image](https://github.com/user-attachments/assets/6609abca-d96c-433c-9e7e-18a20ec3db72)

I downloaded the file to my machine

![image](https://github.com/user-attachments/assets/072edcb3-ba3a-4173-b403-8d2d9a2dd2fd)

The description of the challenge gave it away, the word "seek" took my mind to "stegseek"

![image](https://github.com/user-attachments/assets/5c05096d-f780-48a8-86f8-f831e529bbbb)

FLAG:```csean-ctf{That_Was_S0_Fast}24```














