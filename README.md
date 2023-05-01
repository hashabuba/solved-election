Download Link: https://assignmentchef.com/product/solved-election
<br>
<strong>a) </strong>Ask the user for the number of candidates in a local election. Use a try/except block to make sure the user does not enter a character or a floating point number as input. You need a loop to assure the user enters a valid whole number.

<strong>b)</strong> Given the number of candidates, ask for the user for last names of a series of candidates and the number of votes received by each candidate and store the data in 2 parallel arrays.

<strong>c)</strong> Validate the number of votes to make sure the number of votes is not a negative number. If a negative number is entered, the program must issue a message and continue to ask the user for a valid entry.

<strong>d)</strong> Write a function to display each candidate’s name, the number of votes received, and the percentage of the total votes received by the candidate. The percentage value is calculated by dividing the number of votes by the total number of votes and multiplying the number by 100. The function accepts 2 arrays and the size of the array and displays the desired output. Make sure to display the percentage values to 2 digits after the decimal point.

<strong>e)</strong> Write a function that accepts the name of an output file and displays the array of names and the array of votes to the provided output file. Each record must be written on its own line. Note that the name of the file is entered in the main function and the value passed to the function along with the arrays to be displayed.

<strong>f)</strong> Write a function to return the name of the winner. DO NOT use a pre-defined Python function. The function accepts the array of names and votes, finds the minimum number of votes and returns the name associated with the minimum number of votes.

<strong>g)</strong> Write a function to return the name of the loser. DO NOT use a pre-defined Python function. The function accepts the array of names and votes, finds the maximum number of votes and returns the name associated with the minimum number of votes.

<strong>h)</strong> Write a function to sort the candidates by name. I just need the names in a sorted order. The function accepts an array of names and sorts the data. After the function is called, the data would be in alphabetical order. LOOK at the end of this document for a pseudocode for a function that sorts the data. ALL you have to do is to convert the pseudocode to Python code. Make sure to display the data in the sorted order.

<strong>i)</strong> Write a function that accepts as parameter the name of a candidate and return the number of votes received by the candidate. So, if the user enters Duck, the output will be 6000. Of course, if the given name does not exist, display an appropriate message.

FUNCTION sortData(array, arraySize)

Set flag = 0

While flag == 0

Set flag = 1

Set k = 0 While k &lt;= (arraySize – 2)

If array[k] &gt; array[k+1] then

Set temp = array[k]

array[k] = array[k+1]

array[k+1] = temp

set flag = 0

end if

set k = k + 1

end while(k)

end while(flag)

FUNCTION searchData(arrayName, arrayData, arraySize, searchItem)

Set found = 0

Set index = 0

While found == 0 and index &lt; arraySize

If searchItem == arrayName [index] then

found = 1

index = index + 1

end while

if found == 1 then

return arrayData[index – 1]

else

return -99

End if

NOTE: The function either returns the number of votes or -99 when the name was not found. In the main function, we can use this return value in an IF statement to either display the number of votes or a message that the name is not found.