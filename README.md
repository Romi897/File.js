# File.js
This is typescript assignment file
//Qno:1Install Node.js, TypeScript and VS Code on your computer.
//Qno:2 Personal Message: Store a person’s name in a variable, and print a message to that person. Your message should be simple, such as, “Hello Eric, would you like to learn some Python today?”
//Solution:
var personName = "Eric";
console.log("Hello " + personName + ", would you like to learn some Python today?");

//Qno:3 Name Cases: Store a person’s name in a variable, and then print that person’s name in lowercase, uppercase, and titlecase.
//Solution:
var name1 = "wania";
var name2 = "ahmed";
var name3 = "hamza";
console.log("Lowercase:");
console.log(name1.toLowerCase());
console.log(name2.toLowerCase());
console.log(name3.toLowerCase());
console.log("\nUppercase:");
console.log(name1.toUpperCase());
console.log(name2.toUpperCase());
console.log(name3.toUpperCase());
console.log("\nTitlecase:");
console.log(titleCase(name1));
console.log(titleCase(name2));
console.log(titleCase(name3));
function titleCase(str) {
  return str.toLowerCase().replace(/(^|\s)\S/g, function (letter) {
    return letter.toUpperCase();
  });
}
//Qno:4 Famous Quote: Find a quote from a famous person you admire. Print the quote and the name of its author. Your output should look something like the following, including the quotation marks:
//Albert Einstein once said, “A person who never made a mistake never tried anything new.”
//Solution:
var quote = "A person who never made a mistake never tried anything new.";
var author = "Albert Einstein";
console.log(author + " once said, \"" + quote + "\"");

//Qno:5 Famous Quote 2: Repeat Exercise 4, but this time store the famous person’s name in a variable called famous_person. Then compose your message and store it in a new variable called message. Print your message.
//Solution:
var famous_person = "Albert Einstein";
var quote = "A person who never made a mistake never tried anything new.";
var message = famous_person + " once said, \"" + quote + "\"";
console.log(message);

//Qno:6 Stripping Names: Store a person’s name, and include some whitespace characters at the beginning and end of the name. Make sure you use each character combination, "\t" and "\n", at least once. Print the name once, so the whitespace around the name is displayed. Then print the name after striping the white spaces.
//Solution:
let nameWithWhitespace = "\n\t Wania \t\n";
console.log("Name with whitespace:", nameWithWhitespace);
let strippedName = nameWithWhitespace.trim();
console.log("Stripped name:", strippedName);


//Qno:7 Number Eight: Write addition, subtraction, multiplication, and division operations that each result in the number 8. Be sure to enclose your operations in print statements to see the results.

//Solution:
console.log("Addition: " + (5 + 3));
console.log("Subtraction: " + (10 - 2));
console.log("Multiplication: " + (4 * 2));
console.log("Division: " + (16 / 2));

//Qno:8 You should create four lines that look like this:
//console.log(5 + 3)
//Your output should simply be four lines with the number 8 appearing once on each line.
//Solution:
console.log(5 + 3);
console.log(10 - 2);
console.log(4 * 2);
console.log(16 / 2);

//Qno:9 Favorite Number: Store your favorite number in a variable. Then, using that variable, create a message that reveals your favorite number. Print that message.
//Solution:
var favoriteNumber = 7;
var message = "My favorite number is: " + favoriteNumber;
console.log(message);

//Qno:10 Adding Comments: Choose two of the programs you’ve written, and add at least one comment to each. If you don’t have anything specific to write because your programs are too simple at this point, just add your name and the current date at the top of each program file. Then write one sentence describing what the program does.
//Solution:
let nameWithWhitespace = "\n\t Wania \t\n";
console.log("Name with whitespace:", nameWithWhitespace);
let strippedName = nameWithWhitespace.trim();
console.log("Stripped name:", strippedName);
let guests = ["Ali", "Raza", "Ahmed", "Umer", "Anas"];
console.log("Invitation Messages:");
for (let i = 0; i < guests.length; i++) {
    console.log("Dear " + guests[i] + ", you're invited to dinner!");
}
let guestCantMakeIt = "Umer";
console.log("\nUnfortunately, " + guestCantMakeIt + " can't make it to dinner.");
let newGuest = "Hassan";
let indexOfGuestCantMakeIt = guests.indexOf(guestCantMakeIt);
if (indexOfGuestCantMakeIt !== -1) {
    guests.splice(indexOfGuestCantMakeIt, 1, newGuest);
}
console.log("\nUpdated Invitation Messages:");
for (let i = 0; i < guests.length; i++) {
    console.log("Dear " + guests[i] + ", you're invited to dinner!");
}
let guests = ["Ali", "Raza", "Ahmed", "Umer", "Anas"];
console.log("Invitation Messages:s");
for (let i = 0; i < guests.length; i++) {
    console.log("Dear " + guests[i] + ", you're invited to dinner!");
}
let guestCantMakeIt = "Umer";
console.log("\nUnfortunately, " + guestCantMakeIt + " can't make it to dinner.");
let newGuest = "Hassan";
let indexOfGuestCantMakeIt = guests.indexOf(guestCantMakeIt);
if (indexOfGuestCantMakeIt !== -1) {
    guests.splice(indexOfGuestCantMakeIt, 1, newGuest);
}
console.log("\nUpdated Invitation Messages:");
for (let i = 0; i < guests.length; i++) {
    console.log("Dear " + guests[i] + ", you're invited to dinner!");
}
//Qno:13 Your Own Array: Think of your favorite mode of transportation, such as a motorcycle or a car, and make a list that stores several examples. Use your list to print a series of statements about these items, such as “I would like to own a Honda motorcycle.”
//solution:
var modesOfTransportation = ["car", "motorcycle", "bicycle", "train"];
for (var i = 0; i < modesOfTransportation.length; i++) {
    console.log("I would like to own a " + modesOfTransportation[i] + ".");
}
//Qno:14 Guest List: If you could invite anyone, living or deceased, to dinner, who would you invite? Make a list that includes at least three people you’d like to invite to dinner. Then use your list to print a message to each person, inviting them to dinner.
//solution:
let guests = ["Ali", "Anas", "Ahmed", "Raza"];
for (let i = 0; i < guests.length; i++) {
    console.log("Dear " + guests[i] + ", you're invited to dinner!");
}
//Qno:15 Changing Guest List: You just heard that one of your guests can’t make the dinner, so you need to send out a new set of invitations. You’ll have to think of someone else to invite.
//• Start with your program from Exercise 14. Add a print statement at the end of your program stating the name of the guest who can’t make it.
//• Modify your list, replacing the name of the guest who can’t make it with the name of the new person you are inviting.
//• Print a second set of invitation messages, one for each person who is still in your list.
//solution:
let guests = ["Ali", "Raza", "Ahmed", "Umer", "Anas"];
console.log("Invitation Messages:");
for (let i = 0; i < guests.length; i++) {
    console.log("Dear " + guests[i] + ", you're invited to dinner!");
}
let guestCantMakeIt = "Umer";
console.log("\nUnfortunately, " + guestCantMakeIt + " can't make it to dinner.");
let newGuest = "Hassan";
let indexOfGuestCantMakeIt = guests.indexOf(guestCantMakeIt);
if (indexOfGuestCantMakeIt !== -1) {
    guests.splice(indexOfGuestCantMakeIt, 1, newGuest);
}
console.log("\nUpdated Invitation Messages:");
for (let i = 0; i < guests.length; i++) {
    console.log("Dear " + guests[i] + ", you're invited to dinner!");
}
//Qno:16 More Guests: You just found a bigger dinner table, so now more space is available. Think of three more guests to invite to dinner.
//• Start with your program from Exercise 15. Add a print statement to the end of your program informing people that you found a bigger dinner table.
//• Add one new guest to the beginning of your array.
//• Add one new guest to the middle of your array. • Use append() to add one new guest to the end of your list. • Print a new set of invitation messages, one for each person in your list.

//Solution:
let guests = ["Ali", "Hamza", "Raza", "Ahmed", "Anas", "Romaisa"];
console.log("Invitation Messages:");
for (let i = 0; i < guests.length; i++) {
    console.log("Dear " + guests[i] + ", you're invited to dinner!");
}
console.log("\nGreat news! A bigger dinner table has been found.");
guests.unshift("Sana");
guests.splice(Math.floor(guests.length / 2), 0, "Saad");
guests.push("Alisha");
console.log("\nUpdated Invitation Messages:");
for (let i = 0; i < guests.length; i++) {
    console.log("Dear " + guests[i] + ", you're invited to dinner!");
}
//Qno:17 Shrinking Guest List: You just found out that your new dinner table won’t arrive in time for the dinner, and you have space for only two guests.
//• Start with your program from Exercise 16. Add a new line that prints a message saying that you can invite only two people for dinner.
//• Remove guests from your list one at a time until only two names remain in your list. Each time you pop a name from your list, print a message to that person letting them know you’re sorry you can’t invite them to dinner.
//• Print a message to each of the two people still on your list, letting them know they’re still invited.
//• Remove the last two names from your list, so you have an empty list. Print your list to make sure you actually have an empty list at the end of your program.
//Solution:

let guests = ["Ali", "Hamza", "Sam", "Nihal", "Nehan", "Raza"];
console.log("Unfortunately, due to space constraints, only two people can be invited for dinner.");
while (guests.length > 2) {
    let removedGuest = guests.pop();
    console.log("Sorry, " + removedGuest + ", you're no longer invited to dinner.");
}
console.log("Dear " + guests[0] + ", you're still invited to dinner.");
console.log("Dear " + guests[1] + ", you're still invited to dinner.");
guests.pop();
guests.pop();
console.log("Remaining guests:", guests);



//Qno:18 Seeing the World: Think of at least five places in the world you’d like to visit.
//• Store the locations in a array. Make sure the array is not in alphabetical order.
//• Print your array in its original order.
//• Print your array in alphabetical order without modifying the actual list.
//• Show that your array is still in its original order by printing it.
//• Print your array in reverse alphabetical order without changing the order of the original list.
//• Show that your array is still in its original order by printing it again.
//• Reverse the order of your list. Print the array to show that its order has changed.
//• Reverse the order of your list again. Print the list to show it’s back to its original order.
//• Sort your array so it’s stored in alphabetical order. Print the array to show that its order has been changed.
//• Sort to change your array so it’s stored in reverse alphabetical order. Print the list to show that its order has changed.
//Solution:
let placesInPakistan = ["Hunza Valley", "Lahore", "Karachi", "Murree", "Swat Valley"];
console.log("Original order:", placesInPakistan);
console.log("Alphabetical order:", [...placesInPakistan].sort());
console.log("Original order (again):", placesInPakistan);
console.log("Reverse alphabetical order:", [...placesInPakistan].sort().reverse());
console.log("Original order (again):", placesInPakistan);
placesInPakistan.reverse();
console.log("Reversed order:", placesInPakistan)
placesInPakistan.reverse();
console.log("Original order (again):", placesInPakistan);
placesInPakistan.sort();
console.log("Sorted in alphabetical order:", placesInPakistan);
placesInPakistan.sort((a, b) => b.localeCompare(a));
console.log("Sorted in reverse alphabetical order:", placesInPakistan);


//Qno:19 Dinner Guests: Working with one of the programs from Exercises 14 through 18, print a message indicating the number of people you are inviting to dinner.
//Solution:
let guests = ["Ayesha", "Ali", "Ahmed", "Wania", "Hamza", "Zara"];
let numberOfGuests = guests.length;
console.log("You are inviting " + numberOfGuests + " people to dinner.");
console.log("Guests:");
for (let i = 0; i < numberOfGuests; i++) {
    console.log("- " + guests[i]);
}
//Qno:20 Think of something you could store in a array. For example, you could make a list of mountains, rivers, countries, cities, languages, or anything else you’d like. Write a program that creates a list containing these items.
//Solution:
let citiesOfPakistan = ["Karachi", "Lahore", "Islamabad", "Rawalpindi", "Faisalabad", "Multan", "Peshawar", "Quetta"];
console.log("Cities of Pakistan:");// Define an array of people to invite to dinner
let guests = ["Ali", "Anas", "Ahmed", "Raza"];

// Loop through the array and print an invitation message for each person
for (let i = 0; i < guests.length; i++) {
    console.log("Dear " + guests[i] + ", you're invited to dinner!");
}

for (let i = 0; i < citiesOfPakistan.length; i++) {
    console.log("- " + citiesOfPakistan[i]);
}
//Qno:21 They think of something you could store in a TypeScript Object. Write a program that creates Objects containing these items.

//Solution:
function createWaterBottle(brand, capacity, material, color) {
    return {
        brand: brand,
        capacity: capacity,
        material: material,
        color: color
    };
}
let bottle1 = createWaterBottle("Nalgene", "32 oz", "Plastic", "Blue");
let bottle2 = createWaterBottle("Hydro Flask", "20 oz", "Stainless Steel", "Black");
let bottle3 = createWaterBottle("CamelBak", "24 oz", "Plastic", "Green");
console.log("Water Bottle 1:", bottle1);
console.log("Water Bottle 2:", bottle2);
console.log("Water Bottle 3:", bottle3);
//QNO:22 Intentional Error: If you haven’t received an array index error in one of your programs yet, try to make one happen. Change an index in one of your programs to produce an index error. Make sure you correct the error before closing the program.
//Solution:
let myArray = [1, 2, 3, 4, 5];
console.log(myArray[10]);
console.log(myArray[2]); 


//Qno:23 Conditional Tests: Write a series of conditional tests. Print a statement describing each test and your prediction for the results of each test. Your code should look something like this:
//let car = 'subaru';
//console.log("Is car == 'subaru'? I predict True.")
//console.log(car == 'subaru')
//• Look closely at your results, and make sure you understand why each line evaluates to True or False.
//• Create at least 10 tests. Have at least 5 tests evaluate to True and another 5 tests evaluate to False.

//Solution:

let x = 5;
let y = 10;
console.log("Test 1: Is x equal to 5? I predict True.");
console.log(x == 5); 
console.log("Test 2: Is y not equal to 10? I predict False.");
console.log(y != 10);
console.log("Test 3: Is x greater than y? I predict False.");
console.log(x > y); 
console.log("Test 4: Is x less than y? I predict True.");
console.log(x < y); 
console.log("Test 5: Is y greater than or equal to 10? I predict True.");
console.log(y >= 10);
console.log("Test 6: Is x less than or equal to 5? I predict True.");
console.log(x <= 5); 
console.log("Test 7: Is x equal to 5 AND y equal to 10? I predict True.");
console.log(x == 5 && y == 10); 
console.log("Test 8: Is x equal to 5 OR y equal to 5? I predict True.");
console.log(x == 5 || y == 5);
console.log("Test 9: Is NOT(x equal to 10)? I predict True.");
console.log(!(x == 10)); 
console.log("Test 10: Is '5' equal to 5? I predict False.");
console.log('5' == 5); 

//Qno24:More Conditional Tests: You don’t have to limit the number of tests you create to 10. If you want to try more comparisons, write more tests. Have at least one True and one False result for each of the following:
//• Tests for equality and inequality with strings
//• Tests using the lower case function
//• Numerical tests involving equality and inequality, greater than and less than, greater than or equal to, and less than or equal to
//• Tests using "and" and "or" operators
//• Test whether an item is in a array
//• Test whether an item is not in a array

//Solution:

let string1 = 'apple';
let string2 = 'banana';
let number1 = 5;
let number2 = 10;
let array = ['apple', 'banana', 'orange'];
console.log("Test 1: Is 'apple' equal to 'banana'? I predict False.");
console.log(string1 == string2);

console.log("Test 2: Is 'apple' not equal to 'banana'? I predict True.");
console.log(string1 != string2);
console.log("Test 3: Is 'APPLE' equal to 'apple'? I predict True.");
console.log(string1.toLowerCase() == 'apple'); 
console.log("Test 4: Is 5 equal to 10? I predict False.");
console.log(number1 == number2); 

console.log("Test 5: Is 5 greater than 10? I predict False.");
console.log(number1 > number2); 

console.log("Test 6: Is 5 less than 10? I predict True.");
console.log(number1 < number2);

console.log("Test 7: Is 5 greater than or equal to 5? I predict True.");
console.log(number1 >= number1);

console.log("Test 8: Is 5 less than or equal to 10? I predict True.");
console.log(number1 <= number2); 
console.log("Test 9: Is 5 less than 10 AND 'apple' equal to 'apple'? I predict True.");
console.log(number1 < number2 && string1 == 'apple');

console.log("Test 10: Is 5 less than 10 OR 'apple' equal to 'banana'? I predict True.");
console.log(number1 < number2 || string1 == string2); 
console.log("Test 11: Is 'banana' in the array? I predict True.");
console.log(array.includes('banana')); 
console.log("Test 12: Is 'grape' not in the array? I predict True.");
console.log(!array.includes('grape')); 

//Qno25:Alien Colors #1: Imagine an alien was just shot down in a game. Create a variable called alien_color and assign it a value of 'green', 'yellow', or 'red'.
//• Write an if statement to test whether the alien’s color is green. If it is, print a message that the player just earned 5 points.
//• Write one version of this program that passes the if test and another that fails. (The version that fails will have no output.)

//Solution:
var alien_color = 'green';
if (alien_color === 'green') {
    console.log("Congratulations! You just earned 5 points.");
}
var alien_color = 'red';
if (alien_color === 'green') {
    console.log("Congratulations! You just earned 5 points.");
}

//Qno:26 Alien Colors #2: Choose a color for an alien as you did in Exercise 25, and write an if-else chain.
//• If the alien’s color is green, print a statement that the player just earned 5 points for shooting the alien.
//• If the alien’s color isn’t green, print a statement that the player just earned 10 points.
//• Write one version of this program that runs the if block and another that runs the else block.

//Solution:
var alien_color = 'green';
if (alien_color === 'green') {
    console.log("Congratulations! You just earned 5 points for shooting the alien.");
} else {
    console.log("Congratulations! You just earned 10 points.");
}
var alien_color = 'red';
if (alien_color === 'green') {
    console.log("Congratulations! You just earned 5 points for shooting the alien.");
} else {
    console.log("Congratulations! You just earned 10 points.");
}
//Qno27:Alien Colors #3: Turn your if-else chain from Exercise 5-4 into an if-else chain.
//• If the alien is green, print a message that the player earned 5 points.
//• If the alien is yellow, print a message that the player earned 10 points.
//• If the alien is red, print a message that the player earned 15 points.
//• Write three versions of this program, making sure each message is printed for the appropriate color alien.

//Solution:
var alien_color = 'green';
if (alien_color === 'green') {
    console.log("Congratulations! You just earned 5 points.");
} else if (alien_color === 'yellow') {
    console.log("Congratulations! You just earned 10 points.");
} else if (alien_color === 'red') {
    console.log("Congratulations! You just earned 15 points.");
}
var alien_color = 'yellow';
if (alien_color === 'green') {
    console.log("Congratulations! You just earned 5 points.");
} else if (alien_color === 'yellow') {
    console.log("Congratulations! You just earned 10 points.");
} else if (alien_color === 'red') {
    console.log("Congratulations! You just earned 15 points.");
}
var alien_color = 'red';
if (alien_color === 'green') {
    console.log("Congratulations! You just earned 5 points.");
} else if (alien_color === 'yellow') {
    console.log("Congratulations! You just earned 10 points.");
} else if (alien_color === 'red') {
    console.log("Congratulations! You just earned 15 points.");
}

//Qno:28 Stages of Life: Write an if-else chain that determines a person’s stage of life. Set a value for the variable age, and then:
//• If the person is less than 2 years old, print a message that the person is a baby.
//• If the person is at least 2 years old but less than 4, print a message that the person is a toddler.
//• If the person is at least 4 years old but less than 13, print a message that the person is a kid.
//• If the person is at least 13 years old but less than 20, print a message that the person is a teenager.
//• If the person is at least 20 years old but less than 65, print a message that the person is an adult.
//• If the person is age 65 or older, print a message that the person is an elder.

//Solution:
var age = 30;
if (age < 2) {
    console.log("The person is a baby.");
} else if (age >= 2 && age < 4) {
    console.log("The person is a toddler.");
} else if (age >= 4 && age < 13) {
    console.log("The person is a kid.");
} else if (age >= 13 && age < 20) {
    console.log("The person is a teenager.");
} else if (age >= 20 && age < 65) {
    console.log("The person is an adult.");
} else {
    console.log("The person is an elder.");
}

//Qno:29Favorite Fruit: Make a array of your favorite fruits, and then write a series of independent if statements that check for certain fruits in your array.
//• Make a array of your three favorite fruits and call it favorite_fruits.
//• Write five if statements. Each should check whether a certain kind of fruit is in your array. If the fruit is in your array, the if block should print a statement, such as You really like bananas!

//Solution:
var favorite_fruits = ["banana", "apple", "strawberry"];
if (favorite_fruits.includes("banana")) {
    console.log("You really like bananas!");
}
if (favorite_fruits.includes("apple")) {
    console.log("You really like apples!");
}
if (favorite_fruits.includes("strawberry")) {
    console.log("You really like strawberries!");
}
if (favorite_fruits.includes("orange")) {
    console.log("You really like oranges!");
}
if (favorite_fruits.includes("grape")) {
    console.log("You really like grapes!");
}

//Qno:30 Hello Admin: Make a array of five or more usernames, including the name 'admin'. Imagine you are writing code that will print a greeting to each user after they log in to a website. Loop through the array, and print a greeting to each user:
//• If the username is 'admin', print a special greeting, such as Hello admin, would you like to see a status report?
//• Otherwise, print a generic greeting, such as Hello Eric, thank you for logging in again.

//Solution:
var usernames = ["taha", "ali", "ahmed", "anas", "sarah"];
for (var i = 0; i < usernames.length; i++) {
    if (usernames[i] === "admin") {
        console.log("Hello admin, would you like to see a status report?");
    } else {
        console.log("Hello " + usernames[i] + ", thank you for logging in again.");
    }
}

//Qno:31 No Users: Add an if test to Exercise 28 to make sure the list of users is not empty.
//• If the list is empty, print the message We need to find some users!
//• Remove all of the usernames from your array, and make sure the correct message is printed.

//Solution:
var usernames = ["taha", "ali", "ahmed", "anas", "sarah"];
if (usernames.length > 0) {
    for (var i = 0; i < usernames.length; i++) {
        if (usernames[i] === "admin") {
            console.log("Hello admin, would you like to see a status report?");
        } else {
            console.log("Hello " + usernames[i] + ", thank you for logging in again.");
        }
    }
} else {
    console.log("We need to find some users!");
}

//Qno:32Checking Usernames: Do the following to create a program that simulates how websites ensure that everyone has a unique username.
//• Make a list of five or more usernames called current_users.
//• Make another list of five usernames called new_users. Make sure one or two of the new usernames are also in the current_users list.
//• Loop through the new_users list to see if each new username has already been used. If it has, print a message that the person will need to enter a new username. If a username has not been used, print a message saying that the username is available.
//• Make sure your comparison is case insensitive. If 'John' has been used, 'JOHN' should not be accepted.

//Solution:
var current_users = ["ali", "maida", "eric", "hamza", "ahmed"];
var new_users = ["nehal", "taha", "fabiha", "sarah", "hania"];
for (var i = 0; i < new_users.length; i++) {
    var lowercase_new_username = new_users[i].toLowerCase();
    if (current_users.includes(lowercase_new_username)) {
        console.log("Sorry, the username '" + new_users[i] + "' is not available. Please enter a new username.");
    } else {
        console.log("Congratulations! The username '" + new_users[i] + "' is available.");
    }
}

//Qno:33 Ordinal Numbers: Ordinal numbers indicate their position in a array, such as 1st or 2nd. Most ordinal numbers end in th, except 1, 2, and 3.
//• Store the numbers 1 through 9 in a array.
//• Loop through the array.
//• Use an if-else chain inside the loop to print the proper ordinal ending for each number. Your output should read "1st 2nd 3rd 4th 5th 6th 7th 8th 9th", and each result should be on a separate line.

//Solution:
var numbers = [1, 2, 3, 4, 5, 6, 7, 8, 9];
for (var i = 0; i < numbers.length; i++) {
    var number = numbers[i];
    if (number === 1) {
        console.log(number + "st");
    } else if (number === 2) {
        console.log(number + "nd");
    } else if (number === 3) {
        console.log(number + "rd");
    } else {
        console.log(number + "th");
    }
}

//Qno:34  Pizzas: Think of at least three kinds of your favorite pizza. Store these pizza names in a array, and then use a for loop to print the name of each pizza.
//• Modify your for loop to print a sentence using the name of the pizza instead of printing just the name of the pizza. For each pizza you should have one line of output containing a simple statement like I like pepperoni pizza.
//• Add a line at the end of your program, outside the for loop, that states how much you like pizza. The output should consist of three or more lines about the kinds of pizza you like and then an additional sentence, such as I really love pizza!

//Solution:
var pizzas = ["pepperoni", "fajita", "tikka"];
for (var i = 0; i < pizzas.length; i++) {
    console.log("I like " + pizzas[i] + " pizza.");
}
console.log("Pizza is one of my favorite foods! I really love pizza!");

//Qno:35 Animals: Think of at least three different animals that have a common characteristic. Store the names of these animals in a list, and then use a for loop to print out the name of each animal. • Modify your program to print a statement about each animal, such as A dog would make a great pet. • Add a line at the end of your program stating what these animals have in common. You could print a sentence such as Any of these animals would make a great pet!

//Solution:
var animals = ["dog", "cat", "cow"];
for (var i = 0; i < animals.length; i++) {
    console.log("A " + animals[i] + " would make a great pet.");
}
console.log("Any of these animals would make a great pet!");

//Qno:36 T-Shirt: Write a function called make_shirt() that accepts a size and the text of a message that should be printed on the shirt. The function should print a sentence summarizing the size of the shirt and the message printed on it. Call the function.
//Solution:
function make_shirt(size, message) {
    console.log("The shirt size is " + size + " and the message printed on it is: '" + message + "'.");
}
make_shirt("large", "Hello, World!");

//Qno:37 Large Shirts: Modify the make_shirt() function so that shirts are large by default with a message that reads I love TypeScript. Make a large shirt and a medium shirt with the default message, and a shirt of any size with a different message.
//Solution:
function make_shirt(size = "large", message = "I love TypeScript") {
    console.log("The shirt size is " + size + " and the message printed on it is: '" + message + "'.");
}
make_shirt();
make_shirt("medium");
make_shirt("small", "Hello, JavaScript!"); 

//Qno:38  Cities: Write a function called describe_city() that accepts the name of a city and its country. The function should print a simple sentence, such as Karachi is in Pakistan. Give the parameter for the country a default value. Call your function for three different cities, at least one of which is not in the default country.
//Solution:
function describe_city(city, country = "Unknown") {
    console.log(city + " is in " + country + ".");
}
describe_city("Karachi", "Pakistan");
describe_city("New York", "USA");
describe_city("Lahore");

//Qno:39 City Names: Write a function called city_country() that takes in the name of a city and its country. The function should return a string formatted like this:
//"Lahore, Pakistan"
//Call your function with at least three city-country pairs, and print the value that’s returned.

//Solution:
function city_country(city, country) {
    return city + ", " + country;
}
var city1 = city_country("Lahore", "Pakistan");
var city2 = city_country("Tokyo", "Japan");
var city3 = city_country("Sundey", "Australia");
console.log(city1);
console.log(city2);
console.log(city3);

//Qno:40 Album: Write a function called make_album() that builds a Object describing a music album. The function should take in an artist name and an album title, and it should return a Object containing these two pieces of information. Use the function to make three dictionaries representing different albums. Print each return value to show that Objects are storing the album information correctly. Add an optional parameter to make_album() that allows you to store the number of tracks on an album. If the calling line includes a value for the number of tracks, add that value to the album’s Object. Make at least one new function call that includes the number of tracks on an album.
//Solution:
function make_album(artist, title, tracks) {
    var album = {
        artist: artist,
        title: title
    };
    if (tracks) {
        album.tracks = tracks;
    }
    return album;
}
var album1 = make_album("Artist1", "Album1");
var album2 = make_album("Artist2", "Album2", 12);
var album3 = make_album("Artist3", "Album3");
console.log(album1);
console.log(album2);
console.log(album3);

//QNO:41 Magicians: Make a array of magician’s names. Pass the array to a function called show_magicians(), which prints the name of each magician in the array.
//Solution:
function show_magicians(magicians) {

    for (var i = 0; i < magicians.length; i++) {
        console.log(magicians[i]);
    }
}
var pakistani_magicians = ["Ahmed Ali", "Zahid Ali", "Ali Raza", "Hassan Ali"]
show_magicians(pakistani_magicians);

//Qno:42Great Magicians: Start with a copy of your program from Exercise 39. Write a function called make_great() that modifies the array of magicians by adding the phrase the Great to each magician’s name. Call show_magicians() to see that the list has actually been modified.
//Solution:
let magicians = ["Haseeb Ahmed", "Ali Raza", "Sara Khan", "Ahmed Hassan"];
function makeGreat(magiciansArray) {
    for (let i = 0; i < magiciansArray.length; i++) {
        magiciansArray[i] = "the Great " + magiciansArray[i];
    }}
function showMagicians(magiciansArray) {
    console.log("List of Pakistani Magicians:");
    magiciansArray.forEach(magician => console.log("- " + magician));
}
makeGreat(magicians);
showMagicians(magicians);



//Qno:43 Unchanged Magicians: Start with your work from Exercise 40. Call the function make_great() with a copy of the array of magicians’ names. Because the original array will be unchanged, return the new array and store it in a separate array. Call show_magicians() with each array to show that you have one array of the original names and one array with the Great added to each magician’s name.
//Solution:
//Qno:44 Sandwiches: Write a function that accepts a array of items a person wants on a sandwich. The function should have one parameter that collects as many items as the function call provides, and it should print a summary of the sandwich that is being ordered. Call the function three times, using a different number of arguments each time.
//Solutions;
function makeSandwich(...ingredients) {
    console.log("Preparing a  sandwich with the following ingredients:");
    if (ingredients.length === 0) {
        console.log("  - No ingredients provided. Please specify some ingredients for your sandwich.");
    } else {
        ingredients.forEach((ingredient, index) => {
            console.log(`  ${index + 1}. ${ingredient}`);
        });
    }
}
makeSandwich("Chicken", "Cucumber", "Tomato", "Lettuce", "Mayonnaise");
makeSandwich("Beef", "Onion", "Cheese");
makeSandwich("Egg", "Potato");


//Qno:45 Cars: Write a function that stores information about a car in a Object. The function should always receive a manufacturer and a model name. It should then accept an arbitrary number of keyword arguments. Call the function with the required information and two other name-value pairs, such as a color or an optional feature. Print the Object that’s returned to make sure all the information was stored correctly.
//Solution:
function createCar(manufacturer, modelName, ...otherInfo) {
    let car = {
        manufacturer: manufacturer,
        modelName: modelName
    };
    for (let i = 0; i < otherInfo.length; i += 2) {
        const key = otherInfo[i];
        const value = otherInfo[i + 1];
        car[key] = value;
    }
    return car;
}
const myCar = createCar('Toyota', 'Camry', 'color', 'blue', 'year', 2022);
console.log(myCar);
