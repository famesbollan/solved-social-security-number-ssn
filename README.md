Download Link: https://assignmentchef.com/product/solved-social-security-number-ssn
<br>
5/5 - (3 votes)

Your program should prompt a user to enter a social security number (SSN) as a series of digits.It will check whether the user entered a valid 9-digit SSN and report an error message if the SSN entered is too short or too long or if the user enters a non-numeric input.It should report a specific error message for each of the three possible errors listed in the bullet point above.If the user makes a mistake, the program should re-prompt the user using a loop (suggestion: do-while loop).Once the user enters a valid input, the program will display the SSN in the the format XXX-XX-XXXXYou are required to write a function with the following signature to check whether the user entered a numerical SSN (i.e. whether all of the digits entered were numerical). If the user enters any other character besides 0-9, return false, otherwise return true. Hint: Use ASCIICopy and paste the below prototype above main and then write the function below main.bool isNumeric(string SSN);//use ASCII to determines if a string contains only the characters 0-9



You are also required to have a function with the following signature to display the SSN.Copy and paste the below prototype above main and then write the function below main.void displayFormattedNumber(string SSN);

//Calls the formatSSN function and then displays it to the console

//With the message “You entered: ” followed by the SSN

string formatSSN(string SSN);

//helper function to displayFormatted SSN

//converts a 9 character string into an SSN in the format XXX-XX-XXXX

Your program should work identically to example below:Please enter a 9-digit SSN (no spaces no punctuation): 12345

You entered too few digits. Please try again.

Please enter a 9-digit SSN (no spaces no punctuation): 123456789012345

You entered too many digits. Please try again.

Please enter a 9-digit SSN (no spaces no punctuation): 123 456

You entered too few digits. Please try again.

Please enter a 9-digit SSN (no spaces no punctuation): 123 456 7890

Please enter a number with no spaces or punctuation. Please try again.

Please enter a 9-digit SSN (no spaces no punctuation): 123-45-6789

Please enter a number with no spaces or punctuation. Please try again.

Please enter a 9-digit SSN (no spaces no punctuation): 123456789

You entered: 123-45-6789

It is strongly suggested to structure your main function like this:bool not_valid_SSN = true;

do {

//user input

if (test for too short) {

//display appropriate error message

} else if (!is_numeric(SSN)) {

//display error message

} else if(test for too long) {

//display appropriate error message

} else {

//display appropriate formatted phone number

not_valid_SSN = false;

}

} while(not_valid_SSN);