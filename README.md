# IT23603318_IT3040_Assignment1

# Assignment 1 - Transliteration Accuracy Testing

IT3040 – ITPM | BSc (Hons) in Information Technology – Year 3

## Description
This project tests the Chat Sinhala transliteration function of the application at
https://www.pixelssuite.com/chat-translator using Playwright automation.
It inputs chat-style Singlish text and records whether the Sinhala output is correct.

## Prerequisites
- Python 3.13
- Google Chrome browser

## Installation

1. Clone or download this repository and extract to D:\test_automation

2. Open Command Prompt and navigate to the project folder:
cd /d D:\test_automation

3. Install required dependencies:
pip install -U pip
pip install playwright openpyxl
playwright install
python -m playwright install

## How to Run

python test_automation.py --excel "test_automation/Assignment 1 - Test cases.xlsx" --url "https://www.pixelssuite.com/chat-translator" --wait-ms 5000 --type-delay-ms 80 --slow-mo-ms 200 --save-every 1 --keep-open

## What It Does
- Opens the chat translator website in a browser
- Types each Singlish input from the Excel file
- Records the actual Sinhala output into the Actual output column
- Compares it with the Expected output and marks Pass or Fail in the Status column

## Project Structure
test_automation/
├── IT23603318_Test_cases.xlsx
├── IT23603318_test_automation.py
├── IT23603318_Requirements.txt
├── IT23603318_Commands.txt
├── IT23603318_README.md
