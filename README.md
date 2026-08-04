# Password Manager Exporter

**Project made out of boredom :D** 

---

## Introduction

Password Manager Exporter is a client-side web application designed to simplify the process of exporting and migrating data from major password managers. The tool operates entirely locally, ensuring maximum confidentiality of sensitive information.

The project was born from the need to have a single standardized interface to manage the multiple export formats used by different password management services.

---

## Product Overview

Password Manager Exporter allows you to:

- Import JSON files from over 25 different password managers
- Automatically decode data structure, recognizing the source format
- Organize credentials into a hierarchical structure based on original folders
- Export data in four standardized formats (TXT, CSV, HTML, JSON)
- Download a ZIP archive containing all organized files

---

## Core Features

### Data Import
- Support for JSON from all major password managers
- Automatic source format detection
- Encrypted file handling with master password
- Drag & drop anywhere on the page
- Data validation and parsing

### Data Processing
- Automatic field extraction: service name, username, password, URL, notes
- Preservation of original folder structure
- Asynchronous processing with progress bar
- Large dataset handling

### Data Export
- **TXT**: Readable format with standardized structure
- **CSV**: Compatible with Excel, Google Sheets, and data analysis software
- **HTML**: Navigable tabular display
- **JSON**: Preserves original structure for future imports
- ZIP compression with preserved folder structure

---

## Supported Password Managers

| Service | Supported Formats |
|---------|-------------------|
| Bitwarden | JSON, Encrypted JSON |
| 1Password | 1PUX, 1pif, OPVault |
| Dashlane | JSON, DASH |
| LastPass | JSON |
| KeePass / KeePassXC | KDBX, XML, JSON |
| NordPass | JSON |
| RoboForm | RFO, JSON |
| Enpass | JSON |
| Keeper Security | JSON |
| Password Safe | XML, JSON |
| Sticky Password | JSON |
| Norton Password Manager | JSON |
| Google Password Manager | JSON |
| Apple Passwords | JSON |
| Microsoft Edge | JSON |
| Chrome | JSON |
| Firefox | JSON |
| Samsung Pass | JSON |
| LogMeOnce | JSON |
| mSecure | JSON |
| Proton Pass | JSON, Encrypted ZIP |
| Generic | Any structured JSON |

---

## Technical Architecture

### Technology Stack
- **Frontend**: HTML5, CSS3, JavaScript ES6+
- **Compression**: JSZip 3.10.1
- **File Management**: FileSaver.js 2.0.5
- **Model**: Single Page Application (SPA)

### Design Principles
- **Privacy by Design**: Zero data transmitted to external servers
- **Offline First**: Works completely without Internet connection
- **Zero Persistence**: No data saved in localStorage or cookies
- **Memory Only**: Processing exclusively in RAM

### Processing Flow
1. **Acquisition**: JSON file loading via Drag & Drop or manual selection
2. **Detection**: Automatic structure analysis to identify source format
3. **Decoding**: Data parsing with relevant field extraction
4. **Organization**: Folder grouping and hierarchical structuring
5. **Export**: File generation in selected formats
6. **Compression**: ZIP archive creation
7. **Download**: File delivery to the user

---

## Security and Privacy

### Security Guarantees
- **Zero Server**: No communication with external servers
- **Zero Storage**: Data is never written to disk
- **Zero Persistence**: No cookies, localStorage, or cache used
- **Encryption Handling**: Master passwords processed exclusively in memory

### Recommended Best Practices
- Use the application on personal and trusted devices
- Delete exported files after use
- Do not share generated archives with third parties
- Always keep your master password secure

---

## License

**MIT License**

Copyright © 2024 MegaByte

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
