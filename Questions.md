# Python-Strings
End of topic project: Medical Insurnace
Working with Strings
1.
First, take a look at the code in script.py.

The string medical_data stores the medical records for ten individuals. Each record is separated by a ; and contains the name, age, BMI (body mass index), and insurance cost for an individual, in that order.

Print medical_data to see the output in the terminal


Stuck? Get a hint
2.
We want the insurance costs to be represented in US dollars.

Replace all instances of # in medical_data with $. Store the result in a variable called updated_medical_data.

Print updated_medical_data.


Stuck? Get a hint
3.
We want to calculate the number of medical records in our data.

Create a variable called num_records and initialize it at 0.


Stuck? Get a hint
4.
Next, write a for loop to iterate through the updated_medical_data string. Inside of the loop, add 1 to num_records when the current character is equal to $.


Stuck? Get a hint
5.
Outside of the loop, print num_records with the following message:

There are {num_records} medical records in the data.

Stuck? Get a hint
Splitting Strings
6.
The medical data in its current form is difficult to analyze. An essential job for a data scientist is to clean up data so that it’s easy to work with.

Let’s start off by splitting the updated_medical_data string into a list of each medical record. Remember that each medical record is separated by a ; in the string.

Store the result in a variable called medical_data_split and print this variable.


Stuck? Get a hint
7.
Our data is now stored in a list, but it is still hard to read. Let’s split each medical record into its own list.

First, define an empty list called medical_records.


Stuck? Get a hint
8.
Next, iterate through medical_data_split and for each record, split the string after each comma (,) and append the split string to medical_records.

Print medical_records after the loop.


Stuck? Get a hint
Cleaning Data
9.
Our data is now slightly more readable. However, it is not properly formatted – it contains unnecessary whitespace.

To fix this, let’s start by creating an empty list called medical_records_clean.


Stuck? Get a hint
10.
Next, use a for loop to iterate through medical_records.

Inside of the loop, create an empty list called record_clean. We’ll use this list to store a formatted version of each medical record.


Stuck? Get a hint
11.
After the record_clean variable, create a nested for loop that goes through each record:

for item in record:
Inside of this loop, append item.strip() to record_clean to remove any whitespace from the string.


Stuck? Get a hint
12.
Finally, we need to add each cleaned up record to medical_records_clean.

Outside of the nested for loop, append record_clean to medical_records_clean.


Stuck? Get a hint
13.
Print medical_records_clean outside of the for loops to see the output.

You should see output that is formatted and much easier to read.


Stuck? Get a hint
Analyzing Data
14.
Our data is now clean and ready for analysis.

For example, to print out the names of each of the ten individuals, we can use the following loop:

for record in medical_records_clean:
  print(record[0])
Add this loop to your code and click “Save.”


Stuck? Get a hint
15.
You want all of the names in the medical records to be in uppercase characters.

In the for loop, update records[0] before the print statement so that all of the characters are uppercase.

Click “Save” to see the result.


Stuck? Get a hint
16.
Let’s store each name, age, BMI, and insurance cost in separate lists.

To start, create four empty lists:

names
ages
bmis
insurance_costs

Stuck? Get a hint
17.
Next, iterate through medical_records_clean and for each record:

Append the name to names.
Append the age to ages.
Append the BMI to bmis.
Append the insurance cost to insurance_costs.

Stuck? Get a hint
18.
Print names, ages, bmis, and insurance_costs outside of the loop.

Make sure the output is what you expect.


Stuck? Get a hint
19.
Now that all of our data is in separate lists, we can easily perform analysis on that data. Let’s calculate the average BMI in our dataset.

First, create a variable called total_bmi and set it equal to 0.


Stuck? Get a hint
20.
Next, use a for loop to iterate through bmis and add each bmi to total_bmi.

Remember to convert bmi to a float.


Stuck? Get a hint
21.
After the for loop, create a variable called average_bmi that stores the total_bmi divided by the length of the bmis list.

Print out average_bmi with the following message:

Average BMI: {average_bmi}

Stuck? Get a hint
Extra
22.
Congratulations! In this project, you used Python strings to transform and clean up medical data.

As a data scientist, it’s important that you have clean and accurate data before you analyze it. You now have a better idea of the data preparation process moving forward.

If you’d like extra practice with Python strings, here are some suggestions to get you started:

Calculate the average insurance cost in insurance_costs. You will have to remove the $ in order to calculate this.
Write a for loop that outputs a string for each individual in the following format:
Marina is 27 year olds with a BMI of 31.1 and an insurance cost of $7010.0.
Markus is 30 years old with a BMI of 22.4 and an insurance cost of $4050.0
...
...
Happy coding!
