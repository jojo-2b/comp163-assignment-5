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
