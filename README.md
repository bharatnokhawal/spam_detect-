# Phishing Detection Project

This project aims to detect potential phishing attempts within a dataset containing text data, such as emails or messages. It analyzes each data entry for indications of phishing attempts, including sensitive requests, urgent prompts, and solicitations.

## Dataset

The dataset used for this project is stored in a CSV file named `dataset.csv`. Each row in the CSV file represents a data entry, with two columns:

- `v1`: Contains labels indicating whether a message is "ham" (not spam) or "spam".
- `v2`: Contains the text of the message.

## Analysis

The Python script `phishing_detection.py` performs the following analysis on the dataset:

1. Iterates over each data entry and extracts the text of the message.
2. Analyzes the text for indications of phishing attempts, including:
   - Sensitive requests (e.g., requests for passwords, account information).
   - Urgent prompts (e.g., urgent action required, limited-time offers).
   - Solicitations (e.g., offers for free prizes, claims).
3. Determines if the message is suspicious based on the presence of any of these characteristics.
4. Prints the result for each data entry, indicating whether it contains indications of phishing attempts.

## Usage

To use this project:

1. Clone the repository to your local machine.
2. Ensure you have Python installed.
3. Install the required libraries using pip: `pip install pandas scikit-learn`.
4. Replace the `dataset.csv` file with your own dataset containing text data.
5. Run the Python script `phishing_detection.py`.

```bash
python phishing_detection.py
