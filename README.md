def find_smallest_element(input_list):
  """
  Finds the smallest element in a given list.

  Args:
    input_list: A list of comparable elements (e.g., numbers, strings).

  Returns:
    The smallest element in the list.
    Raises ValueError if the input list is empty.
  """
  if not input_list:
    raise ValueError("The input list cannot be empty.")
  
  smallest_element = min(input_list)
  return smallest_element

# Example usage:
numbers = [4, 8, 1, 9, 3, 5]
smallest = find_smallest_element(numbers)
print(f"The smallest element in {numbers} is: {smallest}")

strings = ["apple", "banana", "cherry", "date"]
smallest_string = find_smallest_element(strings)
print(f"The smallest string in {strings} is: {smallest_string}")

# Example with an empty list
try:
  empty_list = []
  find_smallest_element(empty_list)
except ValueError as e:
  print(e)
