import sys

def is_prime(n):
    if n <= 1:
        return False
    if n <= 3:
        return True
    if n % 2 == 0 or n % 3 == 0:
        return False
    i = 5
    while i * i <= n:
        if n % i == 0 or n % (i + 2) == 0:
            return False
        i += 6
    return True

def main():
    if len(sys.argv) != 2:
        print("Usage: rsa <file>")
        sys.exit(1)

    input_file = sys.argv[1]

    with open(input_file, 'r') as file:
        numbers = file.read().splitlines()

    for number in numbers:
        n = int(number)
        for i in range(2, n):
            if n % i == 0 and is_prime(i) and is_prime(n // i):
                print(f"{n}={i}*{n//i}")
                break

if __name__ == "__main__":
    main()
