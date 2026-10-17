# Doctor Prescription Analyzer

A web-based application designed to analyze medical prescription images and convert prescription information into structured digital data.

The project provides an interactive interface for uploading prescription images, processing extracted prescription information, and storing structured analysis data using Vercel Blob storage.

## Key Features

- **Prescription Image Upload** - Upload medical prescription images through an interactive interface.
- **Drag & Drop Support** - Easily select prescription images using drag-and-drop functionality.
- **Prescription Data Processing** - Organizes analyzed prescription information into structured data.
- **Patient-Based Records** - Creates prescription records associated with patient information.
- **Cloud Storage Integration** - Stores structured prescription data using Vercel Blob.
- **Responsive Interface** - Modern web interface built using React and Tailwind CSS.
- **Error Handling** - Provides feedback for upload and processing failures.
- **Secure Configuration** - Uses environment variables for storage configuration instead of hardcoding credentials.

## Tech Stack

| Technology | Purpose |
|---|---|
| React | Frontend development |
| Vite | Development and build tooling |
| JavaScript | Application logic |
| Tailwind CSS | User interface styling |
| Lucide React | Interface icons |
| Vercel Blob | Cloud-based data storage |
| ESLint | Code quality and linting |
| Vercel | Application deployment |

## Application Workflow

```text
Prescription Image
        |
        v
Image Upload
        |
        v
Prescription Analysis
        |
        v
Extracted Information
        |
        v
Structured Prescription Data
        |
        v
Patient Prescription Record
        |
        v
Vercel Blob Storage
```

## Project Structure

```text
Doctor-Prescription-Analyzer/
|
|-- public/
|-- src/
|   |-- assets/
|   |-- App.css
|   |-- App.jsx
|   |-- index.css
|   |-- main.jsx
|   `-- Page.jsx
|
|-- .gitignore
|-- eslint.config.js
|-- index.html
|-- package.json
|-- README.md
`-- vite.config.js
```

### Core Application

`src/Page.jsx` contains the primary prescription-analysis interface and application workflow, including image handling, prescription data processing, and cloud-storage integration.

## Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/GoelAnshul24/Doctor-Prescription-Analyzer.git
cd Doctor-Prescription-Analyzer
```

### 2. Install dependencies

Make sure Node.js and npm are installed.

```bash
npm install
```

### 3. Configure environment variables

The application uses Vercel Blob for storage. Configure the required environment variables locally rather than hardcoding credentials in the source code.

Example:

```env
VITE_BLOB_READ_WRITE_TOKEN=your_vercel_blob_token
```

Never commit real API keys, access tokens, passwords, or other credentials to GitHub.

### 4. Start the development server

```bash
npm run dev
```

Open the local URL displayed by Vite in your browser.

## Available Scripts

```bash
npm run dev
```

Starts the development server.

```bash
npm run build
```

Creates a production build.

```bash
npm run lint
```

Runs ESLint checks.

```bash
npm run preview
```

Locally previews the production build.

## Deployment

The application is deployed using Vercel.

**Live Application:** [Doctor Prescription Analyzer](https://htd-deploy.vercel.app/)

## Security

- Sensitive credentials should be stored using environment variables.
- Vercel Blob access tokens should never be committed to the repository.
- Prescription and patient information may contain sensitive data and should be handled appropriately.
- Public demonstrations should use fictional or anonymized prescription information.

## Future Improvements

- Improve prescription information extraction and validation.
- Add structured medicine and dosage verification.
- Improve handling of unclear or incomplete prescription images.
- Add secure user authentication.
- Add prescription history and search functionality.
- Improve storage and retrieval of patient prescription records.
- Add automated testing and stronger error handling.

## Disclaimer

This project is intended for educational and demonstration purposes. Prescription-analysis results should not be treated as a substitute for verification by a qualified healthcare professional.

## Author

**Anshul Goel**

GitHub: [GoelAnshul24](https://github.com/GoelAnshul24)
