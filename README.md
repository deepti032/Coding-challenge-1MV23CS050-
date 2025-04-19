# Coding-challenge-1MV23CS050-
1.FIBONACCI SERIES
program:
def print_fibonacci(n):
    a, b = 0, 1
    result = []
    for _ in range(n):
        result.append(str(a))
        a, b = b, a + b
    print(" ".join(result))

n = int(input("Enter a number: "))
print_fibonacci(n)

2.PRIME NUMBERS TILL N
program:
def is_prime(num):
    if num < 2:
        return False
    for i in range(2, int(num**0.5) + 1):
        if num % i == 0:
            return False
    return True

def print_primes_up_to(n):
    primes = [str(i) for i in range(2, n + 1) if is_prime(i)]
    print(" ".join(primes))


n = int(input("Enter a number: "))
print_primes_up_to(n)


3.VOWEL AND CONSONANT COUNTER
program:
def count_vowels_and_consonants(s):
    vowels = 'aeiou'
    s = s.lower()
    vowel_count = 0
    consonant_count = 0

   for char in s:
        if char.isalpha():
            if char in vowels:
                vowel_count += 1
            else:
                consonant_count += 1

  print(vowel_count, consonant_count)


input_string = input("Enter a string: ")
count_vowels_and_consonants(input_string)

4.CENTRE ALIGNED STAR TRIANGLE
program:
def print_triangle(n):
  for i in range(1, n + 1):
     
  for j in range(n - i):
            print(" ", end="")
        
  for k in range(2 * i - 1):
            print("*", end="")
       
  print()


n = int(input("Enter number of rows: "))
print_triangle(n)
