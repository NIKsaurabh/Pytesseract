# Pytesseract
I have used Pytesseract on anaconda which is installed on my ubuntu 20.04 OS. For using Pytesseract in windows we have to set path but in linux just run following command on your terminal and you are ready to roll.

#### sudo apt update
#### conda install -c conda-forge pytesseract 
#### sudo apt install tesseract-ocr
#### sudo apt install libtesseract-dev

### Some of my findings using Pytesseract
1. It completely reads the crisp and clear text written in black on white background (image 1) and even hindi language (image 2).
2. If a text is written in white on black background (image 3) then pytesseract does not read it correctly if the same text is in black on white background (image                4) it reads correctly.
3. Pytesseract can extract numbers and alphabets from number plate of vehicle (image 5,6). If the number plate is on the vehicle then it cannot extract string from that image (image 7).
4. 
