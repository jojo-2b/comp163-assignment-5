# comp163-assignment-5
#test case 1
print(" === Challenge 1: Collatz Conjecture === ") # will print without being in output

current_number = int(input("Enter starting number: "))
step_count = 0

print("Sequence:", end=" ")
print(current_number, end=" ")

while current_number != 1:
    if current_number % 2 == 0:
        current_number = current_number // 2
    else: 
        current_number = current_number * 3 + 1  

    print(current_number, end=" ")      
    step_count += 1 

print("\nSteps:", step_count)    
print(" ")# to satisfy test case

print("=== Challenge 2: Prime Number Checker ===")

pri = int(input("Enter a number: "))

if pri <= 1:
    print(f"Enter an integer.")
else:
    print(f"Testing divisors from 2 to {pri-1}...")
    divisor = None

    for d in range(2, pri):
        if pri % d == 0:
            divisor_found = d
            break    
    if divisor is None:
        print(f"{pri} is prime!")
    else:
        print(f"{pri} is not prime (divisible by {divisor}")  
        
        print(" ")

print(" === Challenge 3: Multiplication Table === ")
        
     print("  ", end="") #header
        for col in range(1, 11):
            print(f" {col:4} ", end="")
            print()

        for row in range(1, 11):
            print(f"{row:2} ", end="")  
            for col in range(1, 11):
                product = row * col #will give necessary products that are needed
                print(f"{product:4}", end="")
            print()
