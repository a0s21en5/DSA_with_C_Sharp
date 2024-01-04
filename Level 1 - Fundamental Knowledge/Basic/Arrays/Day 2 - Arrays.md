# Arrays

- An array is a collection of elements of a single data type stored in adjacent memory locations.

- An array is a collection of related alues placed in contiguous memory locations and these values are referenced using common array name.

- Simplifies the task of maintaining these values.

- An array always stores values of single data type.

- Each values is referres to as an element.

- These elements are accessed using `subscripts` or `index number` that determine the position of the element in the array list.

- C# supports zero-based index values in an array.

- Arrays are reference type variables.

- An array declaration specifies the type of data that it can hold and an identifier.

- declaring an array does not allocate memory to the array.



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


## Array Declaration and Initialization

Example: Array Declaration

```
int[] evenNums;  // integer array

string[] cities; // string array
```


Example: Array Declaration & Initialization
```
int[] evenNums = new int[5]{ 2, 4, 6, 8, 10 }; 

string[] cities = new string[3]{ "Mumbai", "London", "New York" };
```


Example: Array Declaration using var
```
var evenNums = new int[]{ 2, 4, 6, 8, 10}; 

var cities = new string[]{ "Mumbai", "London", "New York" };
```


Example: Short Syntax of Array Declaration
```
int[] evenNums = { 2, 4, 6, 8, 10}; 

string[] cities = { "Mumbai", "London", "New York" }
```


Example: Invalid Array Creation
```
//must specify the size 
int[] evenNums = new int[]; 

//number of elements must be equal to the specified size 
int[] evenNums = new int[5] { 2, 4 };

//cannot use var with array initializer
var evenNums = { 2, 4, 6, 8, 10}; 
```


Late Initialization
```
int[] evenNums;

evenNums = new int[5];
// or
evenNums = new int[]{ 2, 4, 6, 8, 10 };
```


Example: Access Array Elements using Indexes
```
int[] evenNums = new int[5];
evenNums[0] = 2;
evenNums[1] = 4;
//evenNums[6] = 12;  //Throws run-time exception IndexOutOfRange

Console.WriteLine(evenNums[0]);  //prints 2
Console.WriteLine(evenNums[1]);  //prints 4
```


Example: Access Array Elements using Indexes
```
int[] evenNums = { 2, 4, 6, 8, 10 };

for(int i = 0; i < evenNums.Length; i++)
            Console.WriteLine(evenNums[i]);  

for(int i = 0; i < evenNums.Length; i++)
    evenNums[i] = evenNums[i] + 10;  // update the value of each element by 10
```


Example: Accessing Array using foreach Loop
```
nt[] evenNums = { 2, 4, 6, 8, 10}; 
string[] cities = { "Mumbai", "London", "New York" }; 

foreach(var item in evenNums)
            Console.WriteLine(item);   

foreach(var city in cities)
            Console.WriteLine(city);  
```


Example: Array Methods
```
int[] nums = new int[5]{ 10, 15, 16, 8, 6 };

Array.Sort(nums); // sorts array 
Array.Reverse(nums); // sorts array in descending order
Array.ForEach(nums, n => Console.WriteLine(n)); // iterates array
Array.BinarySearch(nums, 5);// binary search 
```