# GUI-Encryption
#FCAI Team
The provided code is a Python script that implements a graphical user interface (GUI) for encrypting text using three different ciphers: Playfair Cipher, Monoalphabetic Cipher, and Caesar Cipher.
- !pip install ipywidgets --> This line installs the ipywidgets library, which is used to create interactive widgets in Jupyter notebooks.
- !jupyter nbextension enable --py widgetsnbextension --> This line enables the widgetsnbextension Jupyter notebook extension, which is required for using the widgets in the notebook.
- from ipywidgets import * --> This line imports all the widgets from the ipywidgets library.
- from IPython.display import display --> This line imports the display function from the IPython.display module, which is used to display the widgets in the notebook.
- Playfair Cipher Encrypt: Key Matrix: A key matrix (5x5 grid) is generated from a keyword. The letters of the keyword are arranged in a grid, and the remaining letters of the alphabet are added in order, excluding duplicates and the letters already in the grid. Typically, 'I' and 'J' are treated as the same letter.
  - if repeated letter in a pair, insert filler like 'X’ 
    (Ex. balloon will treated as ba lx lo on).
  - if both letters fall in the same row, replace each with letter to right      
    (wrapping back to start from end) (EX. ar encrypted as RM) .
  - if both letters fall in the same column, replace each with the letter below
     it (again wrapping to top from bottom) (EX. mu encrypted as CM).
  - otherwise each letter is replaced by the letter in the same row and in the
     column of the other letter of the pair (EX. hs  BP and ea IM/JM).
- Monoalphabetic Cipher Encrypt: A Monoalphabetic Cipher is a substitution cipher where each letter in an alphabet is mapped to its unique letter in the same or another alphabet. It is a type of simple substitution cipher, where each letter is replaced with another letter consistently throughout the text. This means that the same plaintext letter will always be replaced by the same ciphertext letter.
- Ceaser Cipher Encrypt: The Caesar Cipher is a substitution cipher where each letter in the plaintext is shifted a certain number of places down or up the alphabet. It is named after Julius Caesar, who is historically recorded as using this type of encryption to protect his messages.


