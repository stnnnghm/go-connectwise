# go-connectwise

Hands-On Test
Data Transformation

1. Populate a string with the following input data (in this exact multi-line format):

(Name)John Doe
(Age)20
(City)Ashtabula, OH
(Flags)NYN

(Name)Jane Doe
(Flags)YNY
(City)N Kingsville, OH

(Name)Sally Jones
(Age)25
(City)Paris
(Flags)YYY

2. Parse the string assuming the following rules:
   a. The string contains a list of person records
   b. Each person record contains the following fields:
   i. Name
   ii. Age (optional)
   iii. City
   iv. Flags
   c. Each line contains a key/value pair for a single field
   i. The key always comes before the value
   ii. The key always begins with an opening parenthesis and always ends with a closing parenthesis
   d. Person records are separated by one or more blank lines
   e. The City line may optionally specify the State (separated by a comma)
   f. The Flags field will always contain exactly three Y or N characters which represent the Boolean values for the following fields in this order:
   i. Is Female
   ii. Is Student
   iii. Is Employee
   g. Invalid or improperly formatted data should be handled gracefully and output with "Invalid data, unable to process"

3. Output the records to the standard output (console) so that they are displayed as follows:

John Doe [20, Male]
City : Ashtabula
State : OH
Student : Yes
Employee : No
Jane Doe [Female]
City : N Kingsville
State : OH
Student : No
Employee : Yes
Sally Jones [25, Female]
City : Paris
State : N/A
Student : Yes
Employee : Yes

4. Unit tests are encouraged
