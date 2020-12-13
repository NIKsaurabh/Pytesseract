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
4. If the image is blur (image 8) then it reads garbage.
5. It extract all thin, thick and bold strings from the image (image 9,10).
6. It can extract strings from photos of books pages and newspaper if image is clear (image 11,12,13,14). If the image is not clear (image 15) it will read garbage.
7. In case of barcode it reads if image is super clear (image 16). If the photo of barcode is taken from camera (image 17,18) then it does not read.
8. It cannot extract strings from  *word clouds* (image 19,20).
9. Pytesseract can read easy captchas (image 21,22,23) but cannot read hard captchas (image 24,25).
10. It cannot correctly read handwritings (image 26,27,28). If handwriting is clean then it can read with some garbage.
