# PDF Translator

This tool translates PDF documents while preserving the original format, including text positioning and images.

## Features

- Extract text from PDF files
- Translate text to any supported language using Google Translate
- Create a new PDF with translated text while maintaining the original format
- Preserve images from the original PDF

## Requirements

- Python 3.6+
- Required Python packages:
  - PyPDF2
  - deep-translator
  - reportlab

## Installation

Install the required packages:

```bash
pip install PyPDF2 deep-translator reportlab
```

## Usage

```bash
python pdf_translator.py <input_pdf> <target_language>
```

Example:

```bash
python pdf_translator.py sample.pdf es  # Translate to Spanish
python pdf_translator.py sample.pdf fr  # Translate to French
python pdf_translator.py sample.pdf de  # Translate to German
```

The translated PDF will be saved as `<original_filename>_<language_code>.pdf`.

## Supported Languages

The tool supports all languages available in Google Translate. Some common language codes:

- `es`: Spanish
- `fr`: French
- `de`: German
- `it`: Italian
- `ja`: Japanese
- `ko`: Korean
- `zh-cn`: Chinese (Simplified)
- `ru`: Russian

## Limitations

- The current implementation has a simplified approach for handling images
- Complex PDF layouts might not be perfectly preserved
- Very large PDFs might encounter translation API limits

## License

MIT
