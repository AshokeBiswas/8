Q1. Is there any difference in the data type of variables list_ and array_list? If there is then write a code to print the data types of both the variables.
Yes, there is a difference in the data type of list_ and array_list. list_ is a Python list, whereas array_list is a NumPy array.

python
Copy code
import numpy as np

list_ = ['1', '2', '3', '4', '5']
array_list = np.array(object=list_)

print(f"Data type of list_: {type(list_)}")
print(f"Data type of array_list: {type(array_list)}")
Q2. Write a code to print the data type of each and every element of both the variables list_ and array_list.
python
Copy code
import numpy as np

list_ = ['1', '2', '3', '4', '5']
array_list = np.array(object=list_)

print("Data types of elements in list_:")
for elem in list_:
    print(type(elem))

print("\nData types of elements in array_list:")
for elem in array_list:
    print(type(elem))
Q3. Considering the following changes in the variable, array_list:
python
Copy code
array_list = np.array(object=list_, dtype=int)
Will there be any difference in the data type of the elements present in both the variables, list_ and array_list? If so, then print the data types of each and every element present in both the variables, list_ and array_list.

Yes, there will be a difference. list_ will still contain strings, while array_list will contain integers.

python
Copy code
import numpy as np

list_ = ['1', '2', '3', '4', '5']
array_list = np.array(object=list_, dtype=int)

print("Data types of elements in list_:")
for elem in list_:
    print(type(elem))

print("\nData types of elements in array_list:")
for elem in array_list:
    print(type(elem))
Q4. Write a code to find the following characteristics of variable, num_array:
(i) shape
(ii) size

python
Copy code
import numpy as np

num_list = [[1, 2, 3], [4, 5, 6]]
num_array = np.array(object=num_list)

print(f"Shape of num_array: {num_array.shape}")
print(f"Size of num_array: {num_array.size}")
Q5. Write a code to create numpy array of 3x3 matrix containing zeros only, using a numpy array creation function.
python
Copy code
import numpy as np

zero_matrix = np.zeros((3, 3))
print(zero_matrix)
Q6. Create an identity matrix of shape (5,5) using numpy functions.
python
Copy code
import numpy as np

identity_matrix = np.eye(5)
print(identity_matrix)
