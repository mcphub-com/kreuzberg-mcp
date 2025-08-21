# Kreuzberg MCP Server

A Model Context Protocol (MCP) server for document intelligence and text extraction using the Kreuzberg framework.

## Overview

This MCP server provides powerful document processing capabilities through the Model Context Protocol, enabling AI assistants to extract text, metadata, and structured data from diverse file formats.

## Features

- **Document Text Extraction**: Extract text from PDFs, images, Office documents, HTML, and more
- **OCR Support**: Multiple OCR backends (Tesseract, EasyOCR, PaddleOCR)
- **Structured Data**: Extract tables, entities, and keywords
- **Content Chunking**: Split documents into manageable chunks
- **PDF Download**: Download and cache PDFs from URLs
- **Configuration Management**: Flexible configuration system

## Supported Formats

- PDF documents
- Images (PNG, JPG, JPEG, TIFF, BMP, WEBP)
- Office documents (DOCX, PPTX, XLSX)
- HTML files
- Text files (TXT, CSV, TSV)
- And more...

## MCP Tools

### `extract_document`
Extract comprehensive text content and metadata from a document file.

### `extract_bytes`
Extract text content from base64-encoded document bytes.

### `extract_simple`
Simple text extraction from a document file (returns plain text).

### `get_pdf_local_path`
Download a PDF from a URL and return the local file path.

## MCP Resources

- `config://default` - Default extraction configuration
- `config://discovered` - Configuration discovered from config files
- `config://available-backends` - Available OCR backends
- `extractors://supported-formats` - Supported document formats

## MCP Prompts

- `extract_and_summarize` - Extract text and provide summarization prompt
- `extract_structured` - Extract text with structured analysis prompt

## Usage

The server is designed to run in a Docker container and communicate via the Model Context Protocol.

## Configuration

The server supports flexible configuration through:
- Configuration files (automatically discovered)
- Tool parameters (override defaults)
- Environment variables

## License

MIT License - see the project repository for details.
