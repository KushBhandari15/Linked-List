# Linked-List
Explore creating and using an ordered linked list

Objective:

The objective of this Lab is to explore creating and using an ordered linked list.

Task 1: Create an ordered linked list class.
1. Create a new project. You can name this whatever you like.
2. Design and implement an ordered linked list class as described in class. This class should
be a template. The template is expected to have overloaded the >, < and == operators.
  a. The class should have the following methods fully implemented.
    i. Constructor
    ii. AddItem – adds an item from the list
    iii. GetItem – searches the list for the given item. If found, it removes it from
    the list and returns it. If not found, it returns a null pointer.
    iv. IsInlist – returns a bool indicating if the given item is in the list.
    v. IsEmpty – returns a bool indicating if the list is empty.
    vi. Size – returns an int indicating the number of items in the list.
    vii. SeeNext – returns the item without removing it from the list at a given
    location in the list. The class will maintain the next location and will start
    at the first item in the list. When it gets to the last item in the list, it will
    return a null pointer after it gets past the last item. If the list is empty,
    this will throw an error or display an error message. 2 calls to SeeNext
    will return the 2 items next to each other in the list unless SeeAt or Reset
    is called in between the 2 calls (or the first call returns the last item in the
    list).
    viii. SeeAt – Finds an item at a location in the list (int passed in from user),
    and returns the item without removing it. If the location passed by the
    user is past the end of the list, this will throw an error or display an error
    message. This will set the location used by SeeNext to point at the item
    after the item returned.
    ix. Reset – resets the location that the SeeNext function uses to point at the
    first item in the list.
    x. Destructor
  b. All items passed to or from the class should be done so via a pointer rather than
  by value.
  c. Make sure you don’t have any memory leaks.

Complete this before moving on to task 2.

Task 2: Create a class to be used as the item stored in the list. This class will be a student. It
should have the following members at a minimum.
1. Priavte:
  a. FirstName
  b. LastName
  c. MNumber – This should store the M as well as any leading zeros.
  d. GPA
  e. Birthday
2. Public:
  a. Constructor – This accepts parameters for FirstName, LastName, MNumber and
  Birthday. It has an optional parameter for GPA which if missing is set to 0.0.
  b. GetName – this returns a string containing both FirstName concatenated with
  LastName
  c. GetMNumber
  d. GetAge – returns the age in years of the student.
  e. Overloads of the >, < and == operators that compare the MNumber member of
  two student instances.

Complete this before moving on to task 3.

Task 3: Create a test program that has a menu allowing you to test each of the functions in
your linked last class (Task 1).

1. This should present the user with a choice of public member functions of your linked list
class and ask which the user would like to try.
2. When the user selects a member function, the program will prompt the user for any
required information. For example, the GetItem function only requires an MNumber as
that is what is being compared but the AddItem requires the user to enter a FirstName,
LastName, MNumber, Birthday and optionally a GPA.
3. Test your program. Include a screen shot of some of this testing in your lab report.

Complete this before moving on to task 4.

Task 4: Create a visualization of your list using ASCII art.
1. Modify your Student class to include a display method that will output to the screen the
contents of the class
  a. This method should write directly to the screen.
  b. This method does not need to display all members of the item, just key members
  (explain your choice of key members in your lab report).
  c. This method should reuse members of the class as much as possible.

3. Modify your linked list class to add a new public method to display the list.
  a. This method should write directly to the screen.
  b. This method should walk through the list and display every item in the list on the
  screen. The format of the output is up to you.
  c. To display the contents of the item in the list, it should call the display member
  of the item (created in step 1 of this task).
  d. This method should reuse members of the class as much as possible.
  e. This method should not change the results of SeeNext method meaning it should
  not have a different value for the internal variable used by SeeNext after this
  method completes.
4. Modify your test program from task 3 to include an option that calls this new method.
5. Include in the lab report a screen shot(s) of the output of a test.
