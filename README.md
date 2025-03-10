# Mistral OCR PDF-to-HTML Converter

[Google Collab Link](https://colab.research.google.com/drive/1OnAxHy0ZKiP31yx0o6iSyPbng7NbAaue?usp=sharing))

A collection of Jupyter notebooks for converting PDF documents to accessible, structured HTML using Mistral AI's OCR and vision capabilities.

## Overview

This project provides tools to transform PDF documents into well-structured, WCAG-compliant HTML that preserves the original document's layout, formatting, and content. It uses Mistral's OCR API to extract text and images, then processes them to create accessible web content.

## Notebooks

This repository contains the following notebooks:

### 1. `structured_ocr.ipynb`
The original example notebook from Mistral that demonstrates basic OCR extraction and structured data formatting.

### 2. `custom-structured-ocr.ipynb`
A simplified notebook for PDF-to-HTML conversion with a focus on Google Colab compatibility. Features include:
- PDF upload via Google Colab's file upload mechanism
- OCR processing with Mistral OCR
- Basic HTML conversion with preserved layout
- Image extraction with basic alt text
- Download capability for the generated HTML

### 3. `custom-structured-ocr-v2.ipynb`
An enhanced version with advanced accessibility features:
- Full WCAG 2.1 compliance
- Screen reader optimized content
- Semantic HTML5 structure
- AI-generated descriptive alt text for images using Pixtral 12B
- Enhanced table accessibility with proper ARIA attributes
- Proper document structure and heading hierarchy

## Getting Started

### Prerequisites
- Google Colab account (for running the notebooks in the cloud)
- Mistral API key from [Mistral Platform](https://console.mistral.ai/api-keys/)

### Running the Notebooks
1. Open the desired notebook in Google Colab
2. Enter your Mistral API key in the designated cell
3. Run the cells in sequence
4. Upload your PDF when prompted
5. The notebook will process your document and create the HTML output
6. Download the generated HTML file

## Features

### OCR Processing
- Extracts text while preserving formatting
- Identifies and extracts images with their positions
- Maintains the document's structure and layout

### Accessibility Features
- Semantic HTML5 elements (`<main>`, `<section>`, `<figure>`, etc.)
- ARIA landmarks and regions
- Proper heading hierarchy
- Skip links for keyboard navigation
- High contrast text (WCAG AA 4.5:1 ratio)
- Proper image alt text
- Accessible tables with proper markup
- Print-friendly styling

### Image Processing
- AI-generated descriptive alt text
- Special handling for charts and graphs
- Figure captions for complex images

## API Usage Notes

This project uses:
- **Mistral OCR API** (`mistral-ocr-latest`) for text and image extraction
- **Pixtral 12B** (`pixtral-12b-latest`) for image understanding and alt text generation

Note that API usage incurs costs according to your Mistral AI account plan.

## Contributing

Feel free to fork this repository and submit pull requests with improvements or features.

## License

This project is provided as-is for educational and demonstrative purposes.

## Acknowledgments

- [Mistral AI](https://mistral.ai/) for providing the OCR and language model APIs
- WCAG guidelines for accessibility best practices
