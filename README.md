# Image Steganography
PURPOSE
-The purpose of Steganography is to maintain secret communication between two parties.
The main objective of our project is to provide security based on          steganography techniques to hide message carried by stego - media (image) which should not be sensible to human beings and avoid drawing suspicion to the existence of hidden message. 

The main feature of IMAGE STEGANOGRAPHY is to encode and decode the hidden messages.
This presentation focuses on the numerous steps to successfully embed and retrieve the data within an image.
To ensure that our GUI-based application is user friendly.

Image Steganography is categorised into two modules:-
- Encode
- Decode

- Encode: -
Can choose an image of format .png, .jpg, . jpeg or all files as well but can encode the message and save it only in .png format.
Can enter a secret message in order to encode it into the selected image.
 
- Decode: -
Here users can select the image to extract the hidden message.
Image should be of the .png format.

#WORKING OF IMAGE STEGANOGRAPHY

1.	Pixels are the building blocks of an image.
2.	Every pixel contains three values: (red, green, blue) also known as RGB values.

- Encode

Suppose the message to be hidden is ‘GIET’.
Here, only encoding of ‘G’ is considered for instance.

ASCII value of G is 71.
8-bit binary equivalent is 01000111

First 3 pixel values: (188, 155, 168), (70, 167, 116), (132, 173, 97)                                [0 : even and 1:odd]

0              1              0                   0                0                   1                   1                  1
155           188         168               70             167                116                132              173      97

New Image rgb values:
154           187         168               70              166                115                131              173     96

Similarily “IET” can be encoded.

- Decode
154           187         168               70              166                115                131              173     96

8-bit binary equivalent:
0               1             0                   0                 0                   1                     1                  1       
Ninth value is even, so we continue the steps till it encounters odd.
This binary data (01000111) decimal value is 71 and in ASCII it represents ‘G’

Hence, we get the ‘G’ decoded.



**Screenshots**
![Screenshot (241)](https://user-images.githubusercontent.com/79132253/124146580-86288f80-daab-11eb-8726-071213b1e493.png)
![Screenshot (242)](https://user-images.githubusercontent.com/79132253/124146595-8b85da00-daab-11eb-8855-e1d4ce277438.png)
![Screenshot (243)](https://user-images.githubusercontent.com/79132253/124146607-8f196100-daab-11eb-9c50-51b54d240df7.png)
![Screenshot (244)](https://user-images.githubusercontent.com/79132253/124146629-95a7d880-daab-11eb-96e5-98a202019a9c.png)
![Screenshot (245)](https://user-images.githubusercontent.com/79132253/124146644-993b5f80-daab-11eb-8fc6-c1bb0f2886ae.png)

**Conclusion**
From the proposed project we have learned that while implementing Image Steganography is important, and the methods to do so are far more complex than actually doing the Steganography itself.
There is a lot of research that is beginning to discover new ways to detect Steganography, most of which involves some variation of statistical analysis. It is interesting to see what other methods will be developed and how accurate they will be at detecting Steganography. 
Although it is a simple designed but effective one.

**Future Scope**
The overall project can be upgraded by adding support to decode all file formats.
Secondly, we can add a backend to store all the decoded messages by implementing it in html, css, MongoDb.






