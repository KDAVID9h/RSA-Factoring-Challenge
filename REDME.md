# RSA Factoring Challenge

This project contains scripts to factorize numbers into their prime factors, as well as to solve the RSA Factoring Challenge.

## Prerequisites

- Python 3.x

## Installation

No installation is required. Simply clone the repository to your local machine.

```bash
git clone https://github.com/KDAVID9h/RSA-Factoring-Challenge.git
```

## Usage

### Factorization Script

To factorize numbers into a product of two smaller numbers:

```bash
./factors.py < file >
```

- `<file>` should contain natural numbers to factor, with one number per line.

### RSA Factoring Script

To solve the RSA Factoring Challenge:

```bash
./rsa.py < file >
```

- `<file>` should contain one RSA number per line.

## Examples

### Factorization Script

```bash
./factors.py tests/test00
```

### RSA Factoring Script

```bash
./rsa.py tests/rsa-1
```

## Time Complexity

The factorization script has a time complexity of O(sqrt(n)), where n is the input number.

The RSA factoring script iterates through numbers to find the prime factors, which can have varying time complexities depending on the size of the input.

## Contributing

Contributions are welcome! Feel free to open a pull request or report any issues.
