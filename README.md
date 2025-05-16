# CODM Checker

![CODM Checker Banner](https://i.imgur.com/SDlnfyp.jpeg)

A tool for checking valid Garena accounts that are bound to Call of Duty Mobile (CODM) using user-provided combolists.

## Table of Contents
- [Overview](#overview)
- [Installation](#installation)
- [Usage](#usage)
- [Key Features](#key-features)
- [Components](#components)
- [Troubleshooting](#troubleshooting)
- [Disclaimer](#disclaimer)

## Overview

CODM Checker allows you to validate Garena accounts associated with Call of Duty Mobile. It processes user combolists (username:password combinations) to determine which accounts are valid and bound to CODM.

## Installation

### Prerequisites
- Python 3.x
- Git (for cloning the repository)

### Clone the Repository
```bash
cd storage
cd downloads
git clone https://github.com/sintxcs/checker.git
```

### Install Required Modules
```bash
cd checker
pip install -r requirements.txt
```

## Usage

1. Move your combolist text files to the checker folder
2. Run the checker script:
```bash
cd checker
python checker.sin
```

## Key Features

- **Full Capture Details**: Comprehensive information about validated accounts
- **Sorted Results**: Organized output for easier analysis
- **Clean Check Summary**: Clear overview of checking process results
- **Duplicate Separator**: Automatically identifies and separates duplicate entries
- **Garena Account Separator**: Separates Garena accounts that aren't bound to CODM
- **Anti-Rate Limiting**: 
  - Auto-pauses when Captcha (403) is detected for IP changing
  - Automatically retries after Rate Limit (429) in Garena API
- **Cookie Management**: Auto-saving and rotating cookies for persistent sessions
- **URL Cleaner**: Automatic URL remover for cleaner data processing

## Components

### Core Files

#### checker.sin
The main Python script that performs the account validation process. It processes the combolist files, interacts with the Garena API, and outputs the results.

#### requirements.txt
Contains a list of all Python modules required by the tool:
```
requests
colorama
tqdm
... (and other dependencies)
```

### API Components

#### Credits.js
An API endpoint handler that generates authentication keys for users to access the checker.sin script. This serves as an access control mechanism for the tool.

#### Server.js
A server-side API that:
- Receives data from checker.sin via POST requests
- Extracts valid account information from the provided text files
- Processes and returns validation results

### Output Files

The checker will generate several output files for different types of results:

- **valid.txt**: Contains all valid Garena accounts bound to CODM
- **invalid.txt**: Contains all invalid credentials
- **notbound.txt**: Contains valid Garena accounts not bound to CODM
- **duplicates.txt**: Contains duplicate entries from the combolist

## Troubleshooting

### Missing Modules
If you encounter module import errors, run:
```bash
pip install -r requirements.txt
```

### API Connection Issues
- Ensure you have a stable internet connection
- Check if your IP has been rate-limited (429 error)
- Verify that the authentication keys are valid

## Disclaimer

> [!WARNING]  
> *This tool is for educational purposes only. The creator won't take any responsibility if any users take advantage of this and exploit it for illicit activities.*

Using this tool to gain unauthorized access to accounts or for any malicious purpose is strictly prohibited and may violate applicable laws and regulations.
