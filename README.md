# Pytesseract Coordinate Finder
Using PyTesseract, it locates text on the screen, and grabs the screen coordinates (x,y) of the center of the word (or individual letters *configurable*).
Doesn't do that stupid glyph thing where it makes boxes around text, it just grabs the coordinates of the text. (I made this because all I could find was how to make the glyph)

## Installation

### Install Modules

#### PyTesseract

Install required packages:
```
py -m pip install pytesseract
py -m pip install Pillow
```

#### pyautogui
Install required packages:
```
py -m pip install pyautogui
```

#### pygetwindow
Install required packages:
```
py -m pip install pygetwindow
```

### Configure PyTesseract
PyTesseract requires both the python module, and the OCR folder, so you must have the [Tesseract-OCR](<https://github.com/DiamondYTR/pytesseract-coordinate-finder/tree/main/Tesseract-OCR>) folder in the same folder as the python script.

## Usage
The function "locate_text", takes two arguments, "word", and "letter".

(**word**) is the word that you want to scan for, you cannot scan for sentences.

(**letter**) *is optional*, it will scan for the specific letter within the word's coordinates.

The function returns the coordinates of whatever data you specify.

```
Ex) locate_text("Multiplayer")
```
This will return the coordinates of the middle of the word, in this case, that would be the coordinates of the center of the letter "p" (found automatically)

```
Ex) locate_text("Multiplayer", "r")
```
This will return the coordinates of the center of the letter "r", as opposed to the full word.
This is because you specified you want the coordinates of that specific letter.

## Notes
This program was made in help by ChatGPT, which is why you may see occasional comments throughout the script, though in some areas I heavily modified the original content, so the comments may not always be accurate.

This is my first time using GitHub, I only made this because I know I would've killed to have this when I was originally just trying to make simple text recognition to grab the coordinates of a button on my monitor. So if this repository looks a little off, that's probably why.

I hope this code could be of help to you!




