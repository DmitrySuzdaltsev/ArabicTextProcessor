# Arabic Text Toolkit

A Python library for processing Arabic text, including methods for diacritization, phonemization, and removing diacritics. The toolkit is designed to handle Arabic text and convert it into a phonemic representation following the IPA (International Phonetic Alphabet) standards.

## Features

- **Diacritization**: Automatically adds diacritics (harakats) to Arabic text using a pre-trained model.
- **Phonemization**: Converts Arabic text into a sequence of phonemes, conforming to IPA standards.
- **Diacritics Removal**: Strips diacritical marks from Arabic text, making it easier to handle unvocalized text.

## Installation

Clone the repository and install the required dependencies:

```bash
git clone https://github.com/yourusername/ArabicTextToolkit.git
cd ArabicTextToolkit
pip install -r requirements.txt
```

## Usage
```
from ArabicTextHandler import ArabicTextHandler

# Original Arabic text
input_text = "اللغة العربية جميلة جداً."

# Create an instance of the text handler
text_handler = ArabicTextHandler()

# Remove diacritical marks
cleaned_text = text_handler.strip_diacritics(input_text)
print(f"Text without diacritics: {cleaned_text}")

# Apply diacritical marks
diacritized_text = text_handler.apply_diacritics(cleaned_text)
print(f"Diacritized text: {diacritized_text}")

# Phonemize the text
phonemized_text = text_handler.phonemize_text(input_text)
print(f"Phonemized text: {phonemized_text}")
```
