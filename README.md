# DES Encryption Visualization

This repository contains a detailed, step-by-step visualization of the **Data Encryption Standard (DES)** encryption algorithm. The visualization is interactive and helps users understand each stage of the DES encryption process, from the initial permutation to the final ciphertext.

## Live Demo

You can view the live demo of the visualization here:

[DES Encryption Visualization](https://66e55e39888fbf0008f48101--des-visualization.netlify.app/)

## Table of Contents

- [Introduction](#introduction)
- [Features](#features)
- [How It Works](#how-it-works)
  - [User Interface](#user-interface)
  - [Visualization Steps](#visualization-steps)
- [Technologies Used](#technologies-used)
- [Usage](#usage)
- [License](#license)
- [Acknowledgments](#acknowledgments)

## Introduction

The Data Encryption Standard (DES) is a symmetric-key algorithm for the encryption of electronic data. Understanding DES can be complex due to its multiple stages of permutations, substitutions, and transformations. This project provides an interactive visualization to demystify the DES encryption process.

## Features

- **Interactive Visualization**: Step through each stage of the DES algorithm by pressing the "Enter" key.
- **Detailed Explanations**: At each step, detailed explanations and intermediate results are displayed.
- **Permutation Tables**: View the permutation tables used at various stages, such as the Initial Permutation and S-box substitutions.
- **Binary and Hexadecimal Representations**: See the data represented in both binary and hexadecimal formats.
- **Mermaid.js Diagrams**: Visual diagrams illustrate the flow of data through the encryption process.

## How It Works

### User Interface

- **Diagram Container**: Displays a flowchart of the DES encryption steps, highlighting the current step.
- **Explanation Box**: Provides detailed explanations, intermediate results, and tables relevant to the current step.
- **Interaction**: Users can progress through the steps by pressing the "Enter" key.

### Visualization Steps

The visualization covers the following steps of the DES encryption process:

1. **Original Plaintext**: Displays the initial plaintext in hexadecimal and binary formats.
2. **Initial Permutation (IP)**: Shows how the plaintext bits are rearranged.
3. **Split into L0 and R0**: Splits the permuted plaintext into two halves.
4. **Original Key**: Presents the encryption key in hexadecimal and binary formats.
5. **Parity Drop (PC-1)**: Reduces the key from 64 to 56 bits by discarding parity bits.
6. **Split into C0 and D0**: Splits the permuted key into two halves.
7. **Key Schedule Generation**: Generates 16 round keys through left shifts and PC-2 permutations.
8. **Feistel Rounds**: Details each of the 16 rounds, including expansion, key mixing, S-box substitutions, and permutations.
9. **Swap Halves**: Swaps the left and right halves after the 16th round.
10. **Inverse Initial Permutation (IP⁻¹)**: Applies the final permutation to obtain the ciphertext.
11. **Final Ciphertext**: Presents the encrypted message in binary and hexadecimal formats.

At each step, the visualization provides:

- **Binary Data**: Shows the current binary data being processed.
- **Permutation Tables**: Displays the permutation tables used and how bits are rearranged.
- **Intermediate Values**: Shows the values of L and R halves, round keys, and results of the Feistel function.
- **S-box Details**: Provides inputs, outputs, and selection processes for S-box substitutions.

## Technologies Used

- **HTML/CSS**: For structuring and styling the web page.
- **JavaScript**: For implementing the DES algorithm and handling user interactions.
- **Mermaid.js**: For generating the flowchart diagrams.
- **Netlify**: For hosting the live demo of the visualization.

## Usage

To use the visualization:

1. **Access the Live Demo**: Visit the [DES Encryption Visualization](https://66e55e39888fbf0008f48101--des-visualization.netlify.app/) page.

2. **Interact with the Visualization**:

   - **Start**: The visualization begins with the initial plaintext and key displayed.
   - **Progress**: Press the **"Enter"** key to move to the next step.
   - **Review**: Read the explanations and examine the diagrams and tables provided at each step.
   - **Repeat**: Once the final ciphertext is displayed, pressing "Enter" again will reset the visualization to the beginning.

3. **Understanding Each Step**:

   - **Diagrams**: The flowchart highlights the current step in the encryption process.
   - **Explanation Box**: Contains detailed information, including intermediate results and computations.
   - **Tables**: Permutation and substitution tables are displayed to show how data is transformed.

## License

This project is licensed under the MIT License.

## Acknowledgments

- **Mermaid.js**: For providing the diagram generation capabilities.
- **Netlify**: For hosting the live demo.
- **Community Resources**: Thanks to all the tutorials and resources that helped in understanding and implementing the DES algorithm.
