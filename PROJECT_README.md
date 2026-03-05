# Ebook Search System

A Flask-based web application for searching and managing ebooks with PDF support and intelligent search capabilities.

## Features

- **Search Functionality**: Search through uploaded PDF documents using TF-IDF vectorization
- **PDF Processing**: Extract and process text from PDF files
- **Session-Based Library**: Maintain personalized ebook libraries with session management
- **Upload Management**: Upload and manage PDF ebooks
- **Similarity-Based Search**: Find similar documents using cosine similarity

## Tech Stack

- **Backend**: Flask (Python 3.12)
- **Machine Learning**: scikit-learn (TF-IDF, Cosine Similarity)
- **PDF Processing**: PyPDF2
- **Frontend**: HTML/CSS/JavaScript
- **Data Storage**: JSON

## Project Structure

```
ebook_search/
├── app.py                 # Main Flask application
├── requirements.txt       # Python dependencies
├── README.md             # This file
├── .vscode/              # VS Code settings
├── static/
│   └── style.css         # Styling
├── templates/
│   ├── base.html         # Base template
│   ├── search.html       # Search page
│   ├── library.html      # Library page
│   └── upload.html       # Upload page
├── data/
│   └── processed_data.json # Processed ebook data
└── uploads/              # Uploaded PDF files
```

## Installation

1. **Clone the repository**:
   ```bash
   git clone https://github.com/Moni-wec/ebook-search-system-monika.git
   cd ebook_search
   ```

2. **Create a virtual environment**:
   ```bash
   python -m venv venv
   ```

3. **Activate the virtual environment**:
   - **Windows**:
     ```bash
     venv\Scripts\activate
     ```
   - **macOS/Linux**:
     ```bash
     source venv/bin/activate
     ```

4. **Install dependencies**:
   ```bash
   pip install -r requirements.txt
   ```

## Usage

1. **Run the application**:
   ```bash
   python app.py
   ```

2. **Access the application**:
   - Open your browser and navigate to `http://localhost:5000`

3. **Features**:
   - **Upload**: Upload PDF ebooks to the system
   - **Search**: Search through your uploaded ebooks
   - **Library**: View and manage your ebook library
   - **Session Management**: Personal library per session (30-minute timeout)

## Requirements

- Python 3.12
- Flask
- PyPDF2
- scikit-learn

See `requirements.txt` for all dependencies.

## Configuration

The application uses the following configuration:
- **Upload Folder**: `/tmp/uploads` (or `uploads/` directory)
- **Data Storage**: JSON-based storage in `/tmp/data/processed_data.json`
- **Session Timeout**: 30 minutes
- **Debug Mode**: Enabled by default

## License

This project is open source and available under the MIT License.

## Author

Monika

## Repository

[GitHub Repository](https://github.com/Moni-wec/ebook-search-system-monika)
