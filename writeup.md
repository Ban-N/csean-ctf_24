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
-rw-r--r-- 1 root      root      24969 Sep 26 17:55 image_2.png
```
After downloading, I checked the file type

```
┌──(root㉿kali)-[/home/csean_ctf/steg/message]
└─# file image_2.png 
image_2.png: JPEG image data, JFIF standard 1.01, aspect ratio, density 1x1, segment length 16, comment: "use_what_you_have_to_get_what_you_want", baseline, precision 8, 697x733, components 3
```
Checking the file type showed me that it's a jpeg file, so I just changed the extension. Also, I found this comment ```use_what_you_have_to_get_what_you_want```, which I used as the password when I ran the steghide tool

```
┌──(root㉿kali)-[/home/csean_ctf/steg/message]
└─# ls -la
total 68
drwxr-xr-x 2 root      root       4096 Sep 26 19:57 .
drwxr-xr-x 6 root      root       4096 Sep 26 19:53 ..
-rw-r--r-- 1 root root 24969 Sep 26 19:41 image_2.jpeg
-rw-r--r-- 1 root root 24969 Sep 26 17:55 image_2.png
```

![image](https://github.com/user-attachments/assets/358f2b58-dffe-4d3d-9107-4ee20163d72e)

FLAG:```csean-ctf{e45y_5teg}24```

-----------------------------------

## FLakes

![image](https://github.com/user-attachments/assets/92f10346-0921-4147-ab42-1f794f738c08)

I downloaded the file to my kali linux then I opened it

![image](https://github.com/user-attachments/assets/ce87a9d7-879b-4e08-aa08-d6f6faeb9f8b)

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

The next thing I did was to analyze the xml files using sublime text. The task here is to investigate the name of the log files

For Log A

![image](https://github.com/user-attachments/assets/87c41d2a-9798-4783-a84d-d92fb316c82c)

This is a `Security Event Log`

For Log B

![image](https://github.com/user-attachments/assets/315dd387-6d05-4e05-ac93-cfbb148855cc)

This is a `PowerShell Log`

For Log C

![image](https://github.com/user-attachments/assets/5784a10d-6f35-4e93-99c5-f819c4372247)

This is a `SMBServer Log`

FLAG:```csean-ctf{Security Event Log, PowerShell Log, SMBServer Log}24```

---------------------------

## Telco - Attackers IP

![image](https://github.com/user-attachments/assets/5aad3886-6693-4f2e-bf2d-72e62fdb9eba)

The very first thing I did was grep out IP address from the logfiles I had

![image](https://github.com/user-attachments/assets/9d501017-2a79-4139-ac8c-e8f238f72235)
![image](https://github.com/user-attachments/assets/ac2411fb-799e-4e27-898a-96d4af9359bf)
![image](https://github.com/user-attachments/assets/6b9da9d7-c473-4bd0-856a-7e6734dcef21)

This showed me that only "log a" had valid Ip Addresses, so to get the Ip Addresses with the most count I wrote a script 

```python
from collections import Counter
import re

# Function to extract IP addresses from a line
def extract_ips(line):
    # Regular expression to match IPv4 addresses
    return re.findall(r'[0-9]+(?:\.[0-9]+){3}', line)

# Read the log file and count IP occurrences
def count_ips(log_file):
    with open(log_file, 'r') as file:
        # Extract all IP addresses
        ips = []
        for line in file:
            ips.extend(extract_ips(line))
        
        # Count occurrences of each IP
        ip_count = Counter(ips)

    # Print the IP addresses and their counts
    for ip, count in ip_count.items():
        print(f"{ip}: {count}")

# Example usage: replace 'logfile.txt' with your actual log file path
log_file = 'logfile_a.xml'
count_ips(log_file)
```
I got interesting stuffs when I ran my script

![image](https://github.com/user-attachments/assets/7a4f399a-f31c-4382-be07-db46a23cf1d9)

The top 3 Ips here are `102.164.18.195`, `181.188.139.179` and `23.4.4.223`, but then `23.4.4.223` isn't a valid ip so I added the next ip that had most count which is `31.189.124.173`

FLAG:```csean-ctf{102.164.18.195, 181.188.139.179, 31.189.124.173}24```

-----------------------------

## Telco - Compromise Server

![image](https://github.com/user-attachments/assets/e1884a8e-9a34-42be-ab4e-d2adf43742ca)

The task here is to find one of the compromised servers, this was quite easy actually

Analyzing "log a" on sublime text I found a windows server

![image](https://github.com/user-attachments/assets/163d5427-e185-4505-a142-2625add87e1b)

FLAG:```csean-ctf{WIN-86KKNGTVC25}24```



# Misc
<hr>

## ChatGPT

![image](https://github.com/user-attachments/assets/59a8b8a4-77bb-4976-8025-1b0cb42150ba)

Upon checking the source, I found some gibberish stuffs

![image](https://github.com/user-attachments/assets/dcfaae14-f629-432c-8596-9e4dd57a6a2b)

I tried decoding it because I thought it was a cipher, but then it's not a cipher. There's a pattern

What I did was eliminate the non capital letters, which left me with this 

```
RANDOM NOT RANDOM
```

FLAG:```csean-ctf{RANDOM_NOT_RANDOM}24```

--------------------------------

## DissKod

![image](https://github.com/user-attachments/assets/3c1c4f2b-b390-42c7-8c75-82e4d491710e)

The "announcement-hint" channel had the flag

![image](https://github.com/user-attachments/assets/bb1dd98f-36f2-4ad1-87eb-ef2dc3534341)

Clicking on that black text revealed the flag

![image](https://github.com/user-attachments/assets/afe9f813-3231-4244-ad73-3a4fca6f4a43)

FLAG:```csean-ctf{hidden_in_plain_sight}24```













































