# Arte-Miss?
In this challenge, it was told that the `mirage.jpg` had the flag. Initially I thought that the flag must've been hidden inside the image in a very small font size somewhere. But after searching for a while, it clicked to me that it could also be inside the properties of the image. So I checked it out and then found the flag under the metadata.
# This or that?
As soon as it was mentioned that the word `ARTEMIS_WHISPER` was written opposite to the character sequence I knew it was a XOR cipher as in the previous Cryptonite challenge as well, there were many XOR ciphers involved and this one had the word "exclusively" too.
`ARTEMIS_WHISPER` in hexadecimal is `415254454d49535f57484953504552`
This XORed with `036363127c7c60001a117c6463170b` gives `423137573135335f4d593537335259` 
And then finally converting the hexadecimal output to text I got the flag `B17W153_MY573RY`. 
# Keynough is enough
For this challenge, I initially thought that it is a Caesar Cipher but then there was no shift given. So I read the question again, and wondered why was vinegar mentioned? I checked online to see if there was a cipher related to it and I came across Vigenere Cipher. After understanding what it was about, it was easy for me to notice that the word `WHISPER` was the key to encode and that's how I got the flag - `OASIS{S1L3N7_V1G3N3R3}`
# BasiKEllY
The word `enigma` made me wonder if it was to be decoded using an enigma machine similar to how we had to do one task in the cryptonite challenge earlier. But I soon realised it was not that as there was no setting given for that. Again I thought of different encryption techniques and realised it was a base32 encoding as all the letters were capital and it ended with padding. After that I converted the sequence to text to obtain the flag.
# Microsoft StrongEdge
Since this was another challenge that involved an attachment my first instinct was to look at the properties of th efile again but this time there was no key there. Then I tried to check if the flag was hidden inside the ppt itself and concelaed by matching the text's color to the background. That also wasn't the case, so afyter checking each element of the ppt my cursor went over a small black color image, which then I enlarged and after flipping and rotating I got the encoded flag from it. 

`BNFVF{e0g4g0e_0s_cc75}` was in the same format as a flag, so it had to be a simple cipher whihc just substiuted the letters. So I figured out that `BNFVF` maps to `OASIS` and the letters are shifted by 13 each. After ddecoding it, I got the flag: `OASIS{r0t4t0r_0f_pp75}`
# Maze Runner
Since it was an attachement again, I tried to see if the flag was hidden inside the image or the properties of it, but it was clear that it wasn't there. Then I realised the question mentions, ideator, surname and location which means that it is related to the origin of the image. After reverse searching the image on Google I got to know it was the world's largest labyrinth in `Fontanellato, Italy`. So I got the location and then after researching I got to know the idea was given by `Jorge Luis Borges` so the surname was also found. Hence, I got the flag.
