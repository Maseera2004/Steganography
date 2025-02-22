# Image Encryption and Decryption Using LSB Technique

This program allows you to encrypt a secret message into an image and later decrypt it using a passcode. The encryption is done using the Least Significant Bit (LSB) technique, where the secret message's characters are hidden in the pixel data of the image.

## Features:
- **Encryption**: Embed a secret message into an image.
- **Decryption**: Extract the secret message from the image using a passcode.
- **Passcode Protection**: The encryption and decryption are secured by a passcode to prevent unauthorized access.

## Requirements:
- Python 3.x
- OpenCV library (`cv2`)

You can install OpenCV using pip if you don't have it:

## Usage:

1. **Encryption:**
   - Choose the "Encrypt" option.
   - Provide an image file (preferably in PNG format for lossless compression).
   - Enter the secret message you want to hide inside the image.
   - Enter a passcode to secure the encryption.

2. **Decryption:**
   - Choose the "Decrypt" option.
   - Provide the encrypted image file.
   - Enter the passcode to unlock and decrypt the secret message.

## Example Workflow:

### Encryption:
1. Run the script and select the encryption option.
2. Provide the image file, secret message, and passcode.
3. The encrypted image will be saved as `encrypted_image.png`.

### Decryption:
1. Run the script and select the decryption option.
2. Provide the encrypted image file.
3. Enter the correct passcode.
4. The secret message will be displayed after successful decryption.

## Notes:
- The message is encoded in the first few pixels of the image (LSB method).
- The first 3 pixels store the length of the message.
- The program allows you to keep the passcode in a file for later use.

## Example:
1. **Encrypt Image**:
   - Choose image: `mypic.png`
   - Secret message: "This is a secret message"
   - Passcode: "mysecretpass"

2. **Decrypt Image**:
   - Choose encrypted image: `encrypted_image.png`
   - Passcode: "mysecretpass"

After entering the correct passcode, the message "This is a secret message" will be displayed.


