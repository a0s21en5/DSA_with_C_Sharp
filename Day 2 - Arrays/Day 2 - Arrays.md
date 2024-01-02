# Arrays

- An array is a collection of elements of a single data type stored in adjacent memory locations.

- An array is a collection of related alues placed in contiguous memory locations and these values are referenced using common array name.

- Simplifies the task of maintaining these values.

- An array always stores values of single data type.

- Each values is referres to as an element.

- These elements are accessed using `subscripts` or `index number` that determine the position of the element in the array list.

- C# supports zero-based index values in an array.

## Array Declaration and Initialization

First Type: Array Declaration and Initialization
```
int[] evenNums = new int[2]; // integer array
evenNums[0] = 5;
evenNums[1] = 15;
```

```
string[] anime_characters = new string[2]; // string array

cities[0] = "Naruto";
cities[1] = "Hinata";
```

Second Type: Array Declaration and Initialization

```
int[] evenNums = new int[] {5, 15}; 

string[] anime_characters = new string[2]{"Hinata","Naruto"}; 
```

Third Type: Array Declaration and Initialization

```
int[] evenNums = {5, 15}; 

string[] anime_characters = {"Hinata","Naruto"}; 
```