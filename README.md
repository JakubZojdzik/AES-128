# AES-128

This repository contains a C implementation of the Advanced Encryption Standard (AES) algorithm for encrypting and decrypting 128-bit data blocks. Only 1 block encoding and decoding is supported.

## Usage

### Compilation

Compile the code using a C compiler. For example, using `gcc`:

```bash
gcc main.c -o aes
```

or using `clang`:

```bash
clang main.c -o aes
```

### Running the Program

Run the compiled executable:

```bash
./aes
```

The program will demonstrate the AES-128 encryption and decryption process using a sample plaintext and key.

## Code Structure

The main functionalities of the AES algorithm are implemented in the following functions:

- `expandKey`: Expands the input key to generate round keys.
- `addRoundKey`: Performs the AddRoundKey operation in the AES algorithm.
- `subBytes`: Substitutes each byte of the state with a corresponding byte from the S-box.
- `shiftRows`: Performs the ShiftRows operation in the AES algorithm.
- `mixColumns`: Performs the MixColumns operation in the AES algorithm.
- `subBytesInv`, `shiftRowsInv`, and `mixColumnsInv`: Inverse operations for decryption.
- `encrypt`: Encrypts a 128-bit plaintext using AES-128.
- `decrypt`: Decrypts a 128-bit ciphertext using AES-128.

## Example

The `main` function in demonstrates how to use the encryption and decryption functions with a sample plaintext and key. Feel free to modify the input data for your use case.

## TODO

Multiple blocks operations with different modes