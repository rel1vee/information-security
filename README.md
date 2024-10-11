# Information Security Tools

This repository contains a collection of Python scripts for various information security tasks, including encryption, steganography, and a combination of both. These tools provide a user-friendly graphical interface for performing cryptographic operations and hiding/extracting messages in images.

## Features

1. **AES Encryption/Decryption (kriptografi.ipynb)**
   - Encrypt and decrypt text using AES encryption
   - User-friendly GUI for easy operation
   - 16-character key input for AES-128 encryption

2. **LSB Steganography (steganografi.ipynb)**
   - Hide messages in images using the Least Significant Bit (LSB) technique
   - Extract hidden messages from steganographic images
   - Support for PNG, JPG, and BMP image formats

3. **Combined AES Encryption and LSB Steganography (kombinasi-kripto-stegano.ipynb)**
   - Encrypt messages using AES before hiding them in images
   - Extract and decrypt hidden messages from images
   - Combines the security of encryption with the secrecy of steganography

## Requirements

- Python 3.x
- PyQt5
- Pillow (PIL)
- NumPy
- PyCryptodome

## Installation

1. Clone this repository:
   ```
   git clone https://github.com/rel1vee/information-security.git
   cd information-security
   ```

2. Install the required packages:
   ```
   pip install PyQt5 Pillow numpy pycryptodome
   ```

## Usage

### AES Encryption/Decryption

1. Run the script:
   ```
   python kriptografi.ipynb
   ```
2. Enter the text you want to encrypt/decrypt in the input field.
3. Enter a 16-character key in the key field.
4. Click "Encrypt" to encrypt the text or "Decrypt" to decrypt the text.
5. The result will appear in the output field.

### LSB Steganography

1. Run the script:
   ```
   python steganografi.ipynb
   ```
2. Click "Select Image" to choose an image file.
3. Enter the message you want to hide in the message field.
4. Click "Hide Message" to embed the message in the image.
5. To extract a message, select a steganographic image and click "Extract Message".

### Combined AES Encryption and LSB Steganography

1. Run the script:
   ```
   python kombinasi-kripto-stegano.ipynb
   ```
2. Click "Select Image" to choose an image file.
3. Enter the message you want to hide and encrypt in the message field.
4. Enter a 16-character key for AES encryption.
5. Click "Encrypt and Hide Message" to process and embed the message.
6. To extract and decrypt a message, select a steganographic image, enter the correct key, and click "Extract and Decrypt Message".

## Security Considerations

- Always use strong, unique keys for encryption.
- Remember that steganography alone does not provide strong security; it's best used in combination with encryption.
- Be aware that saving images in lossy formats (like JPEG) may destroy hidden messages.

## Contributing

Contributions to improve these tools are welcome. Please feel free to submit pull requests or open issues to discuss potential enhancements.

