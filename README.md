# Google Translate API for Python

This repository shows you how to use the `googletrans` library. A library that allows you to use Google Translate in Python. This repository contains three notebooks:
1. `main.ipynb`
2. `translate_txt_file.ipynb`
3. `translate_pdf_file.ipynb`

There is a YouTube tutorial that explains the notebooks in details. If you want to watch it, you can find it [here](https://www.youtube.com/watch?v=CkPvqLvuq2A).

## main.ipynb

In this notebook, you can see the supported languages, as well as how to translate a simple string from English to French.

## translate_txt_file.ipynb

In this notebook, you will read a TXT file -make sure to change the path accordingly-.

```python
with open('./video_script.txt', 'r') as f:
    text = f.read()
```

After that, you will translate it into another language and then save the translation into a new TXT file.

## translate_pdf_file.ipynb

In this notebook, you will use `PyPDF2` to load a PDF file and extract the text from it

```python
from PyPDF2 import PdfReader


reader = PdfReader("./Google_trans_docs.pdf")
number_of_pages = len(reader.pages)
print(f"Number of pages: {number_of_pages}")
```

After that, you will translate the PDF into another language and then save the translation into a TXT file.
