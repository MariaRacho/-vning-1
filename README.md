def calculate_factorial(n):
    # Check if input is a positive integer
    if not isinstance(n, int) or n < 0:
        raise ValueError("Input must be a non-negative integer.")
    
    # Initialize result to 1
    result = 1
    
    # Calculate factorial using loop
    for i in range(1, n + 1):
        result *= i
    
    return result

# Example usage
number = 6
try:
    print(f"The factorial of {number} is: {calculate_factorial(number)}")
except ValueError as e:
    print(f"Error: {e}")
