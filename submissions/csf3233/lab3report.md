# CSM3233 Lab 3
#### Gary Lim S62079

<div style="page-break-after: always"><br></div>

## TASK 1: INSTALLING A HASH CHECKING TOOL

1. List four examples of hash algorithms. 
	1. SHA1
	2. SHA256
	3. SHA384
	4. SHA512
2. What is the issue with the MD5 algorithm?
	- "A major concern with MD5 is the potential it has for message collisions when message hash codes are inadvertently duplicated"

<div style="page-break-after: always"><br></div>

## TASK 2: CHECKING THE INTEGRITY OF THE DOWNLOADED FILE

![](20231108084322.png)

1. Describe the functionality of hashing encryption compared to symmetric and asymmetric encryption.
	- There is no key in hashing.

<div style="page-break-after: always"><br></div>

## TASK 3: INSTALLATION OF ENCRYPTION TOOL

![](20231108084836.png)

![](20231108085047.png)

1. What is the meaning of GPG? 
	- It is a tool to provide digital encryption and signing services using the OpenPGP standard.
2. Using your own words, explain the difference Between PGP and GnuPG?
	- As mentioned, GPG is open sourced version of PGP, both are used to do digital encryption magic, GPG is more in depth and feature rich, while PGP is more user friendly. 

<div style="page-break-after: always"><br></div>

## TASK 4: SHARING A PUBLIC KEY AND ENCRYPTING A FILE

![](20231108093051.png)

<div style="page-break-after: always"><br></div>

## TASK 5: DECRYPTING AN ENCRYPTED FILE

![](20231108092727.png)

![](20231108093337.png)

<div style="page-break-after: always"><br></div>

1. Why cryptography is important in cybersecurity? 
	- because you don't want secrets leaking everywhere
2. Give one example of an application that applied cryptography in our daily life. 
	- messaging app such as Messenger, WhatsApp and Telegram
3. Describe an example of such an application in question 2 which related to the objectives of cryptography. 
	- the message is encrypted p2p so that the message is only known by 2 and only 2 people (supposedly) with the key
4. Describe five (5) differences between symmetric and asymmetric encryption for cryptography. 
	1. Symmetric uses public key, asymmetric uses public and private keys.
	2. Due to that you don't have to share key in asymmetric. 
	3. Symmetric is faster, asymmetric is slower. 
	4. Symmetric encryption efficient for large data, asymmetric is for key exchange and digital signatures.
	5. Symmetric is for data privacy, asymmetric is for secure communication and authentication.
5. List five (5) differences between cryptography and steganography.
	1. Cryptography secures data through encryption with visible scrambled text.
	2. Steganography hides data within other data to keep it secret.
	3. Cryptography emphasizes security and relies on keys.
	4. Steganography focuses on secrecy by concealing data in plain sight.
	5. Cryptography is easily detectable, while steganography is harder to detect.