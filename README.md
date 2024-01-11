# Create-Loops-in-Python

<h2>Introduction</h2>

As a security analyst, some of the measures I take to protect a system will involve repetition. As an example, I might need to investigate multiple IP addresses that have attempted to connect to the network. In Python, iterative statements can help automate repetitive processes like these to make them more efficient.

In this lab, I will practice writing iterative statements in Python.

<h2>Scenario</h2>

I'm working as a security analyst, and I'm writing programs in Python to automate displaying messages regarding network connection attempts, detecting IP addresses that are attempting to access restricted data, and generating employee ID numbers for a Sales department.

<h2>Task 1</h2>

In this task, I'll create a loop related to connecting to a network.

Write an iterative statement that displays Connection could not be established three times. Use the for keyword, the range() function, and a loop variable of i

![image](https://github.com/n8som/Create-Loops-in-Python/assets/110139109/b70448e4-4730-4275-8d1f-8c59d9cf2c8b)

<h2>Task 2</h2>

The range() function can also take in a variable. To repeat a specified action a certain number of times, I can first assign an integer value to a variable. Then, I can pass that variable into the range() function within a for loop.

In my code that displays a network message connection, incorporate a variable called connection_attempts. Assign the positive integer of my choice as the value of that variable and fill in the missing variable in the iterative statement. Test out the code with different values for connection_attempts and observe what happens.

![image](https://github.com/n8som/Create-Loops-in-Python/assets/110139109/0cec0561-b9ad-46ca-a714-d6381efd2616)

![image](https://github.com/n8som/Create-Loops-in-Python/assets/110139109/7c325a94-c04b-4646-a795-b63fc09cb0ec)

<h2>Task 3</h2>

This task can also be achieved with a while loop. Complete the while loop with the correct code to instruct it to display "Connection could not be established." three times.

In this task, a for loop and a while loop will produce similar results, but each is based on a different approach. (In other words, the underlying logic is different in each.) A for loop terminates after a certain number of iterations have completed, whereas a while loop terminates once it reaches a certain condition. In situations where I do not know how many times the specified action should be repeated, while loops are most appropriate.

![image](https://github.com/n8som/Create-Loops-in-Python/assets/110139109/3773be68-7b71-4576-a9c1-2157357960ab)

The messages outputted from both loops, ```for``` and ```while``` were identical. The logic is what differed between the two loops. In the ```for``` loop, the loop variable i was automatically defined in the loop header, and it was updated automatically in each iteration. In the ```while``` loop, the loop variable connection_attempts had to be defined before the loop header, and it had to be explicitly updated inside the loop body.

<h2>Task 4</h2>

Now, I'll move onto my next task. I'll automate checking whether IP addresses are part of an allow list. I will start with a list of IP addresses from which users have tried to log in, stored in a variable called ip_addresses. Write a for loop that displays the elements of this list one at a time. Use i as the loop variable in the for loop.

![image](https://github.com/n8som/Create-Loops-in-Python/assets/110139109/d43b7877-c2bd-4d00-8950-a12fca12e606)

<h2>Task 5</h2>

I am now given a list of IP addresses that are allowed to log in, stored in a variable called allow_list. Write an if statement inside of the for loop. For each IP address in the list of IP addresses from which users have tried to log in, display "IP address is allowed" if it is among the allowed addresses and display "IP address is not allowed" otherwise.

![image](https://github.com/n8som/Create-Loops-in-Python/assets/110139109/e19967c0-593a-4643-9fc0-0f057dcddf90)

<h2>Task 6</h2>

Imagine now that the information the users are trying to access is restricted, and if an IP address outside the list of allowed IP addresses attempts access, the loop should terminate because further investigation would be needed to assess whether this activity poses a threat. To achieve this, use the break keyword and expand the message that is displayed to the user when their IP address is not in allow_list to provide more specifics. Instead of "IP address is not allowed", display "IP address is not allowed. Further investigation of login activity required".

![image](https://github.com/n8som/Create-Loops-in-Python/assets/110139109/0b1dd96b-41b8-4484-be1e-8a14ea3e088a)

<h2>Task 7</h2>

I'll now complete another task. This involves automating the creation of new employee IDs.

I have been asked to create employee IDs for a Sales department, with the criteria that the employee IDs should all be numbers that are unique, divisible by 5, and falling between 5000 and 5150. The employee IDs can include both 5000 and 5150.

Write a while loop that generates unique employee IDs for the Sales department by iterating through numbers and displays each ID created.

![image](https://github.com/n8som/Create-Loops-in-Python/assets/110139109/a3f6868d-9880-4105-b7bb-2381279013f9)

<h2>Task 8</h2>

I would like to incorporate a message that displays Only 10 valid employee ids remaining as a helpful alert once the loop variable reaches 5100.

To do so, include an if statement in my code.

![image](https://github.com/n8som/Create-Loops-in-Python/assets/110139109/24c38cff-7634-480f-a4ed-99a9c2b84819)

Why do you think the statement print(i) is written before the conditional rather than inside the conditional?

The goal is to display every employee ID number that's created, and the loop variable i represents the ID number created in each iteration of the loop. The statement print(i) is written before the conditional, so that the loop is displayed in every iteration. Otherwise, if print(i) was written inside the conditional, the loop variable would only be printed out when it's equal to 5100. (Since the condition in the if statement is i == 5100.)

<h2>Conclusion</h2>

What are the key takeaways from this lab?

- Iterative statements play a major role in automating security-related processes that need to be repeated.
- I can use for loops to repeat a process a specified number of times.
- I can use while loops to repeat a process until a specified condition has been met. Comparison operators are often used in these conditions.
  - The < comparison operator allows me to check whether one value is less than another.
  - The <= comparison operator allows me to check whether one value is less than or equal to another.
  - The == comparison operator allows me to check whether one value is equal to another.

