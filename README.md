# 45-Que-Project-Code

                        //Que # 02
// Print a personalized message
console.log(`Hello ${personName}, would you like to learn some TypeScript and Node.js today?`);


                       //Que # 03
// Store the person's name in a variable
const personName02: string = "John Doe";

// Convert name to lowercase
const lowercaseName: string = personName02.toLowerCase();

// Convert name to uppercase
const uppercaseName: string = personName02.toUpperCase();

// Convert name to titlecase
const titlecaseName: string = personName02.replace(/\w\S*/g, function(txt) {
    return txt.charAt(0).toUpperCase() + txt.substr(1).toLowerCase();
});

// Print the names
console.log("Lowercase:", lowercaseName);
console.log("Uppercase:", uppercaseName);
console.log("Titlecase:", titlecaseName);


                      //Que # 04
// Define the quote and its author
const quote: string = "A person who never made a mistake never tried anything new.";
const author: string = "Albert Einstein";

// Print the quote and its author
console.log(`"${quote}" - ${author}`);


                      //Que # 05
// Store the famous person's name in a variable
const famousPerson: string = "Albert Einstein";

// Define the quote
const quote01: string = "Imagination is more important than knowledge.";

// Compose the message
const message: string = `"${quote01}" - ${famousPerson}`;

// Print the message
console.log(message);


                       //Que # 06
// Store the person's name with whitespace characters
const personNameWithWhitespace: string = "\t\n   John Doe   \t\n";

// Print the name with whitespace
console.log("Name with whitespace:", personNameWithWhitespace);

// Strip the whitespace from the name
const strippedName: string = personNameWithWhitespace.trim();

// Print the stripped name
console.log("Stripped name:", strippedName);


                        //Que # 07 & 08
console.log(5 + 3); // Addition: 5 + 3 = 8
console.log(10 - 2); // Subtraction: 10 - 2 = 8
console.log(4 * 2); // Multiplication: 4 * 2 = 8
console.log(16 / 2); // Division: 16 / 2 = 8


                        //Que # 09
// Store your favorite number in a variable
const favoriteNumber: number = 42;

// Create a message revealing your favorite number
const message01: string = `My favorite number is ${favoriteNumber}.`;

// Print the message
console.log(message01);


                        //Que # 10
// Program to demonstrate basic arithmetic operations resulting in the number 8
console.log(5 + 3); // Addition: 5 + 3 = 8
console.log(10 - 2); // Subtraction: 10 - 2 = 8
console.log(4 * 2); // Multiplication: 4 * 2 = 8
console.log(16 / 2); // Division: 16 / 2 = 8


                        //Que # 11
// Store the names of friends in an array
const names: string[] = ["Aliyan", "Fahad", "Abdullah", "Ahmed"];

// Print each person's name
for (const name of names) {
    console.log(name);
}


                         //Que # 12
// Store the names of friends in an array
const namess: string[] = ["Aliyan", "Fahad", "Abdullah", "Ahmed"];

// Print a personalized message to each person
for (const name of namess) {
    console.log(`Hello ${name}, I hope you're doing well!`);
}

                           //Que # 13
// Store examples of favorite mode of transportation in an array
const transportation: string[] = ["motorcycle", "car", "bicycle", "boat"];

// Print statements about these items
for (const item of transportation) {
    console.log(`I would like to own a ${item}.`);
}

                           //Que # 14
// Initial guest list
const guestList: string[] = ["Albert Einstein", "Leonardo da Vinci", "Marie Curie"];

// Print invitation messages
for (const guest of guestList) {
    console.log(`Dear ${guest}, you are cordially invited to dinner. Please join us.`);
}

                           //Que # 15
// Initial guest list
const guestList02: string[] = ["Albert Einstein", "Leonardo da Vinci", "Marie Curie"];

// Print invitation messages
for (const guest of guestList02) {
    console.log(`Dear ${guest}, you are cordially invited to dinner. Please join us.`);
}

// Name of the guest who can't make it
const unableToAttend: string = "Leonardo da Vinci";
console.log(`${unableToAttend} regrets that they can't make it to the dinner.`);

// Replace the guest who can't make it with a new guest
const replacementGuest: string = "Nikola Tesla";
const indexOfUnableToAttend: number = guestList02.indexOf(unableToAttend);
if (indexOfUnableToAttend !== -1) {
    guestList02[indexOfUnableToAttend] = replacementGuest;
}

// Print invitation messages again with updated guest list
for (const guest of guestList02) {
    console.log(`Dear ${guest}, you are cordially invited to dinner. Please join us.`);
}

                            //Que # 16
// Initial guest list
let guestList03: string[] = ["Albert Einstein", "Leonardo da Vinci", "Marie Curie", "Isaac Newton", "Galileo Galilei", "Nikola Tesla"];

// Inform about the bigger dinner table
console.log("Good news! We found a bigger dinner table.");

// Add one new guest to the beginning of the array
guestList03.unshift("Ada Lovelace");

// Add one new guest to the middle of the array
const middleIndex: number = Math.floor(guestList03.length / 2);
guestList03.splice(middleIndex, 0, "Charles Darwin");

// Add one new guest to the end of the array
guestList03.push("Stephen Hawking");

// Print a new set of invitation messages
for (const guest of guestList03) {
    console.log(`Dear ${guest}, you are cordially invited to dinner. Please join us.`);
}

                             //Que # 17
// Print a message indicating only two people can be invited for dinner
console.log("Unfortunately, we can only invite two people for dinner.");

// Remove guests from the list until only two names remain
while (guestList.length > 2) {
    const removedGuest: string = guestList.pop()!;
    console.log(`Sorry ${removedGuest}, we can't invite you to dinner.`);
}

// Print invitation messages to the two remaining guests
for (const guest of guestList) {
    console.log(`Dear ${guest}, you are still invited to dinner.`);
}

// Remove the last two names from the list
guestList.splice(-2);

// Print the empty list
console.log("Guest list:", guestList);


// Print the empty list
console.log("Guest list:", guestList);


                             //Que # 18
// Array of places to visit
let placesToVisit: string[] = ["Japan", "Italy", "Australia", "Iceland", "Brazil"];

// Print array in its original order
console.log("Original order:", placesToVisit);

// Print array in alphabetical order without modifying the original list
console.log("Alphabetical order:", [...placesToVisit].sort());

// Show that the array is still in its original order
console.log("Original order:", placesToVisit);

// Print array in reverse alphabetical order without changing the original list
console.log("Reverse alphabetical order:", [...placesToVisit].sort().reverse());

// Show that the array is still in its original order
console.log("Original order:", placesToVisit);

// Reverse the order of the list
placesToVisit.reverse();

// Print the array to show its order has changed
console.log("Reversed order:", placesToVisit);

// Reverse the order of the list again
placesToVisit.reverse();

// Print the list to show it's back to its original order
console.log("Original order:", placesToVisit);

// Sort the array in alphabetical order
placesToVisit.sort();

// Print the array to show its order has been changed
console.log("Sorted in alphabetical order:", placesToVisit);

// Sort the array in reverse alphabetical order
placesToVisit.sort((a, b) => b.localeCompare(a));

// Print the array to show its order has been changed
console.log("Sorted in reverse alphabetical order:", placesToVisit);


                                     //Que # 19
// Print the number of people invited to dinner
console.log(`Number of people invited to dinner: ${guestList.length}`);


                                     //Que # 20
// Array of mountains
const mountains: string[] = ["Mount Everest", "K2", "Nagaperbhat", "Lhotse"];


                                    //Que # 21
// Object containing programming languages
const languages: { [key: string]: string } = {
    "JavaScript": "High-level, interpreted programming language",
    "Python": "Interpreted, high-level, general-purpose programming language",
    "TypeScript": "Typed superset of JavaScript that compiles to plain JavaScript"
};

                                     //Que # 22
// Example of an intentional error
let array = [1, 2, 3];
console.log(array[3]); // Accessing an index that doesn't exist in the array


                                      //Que # 23
let car = 'Mastang';

console.log("Is car == 'subaru'? I predict True.");
console.log(car == 'Mastang');

console.log("Is car == 'audi'? I predict False.");
console.log(car == 'audi');

// Add more conditional tests here...


                                       //Que # 24
let string1 = 'hello';
let string2 = 'world';

console.log("Are the strings equal? I predict False.");
console.log(string1 == string2);

console.log("Is the first string shorter than the second? I predict True.");
console.log(string1.length < string2.length);

// Add more conditional tests here...


                                        //Que # 25
// Variable representing the color of the alien
let alien_color: string = 'green';

// Check if the alien's color is green and award points accordingly
if (alien_color === 'green') {
    console.log("The player just earned 5 points.");
}


                                        //Que # 26
// Choose a color for the alien
let alien_color01: string = 'red';

// If-else chain to award points based on the alien's color
if (alien_color01 === 'green') {
    console.log("The player just earned 5 points for shooting the alien.");
} else {
    console.log("The player just earned 10 points.");
}

                                        //Que # 27
// Choose a color for the alien
let alien_color03: string = 'yellow';

// If-else chain to award points based on the alien's color
if (alien_color03 === 'green') {
    console.log("The player earned 5 points.");
} else if (alien_color03 === 'yellow') {
    console.log("The player earned 10 points.");
} else if (alien_color03 === 'red') {
    console.log("The player earned 15 points.");
}

                                        //Que # 28
// Set the age of the person
let age: number = 30;

// Determine the stage of life based on age
if (age < 2) {
    console.log("The person is a baby.");
} else if (age < 4) {
    console.log("The person is a toddler.");
} else if (age < 13) {
    console.log("The person is a kid.");
} else if (age < 20) {
    console.log("The person is a teenager.");
} else if (age < 65) {
    console.log("The person is an adult.");
} else {
    console.log("The person is an elder.");
}

                                         //Que # 29
// Array of favorite fruits
const favorite_fruits: string[] = ["banana", "apple", "mango"];

// Check if certain fruits are in the array
if (favorite_fruits.includes("banana")) {
    console.log("You really like bananas!");
}

                                          //Que # 30
// Array of usernames
const usernames: string[] = ["admin", "user1", "user2", "user3", "user4"];

// Greet each user after logging in
for (const username of usernames) {
    if (username === "admin") {
        console.log("Hello admin, would you like to see a status report?");
    } else {
        console.log(`Hello ${username}, thank you for logging in again.`);
    }
}

                                          //Que # 31
// Check if the list of users is empty
if (usernames.length === 0) {
    console.log("We need to find some users!");
}

                                           //Que # 32
// List of current usernames
const current_users: string[] = ["user1", "user2", "user3", "user4", "user5"];

// List of new usernames
const new_users: string[] = ["user2", "user3", "user6", "user7", "user8"];

// Loop through new_users list to check for uniqueness
for (const new_user of new_users) {
    const is_taken: boolean = current_users.some(user => user.toLowerCase() === new_user.toLowerCase());
    if (is_taken) {
        console.log(`The username ${new_user} is already taken. Please enter a new username.`);
    } else {
        console.log(`The username ${new_user} is available.`);
    }
}

                                           //Que # 33
// Array of numbers
const numbers: number[] = [1, 2, 3, 4, 5, 6, 7, 8, 9];

// Loop through the array and print ordinal numbers
for (const number of numbers) {
    let ordinal: string;
    if (number === 1) {
        ordinal = "st";
    } else if (number === 2) {
        ordinal = "nd";
    } else if (number === 3) {
        ordinal = "rd";
    } else {
        ordinal = "th";
    }
    console.log(`${number}${ordinal}`);
}

                                           //Que # 34
// Array of favorite pizza types
const pizzas: string[] = ["Pepperoni", "Margherita", "Vegetarian"];

// Loop through the array and print a sentence for each pizza
for (const pizza of pizzas) {
    console.log(`I like ${pizza} pizza.`);
}

// Print additional sentence
console.log("I really love pizza!");


                                           //Que # 35
// Array of animals
const animals: string[] = ["Dog", "Cat", "Bird"];

// Loop through the array and print a statement about each animal
for (const animal of animals) {
    console.log(`A ${animal.toLowerCase()} would make a great pet.`);
}

// Print additional sentence
console.log("Any of these animals would make a great pet!");


                                           //Que # 36
// Function to make a shirt
function make_shirt(size: string, message: string): void {
    console.log(`Size: ${size}, Message: ${message}`);
}

// Call the function
make_shirt("Large", "I love TypeScript");


                                           //Que # 37
// Function to make a shirt with default values
function make_shirt01(size: string = "Large", message: string = "I love TypeScript"): void {
    console.log(`Size: ${size}, Message: ${message}`);
}

// Call the function
make_shirt01(); // Large shirt with default message
make_shirt01("Medium"); // Medium shirt with default message
make_shirt("Small", "Hello, World!"); // Small shirt with custom message


                                           //Que # 38
// Function to describe a city
function describe_city(city: string, country: string = "Pakistan"): void {
    console.log(`${city} is in ${country}.`);
}

// Call the function for three different cities
describe_city("Karachi");
describe_city("Lahore");
describe_city("New York", "USA");


                                          //Que # 39
// Function to format city and country
function city_country(city: string, country: string): string {
    return `${city}, ${country}`;
}

// Call the function with city-country pairs
console.log(city_country("Lahore", "Pakistan"));
console.log(city_country("Paris", "France"));
console.log(city_country("Tokyo", "Japan"));


                                          //Que # 40
// Function to create an album
function make_album(artist: string, title: string, tracks?: number): { artist: string, title: string, tracks?: number } {
    const album: { artist: string, title: string, tracks?: number } = { artist, title };
    if (tracks) {
        album.tracks = tracks;
    }
    return album;
}

// Call the function for three different albums
console.log(make_album("Ed Sheeran", "Divide", 12));
console.log(make_album("Taylor Swift", "1989"));
console.log(make_album("Adele", "25", 11));


                                          //Que # 41
// Function to show magicians
function show_magicians(magicians: string[]): void {
    for (const magician of magicians) {
        console.log(magician);
    }
}

// Array of magician names
const magicians: string[] = ["David Copperfield", "Harry Houdini", "Penn & Teller"];

// Call the function
show_magicians(magicians);


                                           //Que # 42
// Function to make magicians great
function make_great(magicians: string[]): string[] {
    const great_magicians: string[] = [];
    for (const magician of magicians) {
        great_magicians.push(`the Great ${magician}`);
    }
    return great_magicians;
}

// Call the function and store the modified list
const great_magicians: string[] = make_great(magicians);

// Call the show_magicians function to see the modified list
show_magicians(great_magicians);


                                            //Que # 43
// Call the function with a copy of the original array
const modified_magicians: string[] = make_great([...magicians]);

// Call the show_magicians function with both arrays
show_magicians(magicians);
show_magicians(modified_magicians);


                                             //Que # 44
// Function to summarize a sandwich order
function make_sandwich(...items: string[]): void {
    console.log("Sandwich order:");
    for (const item of items) {
        console.log(`- ${item}`);
    }
}

// Call the function with different numbers of arguments
make_sandwich("Ham", "Cheese");
make_sandwich("Turkey", "Lettuce", "Tomato");
make_sandwich("Peanut Butter", "Jelly");


                                             //Que # 45
// Function to store car information in an object
function store_car(manufacturer: string, model: string, ...features: string[]): { manufacturer: string, model: string, [key: string]: string } {
    const car: { manufacturer: string, model: string, [key: string]: string } = { manufacturer, model };
    for (let i = 0; i < features.length; i += 2) {
        car[features[i]] = features[i + 1];
    }
    return car;
}

// Call the function
console.log(store_car("Toyota", "Corolla", "Color", "Red", "Year", "2022"));


                                   //                    THE END                  //
