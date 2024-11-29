# Python_Day5

#Activity: Calculate and Display Fibonacci Numbers
def fibonacci(limit):
    fib_sequence = [0, 1]
    while len(fib_sequence) < limit:
        next_value = fib_sequence[-1] + fib_sequence[-2]
        fib_sequence.append(next_value)
    return fib_sequence

# User input for the limit
limit = int(input("Enter the number of Fibonacci numbers to generate: "))

# Calculate and display the Fibonacci sequence
fib_sequence = fibonacci(limit)
print("Fibonacci sequence:")
for num in fib_sequence:
    print(num)


#Project: Simulate Signal Modulation Cycles
def signal_modulation(cycles):
    for cycle in range(1, cycles + 1):
        if cycle % 2 == 0:
            print(f"Cycle {cycle}: Low")
        else:
            print(f"Cycle {cycle}: High")

# User input for the number of cycles
cycles = int(input("Enter the number of signal modulation cycles: "))

# Simulate signal modulation
signal_modulation(cycles)
