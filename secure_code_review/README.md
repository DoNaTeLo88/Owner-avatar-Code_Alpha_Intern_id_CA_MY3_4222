## 🛡 Overview

This Python script is a wrapper around the static analysis tool **Bandit**, designed to scan Python projects for security issues. It allows the user to input a directory, runs Bandit recursively, prints colored messages in the terminal, and saves results to log files.

---

## 🔍 Features

- Interactive input for selecting the project directory
- Runs `bandit -r <directory>` to recursively scan Python files
- Displays colored output:
  - Purple for start message
  - Green if no issues found
  - Red if vulnerabilities are detected
- Logs results in:
  - `bandit_scan_results.txt` (start times and errors)
  - `review_scan_results.txt` (Bandit findings)

---

## 🧠 How It Works

1. Prompts the user to input a project directory path.
2. Displays the current time as the scan start time.
3. Executes Bandit on the selected directory using `subprocess`.
4. Displays and logs results based on the scan:
   - If no issues found (`returncode == 0`), prints a success message.
   - If issues found (`returncode != 0`), prints and logs detailed results.
5. Catches and logs any runtime exceptions.

---

## 📦 Dependencies

- Python 3.x
- [Bandit](https://github.com/PyCQA/bandit)

## Usage 
python secure_code_review.py

## Sample prompt
Enter the directory path to scan: ./my_project

## Output Files
review_scan_results.txt

## Disclaimer
<p>This script is intended for educational and internal audit purposes</p>
<p>Always ensure you have permission to analyze any codebase before scanning it</p>

## Author
<p>Ahmed Saeed Ahmed Hussein</p>
<p>Cybersecurity Intern @ Code Alpha </p>
<p>Intern ID: CA/MY3/4222</p>
