                                                            **Assignment-2**
    

Name: Meghana Chodagiri

Student Id: 700749050


GitHub Link: https://github.com/meghanach1/Assignment-2

Video Link:  https://drive.google.com/file/d/1Rqg0YcQBoyV0Xld-V2-XDSCmSYRstZvG/view?usp=sharing


  1.	Use a python code to display the following star pattern using the for loop


            As per the required output taking rows count as 5
            rows = 5
            # Using for loop for iterating the number of rows
            for i in range (0, rows):
            # Iterating the columns and printing stars till rows count= 5
            for j in range (0, i + 1):
            print ("*", end=' ')
            print (" ")
            # After printing 5 rows again starting second iteration and printing stars till 1
            for i in range (rows, 0, -1):
            for j in range (0, i - 1):
            print ("*", end=' ')
            print (" ")
 

 Output :
 
    *
    * *
    * * *
    * * * *
    * * * * *
    * * * *
    * * *
    * *
    *

2. Use looping to output the elements from a provided list present at odd indexes.
my_list = [10, 20, 30, 40, 50, 60, 70, 80, 90, 100]


A.

    Given list of numbers
    my_list = [10, 20, 30, 40, 50, 60, 70, 80, 90, 100]
    I have created empty list to add only values present in odd indexes
    odds_list= []
    The list index starts with 0
    count = 0
    using for loop iterating the list and finding the values which are in odd places. Let count be the variable that points to the index of the list and when the index  is divided by 2, if the remainder is 1 then the index is odd
    for i in my_list:
    if count % 2 == 1:
    odds_list.append(i)
    count += 1
    after values are appended to the empty list, printing the list
    print(odds_list)

Output is 

    [20, 40, 60, 80, 100]

3. Write a code that appends the type of elements from a given list.
Input
x = [23, ‘Python’, 23.98]
Expected output
[23, 'Python', 23.98]
[<class 'int'>, <class 'str'>, <class 'float'>]
A.

        Declaring given list is below
        x = [23, 'Python',23.98]
        Created another empty list to print the list of datatypes
        dt = []
        Using for loop to iterate the list and getting values to find datatypes by using type() method.
        After finding the datatypes, appending into the empty list dt using append() method
        for i in range(len(x)):
        dt.append(type(x[i]))
        Now, printing both the lists.
        print(x)
        print(dt)


Output:
    
    [23, 'Python', 23.98]
    [<class 'int'>, <class 'str'>, <class 'float'>]

4. Write a function that takes a list and returns a new list with unique items of the first list.
Sample List: [1,2,3,3,3,3,4,5]
Unique List: [1, 2, 3, 4, 5]

A.

    Declaring a user defined function called unique_list and passing a parameter l
    def unique_list(l):
    inside function, we are writing program to get unique items.
    First created an empty list x
    x = []
    Using for loop iterating list of l where we are passing input at the last. The loop will check if there is any item in the other list and append only unique values in new list using append() method
    for a in l:
    if a not in x:
    x.append(a)
    after appending and if the loop ends , it will return the list x and printing the list.
    return x
    print(unique_list([1,2,3,3,3,3,4,5]))


Output:
       
       [1, 2, 3, 4, 5]

5. Write a function that accepts a string and calculate the number of upper-case letters and lower-case
letters.
Input String: 'The quick Brow Fox'

    A.
    
        Declaring given string as str
        str = "The quick Brow Fox"
        declaring count of upper- case and lower-case letters as 0
        upper=0
        lower=0
        using for loop iterating the str, the loop checks if the letter in the string is lower case or upper case using islower() and isupper() methods. Increasing count values respectively if the letter is lower or upper.
        for i in str:
        if (i.islower()):
        lower=lower+1
        elif (i.isupper()):
        upper=upper+1
        Printing the count of lower and upper case letters as below
        print("No of Upper-case characters:",upper)
        print("No of lower case letters:",lower)

 
Output:

    No of Upper-case characters: 3
    No of lower case letters: 12

