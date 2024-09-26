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
Checking the file type showed me that it's a jpeg file, so I just changed the extension. Also, I found this comment ```use_what_you_have_to_get_what_you_want```, which I used as the password when I ran the steghide tool

![image](https://github.com/user-attachments/assets/358f2b58-dffe-4d3d-9107-4ee20163d72e)

FLAG:```csean-ctf{e45y_5teg}24```

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

 
# Forensics
<hr>

## ids

![image](https://github.com/user-attachments/assets/242dc6ea-c10c-4722-8482-84a4614bd224)

I downloaded the file to my kali machine

![image](https://github.com/user-attachments/assets/e3a2c80a-2c29-4171-9be4-9c0b4722bd61)

Catting the file gave me some weird stuffs, but then the name of the file gave it away. It's a hexadecimal string. So I just decoded with cyberchef

![image](https://github.com/user-attachments/assets/fed4f46f-5b55-4b48-9a6c-c1f2af4e255c)

FLAG:```csean-ctf{y0u_got_m3}24```

-----------------------

## sus

![image](https://github.com/user-attachments/assets/8bddde2f-ad64-4c31-b782-106f62fd4a65)

I downloaded the file to my kali machine

![image](https://github.com/user-attachments/assets/59d22763-abbf-4f7e-8702-8cebe78806f5)

I analyzed this using sublime text, and then I noticed something

![image](https://github.com/user-attachments/assets/855b7843-8031-478b-a56f-0a266458ef4f)

So , this is a mail between two people. Reading their conversations I saw this

![image](https://github.com/user-attachments/assets/9231101f-d52c-421d-a679-3571cef680a1)

There's a png file that was sent, but then it is in base64 format. So I copied the base64, saved it to my device 

![image](https://github.com/user-attachments/assets/46524c62-e6ef-47f6-9452-e8508499b1ee)

I then uploaded it to cyberchef so I can save the output in png format

![image](https://github.com/user-attachments/assets/40755c5f-1d13-4fce-ad24-d78edd4f36a3)
![image](https://github.com/user-attachments/assets/afd654f4-df65-4e6e-a4a7-c3f78285ac04)

Checking the content of the image gave me the flag

FLAG:```csean-ctf{4n4lyze_3verything_luffy}24```

----------------------------------

## Telco- Log Identification

![image](https://github.com/user-attachments/assets/83f9749a-4411-409d-ac4d-eaeadb004e0c)

I downloaded those files to my machine then converted them to xml files

![image](https://github.com/user-attachments/assets/2c6da451-77a7-4da3-9909-b2f31afd2bb1)

The next thing I did was to analyze the xml files using sublime text.











































