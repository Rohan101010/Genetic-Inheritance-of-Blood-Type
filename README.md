Genetic Inheritance of Blood Type
This program simulates the genetic inheritance of blood type across multiple generations. It creates a family tree where each person has two parents and two alleles that determine their blood type, using a linked list data structure to represent the family relationships.
How it Works
The program uses a person struct to represent each individual in the family tree. The struct has two pointers to the person's parents, and two char values to represent the person's alleles.
The create_family() function recursively creates a new person by:

Allocating memory for the new person
If there are still generations left to create, recursively creating the person's two parents and assigning them as the new person's parents
Randomly assigning the new person's alleles based on the alleles of their parents
If there are no more generations left, randomly assigning the new person's alleles

To represent the family tree, the program uses a linked list data structure. Each person struct has two pointers to its parents, forming a doubly-linked list. This allows the print_family() function to traverse the family tree and print out each person's generation, blood type, and their parents.
The free_family() function recursively frees the memory allocated for the family tree by traversing the linked list and freeing each person struct.
The random_allele() function randomly selects one of the three possible blood type alleles: 'A', 'B', or 'O'.
How to Use

Compile the program using a C compiler, e.g., gcc -o inheritance inheritance.c.
Run the program, and it will output a family tree of blood types for 3 generations.

Example Output
CopyChild (Generation 0): blood type AO
  Parent (Generation 1): blood type AB
    Grandparent (Generation 2): blood type AO
    Grandparent (Generation 2): blood type BO
  Parent (Generation 1): blood type OO
    Grandparent (Generation 2): blood type AO
    Grandparent (Generation 2): blood type BB
Skills Developed
By working on this project, you'll have the opportunity to develop the following skills:

Data Structures: Understanding how to use structs and linked lists to represent complex data models, such as the person struct with its parent pointers and the family tree.
Recursive Programming: Implementing the create_family() function using recursion to build the family tree.
Memory Management: Properly allocating and freeing memory for the person structs using malloc() and free().
Random Number Generation: Using the rand() function to randomly assign blood type alleles.
Procedural Programming: Organizing the program's logic into separate functions for creating, printing, and freeing the family tree.
Debugging and Problem-Solving: Identifying and fixing any issues that arise during the development process.
Documentation and Readability: Writing a clear and concise README file to explain the project's functionality and usage.

Future Improvements

Add support for the Rh factor (positive or negative) in addition to the ABO blood type.
Allow the user to specify the number of generations to simulate.
Provide options to visualize the family tree in a more graphical format.

Contributing
If you find any issues or have suggestions for improvements, feel free to open a new issue or submit a pull request on the GitHub repository.
