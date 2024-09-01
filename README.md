# Cipher Decryption using NLP

## Overview

This project is focused on decrypting an encrypted text file containing the novel "Moby-Dick" by Herman Melville. The primary objective is to apply various decryption techniques to analyze and decode the text. The decryption process is implemented in Python within a Jupyter Notebook. The project provides an educational exploration of cryptography concepts such as Caesar Cipher, Vigenère Cipher, and Frequency Analysis.

The goal is to demonstrate the decryption process using different cipher methods, and to verify the correctness of these methods against a well-known text dataset. This project can serve as a learning tool for those interested in cryptography and text analysis.

## Project Structure

The repository contains the following files:

- **`Cipher_Decryption.ipynb`**: A Jupyter Notebook containing the Python code for decrypting the text using various ciphers. This notebook also includes explanations of each cipher and step-by-step implementation details.
- **`moby_dick.txt`**: A plain text file containing the complete text of "Moby-Dick". This file is used as both the source of encrypted data and the dataset for testing decryption algorithms.

## Installation

To get started with the project on your local machine, follow the instructions below.

### Prerequisites

Ensure you have Python 3.x installed on your system. You can download it from the official [Python website](https://www.python.org/).

Additionally, you'll need to install Jupyter Notebook to run the `.ipynb` file. You can install Jupyter Notebook along with other dependencies using `pip`.

### Setup Instructions

1. **Clone the repository:**
   ```bash
   git clone https://github.com/yourusername/cipher-decryption.git
   cd cipher-decryption
   ```

2. **Create and activate a virtual environment (optional but recommended):**
   Creating a virtual environment helps to manage project dependencies separately.
   ```bash
   python3 -m venv venv
   source venv/bin/activate  # On Windows, use `venv\Scripts\activate`
   ```

3. **Install dependencies:**
   Install the required Python libraries using the following command:
   ```bash
   pip install -r requirements.txt
   ```
   If a `requirements.txt` file is not included, install the basic dependencies manually:
   ```bash
   pip install jupyter numpy pandas matplotlib
   ```

4. **Launch Jupyter Notebook:**
   After installation, you can open the Jupyter Notebook by running:
   ```bash
   jupyter notebook Cipher_Decryption.ipynb
   ```

   This will open the notebook in your web browser, where you can explore and run the code cells.

## Project Details

### Decryption Algorithms Implemented

The notebook includes implementations of the following cipher techniques:

1. **Caesar Cipher:**
   - A basic encryption technique where each letter in the plaintext is shifted by a certain number of positions in the alphabet.
   - The decryption function reverses the process by shifting the letters in the opposite direction.

   Example usage:
   ```python
   def caesar_decrypt(ciphertext, shift):
       # Decrypts Caesar Cipher with a given shift
       # Your implementation code
       return plaintext
   ```

2. **Vigenère Cipher:**
   - A method of encrypting text by using a keyword where each letter in the text is shifted based on the corresponding letter in the keyword.
   - The decryption function involves reversing this process by applying the inverse shifts.

   Example usage:
   ```python
   def vigenere_decrypt(ciphertext, keyword):
       # Decrypts Vigenère Cipher using the provided keyword
       # Your implementation code
       return plaintext
   ```

3. **Frequency Analysis:**
   - A technique used to analyze the frequency of letters in the ciphertext and compare it to known frequency distributions of letters in a given language (e.g., English).
   - This method is particularly useful for breaking substitution ciphers.

   Example usage:
   ```python
   def frequency_analysis_decrypt(ciphertext):
       # Decrypts using frequency analysis
       # Your implementation code
       return plaintext
   ```

### Additional Analysis

- **Word Frequency Analysis:**
  - Identifies common words or phrases in the encrypted text and compares them to known word patterns in English.
  
- **Brute Force Approach:**
  - For simple ciphers like Caesar Cipher, a brute force approach is used to try all possible shifts and select the one that produces readable text.

## Example Usage

Here is an example of decrypting text using the Caesar Cipher with a known shift:

```python
ciphertext = "Uifsf jt b tfdsfu dpnfupo."  # "There is a secret comment."
shift = 1
plaintext = caesar_decrypt(ciphertext, shift)
print(plaintext)
```

Output:
```
There is a secret comment.
```

## Dataset

The dataset used for testing and evaluation is the text of "Moby-Dick" by Herman Melville. This text is large and contains a diverse range of vocabulary, making it suitable for evaluating the accuracy of decryption methods.

- **`moby_dick.txt`**: Contains the full text of "Moby-Dick" and is used to verify the performance of different decryption techniques.

### How the Dataset is Used:

- **Text Decryption:** The text is encrypted using various ciphers, and the decryption algorithms are tested to ensure they can recover the original text.
- **Frequency Analysis:** The frequency of letters in "Moby-Dick" is analyzed and compared with standard English frequency distributions.

## Results and Discussion

The notebook includes visualizations and analysis of the results. For example, after applying the Caesar Cipher decryption, the notebook compares the decrypted text with the original to calculate accuracy.

- **Accuracy Metrics:** The decryption accuracy is measured based on the number of correctly decrypted characters or words.
- **Visualization:** Graphs and plots (e.g., letter frequency histograms) are provided to help understand the decryption process.

## Contributing

Contributions to improve this project are welcome! Here's how you can contribute:

1. **Fork the repository** on GitHub.
2. **Create a new branch** for your feature or bug fix:
   ```bash
   git checkout -b feature-name
   ```
3. **Commit your changes** with a descriptive commit message:
   ```bash
   git commit -m "Add feature to improve decryption accuracy"
   ```
4. **Push to the branch**:
   ```bash
   git push origin feature-name
   ```
5. **Submit a pull request** on GitHub, describing your changes.

### Suggestions for Contributions:

- Implement additional ciphers (e.g., RSA, Hill Cipher).
- Optimize existing algorithms for performance.
- Add more test cases for the decryption methods.
- Improve visualization and analysis of results.

## Acknowledgments

- **Herman Melville**: For the original text of "Moby-Dick" used in this project.
- **Python Community**: For providing the tools and libraries used in this project.
- **Open-source contributors**: For inspiring the methods and ideas implemented in this project.
