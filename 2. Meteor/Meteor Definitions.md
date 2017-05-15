<h1>Meteor Definitions</h1>

<b>#1: Meteor (JavaScript Framework):</b>
There is a lot to love about the Meteor JavaScript Framework: (1) With nothing but JavaScript, you’re able to build modern, real-time web applications for both desktop and mobile platforms. (2) Beginning developers can quickly build something impressive and useful, while more advanced developers can appreciate Meteor’s flexibility. (3) There’s an active community that organizes meetups, publishes free training material (like this book), and offers help wherever possible.
Meteor adds the html tags to the beginning and end of the file, and it automatically includes any resources contained within the project’s folder (like JavaScript and CSS files).
This isn’t the most remarkable feature in the world, but one of Meteor’s core philosophies is
developer happiness, so there’s plenty of time-saving features like this spread throughout the
framework.

<b>#2: Command Line (CLI):</b>
"The command line is a text interface for your computer. It's a program that takes in commands, which it passes on to the computer's operating system to run."
These days, command line interfaces as they’re known — or “CLI” for short — are still used by
software developers. To install the Meteor framework on our computers, and then interact with that software, we have to work with the command line.

<b>#3: Leaderboard:</b>
Leaderboard is an example application that was designed by the Meteor Development Group to show off what Meteor could do with very few lines of code. Leaderboard has since been replaced by more advanced examples on the official website, but it is our example project for two main reasons:
First, the application already exists. It’s something we can play with, and that means we can get a good idea of what we’re trying to build before we write a single line of code.
Second, the application is simple. This means we don’t have to worry about the conceptual aspect of building the software (which is usually the most difficult part). Instead, we can focus on learning Meteor itself.
To get hands-on time with Leaderboard, visit leaderboard2.meteor.com and, while
clicking
around, take note of its core features: • There’s a list of players.
• Each player has a score.conceptual aspect of building the software (which is usually the most difficult part). Instead, we can focus on learning Meteor itself.
To get hands-on time with Leaderboard, visit leaderboard2.meteor.com and, while
 clicking
around, take note of its core features:
• There’s a list of players.
• Each player has a score.
• Players are ranked by their score.
• You can select players by clicking on them.
• You can increment a selected player’s score.
The central feature of the Leaderboard application is the list of players. Without the list of players
appearing inside the interface, we can’t build anything else of value.

<b>#4: Project:</b>
To create our first Meteor application, we’ll need to create our first project, and a project is the
self-contained set of files that form the foundation of an application. You can use the words
“project” and “application” interchangeably, but “project” is better-suited when talking about
the application as it’s being developed.
Every project is different, but will generally contain:
• HTML files, to create the interface.
• CSS files, to assign styles to the interface.
• JavaScript files, to define application logic.
• Folders, to keep everything organized.
A project can contain other types of files, like images and CoffeeScript files, but we’ll keep things
as simple as possible throughout this book and only work with what we need.

<b>#5: HTML (Files):</b>
HTML files create the interface.

<b>#6: CSS (Files):</b>
CSS files assign styles to the interface.

<b>#7: JavaScript (Files):</b>
JavaScript files define application logic.

<b>#8: Folders:</b>
Folders keep everything organized. Before we create a project for the Leaderboard application though, let’s create a folder to store our Meteor projects. We don’t have to do this, but it’s a good idea for the sake of keeping things organized.

<b>#9:</b>
mkdir Meteor (make directory): To create a new folder, we could select the “New
Folder” option from the “File” menu, but where’s the fun in that? Instead, enter the following into the command line:
mkdir Meteor
Then tap the “Return” key.
This mkdir command stands for “make directory” and it allows us to make a directory. In this particular instance, we’re creating a directory named “Meteor”, but you can call the folder whatever you want. The precise location where the folder will appear will depend on your operating system, but at least on Mac OS X, the folder will appear inside the “Home” directory by default.

<b>#10:</b>
cd Meteor (choose directory): To navigate to a directory that you have created (by using the mkdir Meteor command), type the following command into the command line:
cd Meteor
This cd command stands for “change directory” and it’s the command line equivalent of double-clicking on a directory from within the graphical interface, so after tapping the “Return” key, we’ll be inside the “Meteor” directory.

<b>#11: meteor create ___ (leaderboard):</b>
To create a Meteor project inside a directory (the one you made using mkdir Meteor), type the following command into the command line:
meteor create ___ (leaderboard)
This command has three parts:
• The meteor part defines this as a Meteor command.
• The create part clarifies that we want to create a Meteor project.
• The leaderboard part is the name we’re assigning to the project.
After running this command, a “leaderboard” directory will appear inside the “Meteor” folder, and by default this folder will contain three files:
• leaderboard.html
• leaderboard.css
• leaderboard.js

<b>#12: .Meteor:</b>
A hidden file folder.

<b>#13: Local Server:</b>
To get the web application working as planned, we need to launch what’s known as a local server. This is a web server that runs on our local machine. It’s included with Meteor itself and allows
us to:
 2. Run a database on our local machine.
To continually see the results of our code, we’ll need to keep the local server running. This simply
1. See the processed results of our JavaScript code.
what’s known as a local server. This is a web server that runs on our local machine. 1. See the processed results of our JavaScript code.
It’s included with Meteor itself and allows us to:
 2. Run a database on our local machine.
To continually see the results of our code, we’ll need to keep the local server running. This simply
means leaving the command line open from this point onward. You will, however, need to open
a separate tab or window to write further commands.
To stop the local server, either quit out of the command line, or with the command line in focus, press CTRL + C on your keyboard.

<b>#14: meteor run:</b>
Once you are in the application directory (so "leaderboard" in this case), type the following command into the command line:
meteor run
Here, the meteor part defines this as a Meteor command and the run part clarifies the precise action we want to take. In this context, we’re wanting to run the local server.
Make sure you’re inside a project’s folder before running the command.

<b>#15: http://localhost:3000/:</b>
After tapping the “Return” key (after typing in "meteor run" into the command line), the following should appear:
=> Started proxy.
=> Started MongoDB.
=> Started your app.
=> App running at: http://localhost:3000/
These lines confirm that the local server is starting and the URL on the last line — http://localhost:3000
— is what we can now use to view our Meteor project in a web browser.
Navigate to this URL from inside Chrome and notice that we’re no longer seeing static text.
Instead, we’re seeing a functional web application. The application itself is the result of the code
that’s included with every Meteor project by default.

<b>#16: JavaScript Console:</b>
"Type the following into the JavaScript file: console.log("Hello world");
Then save the file and open the JavaScript Console from inside Chrome: 1. Click on the View menu.
2. Hover over the Developer option.
3. Select the JavaScript Console option.
   Once that’s done, a pane will open at the bottom of the browser and display the “Hello world” text that we just
passed through the console.log statement.
We can also use the Console to manipulate our application’s database.
1. Click on the View menu.
2. Hover over the Developer option.
3. Select the JavaScript Console option.
 Once that’s done, a pane will open at the bottom of the browser and display the “Hello world” text that we just
passed through the console.log statement.
We can also use the Console to manipulate our application’s database.

<b>#17: 'console.log' Statements:</b>
console.log statements are used to see the output of code without creating an interface to display that output. This means that, before we invest time into creating an interface, we can:
1. Confirm that our code is working as expected.
2. Fix any bugs as soon as they appear.

<b>#18: Front-End (Interface):</b>
For our Leaderboard application, without the list of players
appearing inside the interface, we can’t build anything else of value

<b>#19: Database (Back-End):</b>
If you’ve built something on the web before, you’ve probably come into contact with some kind of database. Maybe you’ve installed a copy of WordPress, or used phpMyAdmin, or even built
some software with a language like PHP. In these cases, you would have come into contact with an SQL database.
By default, every Meteor project comes with its own database. There’s no setup or configuration required. Whenever you create a project, a database is automatically created for that project, and whenever the local server is running, so is that database. This database, however, is not an SQL database. Instead, it’s what’s known as a MongoDB database.
For the moment, you only need to know two things:
First, there’s no other type of database available for Meteor. If you’d like to use an SQL database, for instance, it’s just not possible yet. Other options will be available in the future, but
the time-line isn’t clear.
Second, Mongo uses different words to describe familiar concepts. We won’t, for instance,
use words like “tables” and “rows”, but the concepts are basically the same. You can see the
differences in a table (See I#3 in "Images from the Book").

<b>#21: SQL Database:</b>
Maybe you’ve installed a copy of WordPress, or used
phpMyAdmin, or even built
some software with a language like PHP. In these cases, you would have come into contact with an SQL database.

<b>#22: Collection:</b>
Here’s two questions to consider:
• Where do we store the data associated with each player?
• How do we display this data from within the interface?
The facetious answer would be “in a database”, but the more useful answer would be “in a
collection”. A collection is equivalent to an SQL table.
To illustrate the purpose of a collection, imagine we’re creating our own version of WordPress
with Meteor. If that were the case, we’d create a collection for the posts, a collection for the
comments, and a collection for the pages. We’d create a collection for each type of data. For our Leaderboard application, we’ll create a collection for the players.

<b>#23: new Mongo.Collection('players'):</b>
To create a Collection of players, open the JavaScript file and write the following statement:
new Mongo.Collection('players');
Here, we’re creating a collection named “players” inside our project’s Mongo database. You can
name the collection whatever you want, but it must be unique. If the name is not unique, Meteor
will return an error.
To confirm that a collection exists, save the file, switch to Chrome, and enter the name of the
collection’s variable into the Console:
PlayersList
This should show that the collection is working as expected (unless you got an error due to typing or something else).

<b>#24: PlayersList = new Mongo.Collection('players'):</b>
Despite this line of code ("new Mongo.Collection('players')") though, we haven’t defined a way for us to reference this collection, and therefore we have no way of manipulating it.
    PlayersList = new Mongo.Collection('players');
But notice that we didn’t use the var keyword, and that’s because we want to create a global
To fix this, place the collection inside a variable:
  defined a way for us to reference this collection, and therefore we have no way of manipulating it.
 PlayersList = new Mongo.Collection('players');
But notice that we didn’t use the var keyword, and that’s because we want to create a global
variable.

<b>#25: Global Variable:</b>
A variable (without the "var" keyword) that allows us to reference and manipulate a collection throughout all of our project’s files.

<b>#26: Inserting Data:</b>
When we want to insert data into a collection, we have four options. (1) We can insert data through the JavaScript Console, (2) through the command line, (3) through the JavaScript file, (4) and through a
form in the interface. The first option — through the JavaScript Console — is the simplest.
Inside the Console, write the following:
PlayersList.insert();
This is the syntax we use to manipulate a collection.
We start with the variable assigned to the collection — the “PlayersList” variable — and then
attach a function to it. In this case, we’re using the insert function.
If we tapped the “Return” key at this point, nothing would happen, and that’s because we
need to pass data between the brackets of the function for it to actually change the contents of
the collection.
The data we pass through needs to be in the JSON format, and if you’re not familiar with the
JSON format, this is what it looks like:
{
name: "David",
score: 0 }
We can pass this data through the brackets, like so:
PlayersList.insert({ name: "David",
score: 0 });
This is a complete insert function, and if we type this statement into the Console and tap the
“Return” key, a document will be created inside the “PlayersList” collection. We want to create one document for every player we want in our collection. So if we want our leaderboard to contain six players, we’ll need to use
To fix this, place the collection inside a variable:
the insert function six times, thereby creating six documents.
});
This is a complete insert function, and if we type this statement into the Console and tap the
 “Return” key, a document will be created inside the “PlayersList” collection. We want to create one document for every player we want in our collection. So if we want our leaderboard to contain six players, we’ll need to use
the insert function six times, thereby creating six documents.
To achieve this, repeat this statement a few times, making sure to define unique values for the name field so we can distinguish the players:
PlayersList.insert({
name: "Bob",
score: 0 });
Since white-space is ignored though, the statement can be written on one line:
PlayersList.insert({ name: "Bob", score: 0 });
(To see the definition of (a) "Document", see below/#28.)

<b>#27: JSON Format:</b>
The data we pass through to a collection needs to be in the JSON format, and if you’re not familiar with the JSON format, this is what it looks like:
{
name: "David",
score: 0 }
Here, there’s a few things going on:
First, the data is wrapped in a pair of curly braces. This is how we distinguish our JSON data
from the rest of the code.
Second, we’ve defined a pair of keys. These keys are known as name and score, and in Mongo
terminology, these are the fields for our collection. So because every player in the collection will
have a name and a score, we have the name and score fields to hold these values. Third, we’ve defined the values associated with our keys. In this case, the value of the name
field is “David” and the value of the score field is 0.
Fourth, the key-value pairs are separated with commas. This is because the JSON format
ignores white-space, so commas are required to provide structure.

<b>#28: Keys:</b>
Keys (like "name" and "score" above in #27), and in Mongo terminology, these are the fields for our collection. There are values associated with our keys, like
(in the code above in #27) the "name" field being “David” and the value of the "score" field being 0. The key-value pairs are separated with commas to provide structure (and because the JSON format ignores white-space).
We can also click on the downward-facing arrows to see the data associated with each document,
including:
• The _id field, which stores the unique ID of that document (the “primary key”, which we
mentioned before).
• The name field, which stores the name of the player.
• The score field, which stores the score of the player.

<b>#29: (A) Document:</b>
Documents are equivalent to SQL rows. For our Leaderboard application, we want to create one document for every player we want in our collection. So if we want our leaderboard to contain six players, we’ll need to use the insert function six times, thereby creating six documents.

<b>#30: ID (Primary Key):</b>
After creating each document, a random jumble of numbers and letters appears in the Console. This jumble is a unique ID that’s automatically created by MongoDB and associated with each document. It’s known as the primary key.
So in the same way we created a name and score field, Mongo creates an _id field for each document.
(The underscore itself doesn’t have any special significance. It’s just part of the field’s name.)

<b>#31: Finding/Fetching/Counting/Retrieving Data:</b>
Once there is some data in a collection, you can retrieve that data. We’ll do this through the interface in the next chapter, but for the moment, let’s simply do it through the Console.
Inside the Console, enter the following:
PlayersList.find();
Here, we’re using this find function, which is used to retrieve data from the specified collection.
Because we’re not passing anything through the brackets, this statement will retrieve all of the data from the collection.
To retrieve data in a more readable format, attach a fetch function to end of it to convert the
retrieved data into an array:
PlayersList.find().fetch();
 But what if we wanted to retrieve a selection of data from the collection, rather than all of the data? To do this, we could pass JSON-formatted data between the brackets: PlayersList.find({ name: "David" }).fetch();
Here, we’repassing a field name and a value through the find function, and as a result, we’re able
to retrieve only the documents where the player’s name field is equal to “David”. In our case, this
will only retrieve one document, but if our collection contained multiple players named “David”,
they would all be returned based on this query.
What’s also useful is the ability to count the number of documents returned by a query by
attaching the count function to the find function:
PlayersList.find().count();
Since this statement will count all of the documents in the collection, if there’s six players
(documents) in the collection, the number 6 will be returned.

<b>#32: Templates:</b>
If we want to start building the user interface for the Leaderboard application, we are going to need to start creating our first templates.
To begin, place the following code inside the leaderboard.html file:
<head>
<title>Leaderboard</title> </head>
<body> <h1>Leaderboard</h1>
</body>
There’s nothing special about this code — it’s just standard HTML — but there does appear to be
a few things missing:
• We haven’t included the html tags.
• We haven’t included any JavaScript files
• We haven’t included any CSS files.
Templates are used to create a connection between our interface and our JavaScript code. When
we place interface elements inside a template, we’re able to reference and manipulate those
elements with application logic.
To create a template, add the following code to the very bottom of the HTML file, beneath the
closing body tag:
<template name="leaderboard">
we place interface elements inside a template, we’re able to reference and
manipulate those
elements with application logic.
To create a template, add the following code to the very bottom of the HTML file, beneath the
closing body tag:
<template name="leaderboard">
Hello World </template>
Here, we’re using this template tag, which uses a name attribute to distinguish between the
different templates we create. In this case, the name of the template is “leaderboard”, and we’ll
soon reference this name from inside the JavaScript file.
If you save the file in its current state though, the template doesn’t appear inside the web browser because
it’s inside the HTML file. This is because, by default, templates don’t appear inside the interface. This might sound weird, but consider that, in some cases:
• You might want a template to appear at certain times.
• You might want a template to disappear at certain times.
• You might want a template to appear in multiple locations.
To account for this possibility, we need to manually include templates inside the interface.
To make the “leaderboard” template appear inside the browser, place this tag between the body tags inside the HTML file:
{{> leaderboard}}
Obviously, this isn’t HTML. Instead. the use of double-curly braces means this is the Spacebars syntax.
Based on these changes, the HTML file should now resemble:
<head>
<title>Leaderboard</title> </head>
<body> <h1>Leaderboard</h1>
{{> leaderboard}} </body>
<template name="leaderboard"> Hello World
</template>

<b>#33: Spacebars Syntax:</b>
Spacebars is the syntax we use in our HTML when we want
 occur. It’s the syntax that bridges the gap between the interface and the application logic.
1. All Spacebars tags use double-curly braces to distinguish themselves.
2. We only use the greater-than symbol when we want to include a template.

<b>#34: Client and Server:</b>
Inside the JavaScript file, write the following console.log statement: console.log("Hello world");
What I didn’t mention last time though is that, as a result of this statement, something else is also
happening, and if we switch to the command line, we can see that the “Hello world” message
also appears there.
This is significant because we’ve written one line of code that’s executed in two places. The
code is running on both the client (within the user’s web browser) and on the server (where the
application is hosted).
Ever since we created the “PlayersList” collection, the following statement has been running on
both the client and the server:
PlayersList = new Mongo.Collection('players');
But the code doesn’t do the same thing in both places.
When the code is executed on the server, a collection is created inside the Mongo database. This is
where our data is stored. When the code is executed from inside the user’s web browser though —
on the client-side — a local copy of that collection is created on that user’s computer. As a result,
when the user interacts with the database, they’re actually interacting with their local copy. This is partly why Meteor applications are real-time by default. Data is manipulated on the user’s local machine and then invisibly synced in the background with the server-side database.
You just need to grasp that one line of code can:
1. Run in two different environments (on the client and on the server).
2. Behave differently depending on the environment.
That said, in some cases, we don’t want our code to be running in two places at once. If, for
instance, we write code that only affects the interface of an application, it wouldn’t make sense
for that code to run on the server. We’d only want it to run on the client.
something dynamic to
To accommodate for this, there’s a pair of conditionals we can use to determine what
2. Behave differently depending on the environment.
That said, in some cases, we don’t want our code to be running in two places at once. If, for
 instance, we write code that only affects the interface of an application, it wouldn’t make sense
for that code to run on the server. We’d only want it to run on the client.
To accommodate for this, there’s a pair of conditionals we can use to determine what code runs
in which environment.
First, place a Meteor.isClient conditional beneath the console.log statement from before:
if(Meteor.isClient){
// this code only runs on the client }
This conditional allows us to specifically execute code on the client — from inside the user’s
web browser.
We can create the reverse effect with the Meteor.isServer conditional: if(Meteor.isServer){
// this code only runs on the server }
But if none of this is really sinking in, just remember two things:
1. A single line of code can run on both the client and the server.
2. Sometimes we don’t want our code to run in both places.
We’ve mostly been writing code that’s meant to run inside the browser (such as code that affects the interface) [on the client]. There are, however, plenty of situations where we want code to run on the server.
Code that is executed on the server is inherently trusted. So while we’ve stopped users of the application from accessing data on the front-end — on the client-side — we can continue
to retrieve the data while on the server.

<b>#35: Helper Function (and Each Block):</b>
At this point, our “leaderboard” template only shows the static “Hello World” text. To fix this,
we’re going to create a helper function, and a helper function is a regular JavaScript function
that’s attached to a template and allows us to execute code from within an interface. To begin, we’ll take an old approach for creating helper functions. This approach is deprecated,
meaning it’s no longer officially supported, and by the time you’re reading these
words, it may
not work at all. But this older format is easier to teach and understand, and allows us to ease
into the non-deprecated approach that we’ll talk about in a moment.
To begin, we’ll take an old approach for creating helper functions. This approach is
deprecated,
meaning it’s no longer officially supported, and by the time you’re reading these
words, it may
not work at all. But this older format is easier to teach and understand, and allows us to ease
into the non-deprecated approach that we’ll talk about in a moment.
Inside the JavaScript file, write the following inside the isClient conditional: Template.leaderboard.player
This is the deprecated syntax for creating a helper function, and it can be broken down into three
parts:
First, the Template keyword searches through the templates in our Meteor project. We only
have one template at the moment, but a complete project would have many more. Second, the leaderboard keyword is a reference to the name of the template we created
earlier. Every helper function must be attached to a template. In this case, the function is attached
to the “leaderboard” template.
Third, the player keyword is the name we’re giving to this function. We will soon reference
this name from inside the HTML file.
To attach code to this helper, associate it with a function: Template.leaderboard.player = function(){
// code goes here }
The word “helper” might make this sound fancy, but we haven’t done anything special here.
We’ve created a function, named it “player”, and connected it to the “leaderboard” template.
To add some functionality to the function, create a return statement that returns some static
text:
Template.leaderboard.player = function(){
return "Some other text" }
Then remove the “Hello World” text from the “leaderboard” template and replace it with the
following tag:
{{player}}
 braces. But
notice that we’re not using the greater-than symbol, and that’s because we’re not including a
Here, we’re using another Spacebars tag, as evidenced by the use of double-curly
with the
Here, we’re using another Spacebars tag, as evidenced by the use of double-curly
following tag:
{{player}}
 braces. But
notice that we’re not using the greater-than symbol, and that’s because we’re not including a
template. Instead, we’re referencing the name of the player function.
If the text doesn’t appear, something is either wrong with the code, or this approach to creating
helpers has been removed from Meteor. Now that you know the old way to create helper functions, we’re ready to discuss the new way.
Delete all of the helper function we just created and replace it with: Template.leaderboard.helpers
Here, we have this Template keyword, which searches through the templates inside our project,
and this leaderboard keyword, which is a reference to the “leaderboard” template. But what about this helpers keyword?
Are we creating a function named “helpers”?
Nope.
This helpers keyword is a special keyword that allows us to define multiple helper functions
inside a single block of code.
Therefore, instead of creating a single helper function: Template.leaderboard.player = function(){
// code goes here }
We create a block for all of a template’s helper functions: Template.leaderboard.helpers({
// helper functions go here });
These helpers are defined in the JSON format, with the name of the helper as the key and an
associated function as the value:
Template.leaderboard.helpers({
'player': function(){
return "Some other text" }
});
With the use of commas, we can create multiple helper functions: Template.leaderboard.helpers({
'player': function(){
return "Some other text" },
'otherHelperFunction': function(){
return "Some other function"
With the use of commas, we can create multiple helper functions:
Template.leaderboard.helpers({ 'player': function(){
 return "Some other text" },
'otherHelperFunction': function(){
return "Some other function" }
});
Both of these helper functions can then be used from inside the “leaderboard” template:
{{player}}
{{otherHelperFunction}}
This code might look a little busier than the deprecated approach, but that’s only because we’re
working with a small amount of helpers. With a larger amount of helpers, organizing them like
this is the far cleaner approach.
What we really want is a helper function that retrieves the documents from the “PlayersList”
collection. Then we’ll be able to display that data from within the interface.
To achieve this, replace the return statement in the helper function with the following:
return PlayersList.find()
Here, we’re using the find function which will retrieve all of the data from the “PlayersList” collection, and because we’ve placed it inside the helper function, this data is now accessible from inside the “leaderboard” template.
Before, our helper function returned a single piece of data — that string from
before — and for
that purpose, this tag was fine, but now the helper is returning an array of all the documents
from inside the collection, and that means we need to loop through the data that’s returned.
To achieve this, we can use the Spacebars syntax to create an each block:
{{#each player}}
test
{{/each}}
Here, there’s a few things going on:
First, all of the documents from the “PlayersList” collection are retrieved based on the reference
to the player function.
Second, we loop through the returned data with the each syntax.
Third, we output the word “test” for each document (player) that’s retrieved. Because there are
six players inside the collection, the word “test” will appear six times within the
First, all of the documents from the “PlayersList” collection are retrieved based on the
reference
to the player function.
Second, we loop through the returned data with the each syntax.
Third, we output the word “test” for each document (player) that’s retrieved. Because there are
six players inside the collection, the word “test” will appear six times within the interface.
Conceptually, it’s like we have an array:
var playersList = ['David', 'Bob', 'Mary', 'Bill', 'Warren', 'Tim'];
...and it’s like we’re using a forEach to loop through the values of this array:
var playersList = ['David', 'Bob', 'Mary', 'Bill', 'Warren', 'Tim']; playersList.forEach(function(){
console.log('test'); });
Within the each block, we can also retrieve the value of the fields from inside our documents.
So because we’re pulling data from the “PlayersList” collection, we can display the values of the
name and score fields.
To display the player’s names, for instance, we can write: {{#each player}}
{{name}} {{/each}}
Then to display the player’s scores, we can write: {{#each player}}
{{name}}: {{score}} {{/each}}
But while we won’t waste time making this application pretty, we will add some slight structure
to the interface:
<ul>
{{#each player}}
<li>{{name}}: {{score}}</li>
{{/each}} </ul>

<b>#36: Events & Event Selectors:</b>
At this point, we have a list of players that’s appearing inside the interface, but there’s no way for
users to interact with this list. The data is dynamically retrieved from the “PlayersList”
 but the user will still probably assume that the application is completely static. We're going to create the effect of being able to select players inside the list: specifically, when a user clicks on one of the players, the background color of that
collection,
no way for
users to interact with this list. The data is dynamically retrieved from the “PlayersList”
 but the user will still probably assume that the application is completely static. We're going to create the effect of being able to select players inside the list: specifically, when a user clicks on one of the players, the background color of that player’s li element will change to yellow.
We're going to create our first event, and events allow us to trigger the execution of code
when a user clicks on a button, taps a key on their keyboard, or completes a range of other
actions.
To demonstrate this, write the following inside the isClient conditional: Template.leaderboard.events({
// events go here });
Here, there’s a few things going on:
First, the Template part is used to search through all of the templates in the project. Second, the leaderboard part is the name of the template we’re about to attach an event to.
Third, the events part is special keyword that’s used to specify that, within the coming block of
code, we want to specify one or more events. (This code is very similar to how we create helper
functions.)
Between the curly braces of the events block, create an event using the JSON format: Template.leaderboard.events({
'click': function(){
// code goes here }
});
Here, there’s two things going on:
First, we’ve defined the event type. That’s the click part. Because of this, the code inside
the associated function will execute when a user clicks anywhere within the bounds of the
“leaderboard” template.
Second, we’ve attached a function to this event, and inside this function, we can write whatever
code we want to execute when that click occurs.
To demonstrate this, add a console.log statement inside the event:
Template.leaderboard.events({ 'click': function(){
console.log("You clicked something");
collection,
}
whatever
code we want to execute when that click occurs.
To demonstrate this, add a console.log statement inside the event:
Template.leaderboard.events({ 'click': function(){
console.log("You clicked something"); }
});
After saving the file, switch back to Chrome and click anywhere within the bounds of the
“leaderboard” template. With each click, the “You clicked something” message will appear inside
the Console.
The event we’ve created is too broad. It triggers when the user clicks anywhere within the bounds
of the “leaderboard” template. That could be useful in certain circumstances, but generally we’ll
want an event to trigger when a user does something precise, like clicking a particular button.
To achieve this, we’ll use event selectors, and selectors allow us to attach events to specific HTML
elements.
The plan now is to make it so our event triggers when the user clicks on one of these li elements.
To do this, change the event to the following:
'click li': function(){
console.log("You clicked an li element"); }
Here, we’ve made two changes:
First, we’ve added the li part after the click keyword. This means the event will now trigger
when a user clicks any li element inside the “leaderboard” template.
Second, we’ve changed the output of the console.log statement.
What would happen if we had other li elements inside the “leaderboard” template that aren’t
part of the player’s list? It’d cause a problem because the event would trigger when we didn’t want it to trigger.
To fix this, add a .player class to the li elements:
<li class="player">{{name}}: {{score}}</li>
Then use this class as the event selector:
'click .player': function(){
 }
Here, we’ve made is so the event will only trigger when the user clicks on an element that has
console.log("You clicked a .player element");
<li class="player">{{name}}: {{score}}</li> console.log("You clicked a .player element");
Then use this class as the event selector: 'click .player': function(){
 }
Here, we’ve made is so the event will only trigger when the user clicks on an element that has
the .player class attached to it.

<b>#37: Sessions:</b>
When a user clicks one of the .player elements, a function executes. When this function is
triggered, we want to change the background color of that element, thereby creating the effect
of the player being selected.
To achieve this, we’ll use sessions, and sessions allow us to store small pieces of data that is not
saved to the database and won’t be remembered on return visits. This sort of data might
not sound immediately useful, but it’s a surprisingly versatile way to solve a lot of common
problems.
To create a session, write the following statement inside the click .player event: Session.set('selectedPlayer', 'session value test');
Here, we’re using this Session.set function and passing through two arguments:
First, we’re passing through a name for the session. This name is used as a reference. In this
case, we’re calling the session “selectedPlayer”, but feel free to use whatever name you like.
Second, we’re passing through a value for the session. This is the data we’re storing inside
the session. In this case, we’re passing through the static value of “session value test”, but we’ll
use a more interesting value in a moment.
To prove that our session is working as expected, retrieve the value of the sessions with the
following statement:
Session.get('selectedPlayer');
The events block should then resemble:
Template.leaderboard.events({
'click .player': function(){
Session.set('selectedPlayer', 'session value test');
Session.get('selectedPlayer'); }
});
Here, we’re using this Session.get function and passing through the name of the
Template.leaderboard.events({ 'click .player': function(){
Session.set('selectedPlayer', 'session value test');
 Session.get('selectedPlayer'); }
});
Here, we’re using this Session.get function and passing through the name of the “selected-
Player” session that we created a moment ago.
To output the value of this session to the Console, place it inside a variable:
var selectedPlayer=Session.get('selectedPlayer');
Then add a console.log statement beneath this line:
var selectedPlayer=Session.get('selectedPlayer');
console.log(selectedPlayer);
Now when a user clicks on one of the player elements, the “session value test” string will be
stored inside a session and then immediately output to the Console.
When a user clicks one of the players in the list, we want to grab the unique ID of the player
and store it inside the “selectedPlayer” session. This will then allow us to change the background
color of that particular player’s li element.
To begin, create a “playerId” variable at the top of the click .player event, and make it equal
to the “session value test” string from before:
var playerId = "session value test";
Then modify the Session.set function by passing through the “playerId” variable as the second
argument. The event should then resemble:
'click .player': function(){
var playerId = "session value test"; Session.set('selectedPlayer', playerId);
var selectedPlayer=Session.get('selectedPlayer');
}
At this point, the trick is to make the “playerId” variable equal to the unique ID of the player
that’s been clicked.
For now, change the “playerId” variable to the following:
var playerId = this._id;
As for the explanation, there’s two things going on:
First, we have a reference to this, and the value of this depends on the context. In this
context,
this refers to the document of the player that has just been clicked.
Second, the _id part is the name of the field that contains the unique ID of the player.
So in the
    var playerId = this._id;
As for the explanation, there’s two things going on:
First, we have a reference to this, and the value of this depends on the context. In this
context,
this refers to the document of the player that has just been clicked.
Second, the _id part is the name of the field that contains the unique ID of the player. So in the
same way we created a name and score field, Mongo creates an _id field for each document.
(The underscore itself doesn’t have any special significance. It’s just part of the field’s name.)
Because of this change, the following is now possible:
1. A user clicks on one of the players.
2. The player’s unique ID is stored inside the “playerId” variable.
3. The value of the “playerId” variable is stored inside the “selectedPlayer” session. (There can
only be one value stored inside a session, so each time a new value is stored, the previous
value is overwritten.)
4. The value of the “selectedPlayer” session is output to the Console.
Since we don’t need to see the unique ID of the clicked player inside the Console though, we can
simplify the event to the following:
'click .player': function(){
var playerId = this._id;
Session.set('selectedPlayer', playerId); }
Here, we’re just setting the value of the “selectedPlayer” session to the unique ID of the clicked Player.
When a user clicks one of the players inside our list, we want to change the background-color
property of the li element that contains that player. This will create the effect of that player
being selected.
To achieve this, open the project’s CSS file and create a class named “selected”. This class should
have a background-color property, and for this example we’ll pass through a value of “yellow”:
.selected{
background-color: yellow; }
 Template.leaderboard.helpers({ 'player': function(){
return PlayersList.find()
Then switch to the JavaScript file and create a “selectedClass” helper:
.selected{
background-color: yellow; }
 Template.leaderboard.helpers({ 'player': function(){
return PlayersList.find() },
'selectedClass': function(){
// code goes here }
});
As for the content of this function, we’ll make it return the word “selected”:
'selectedClass': function(){
return "selected" }
Note: We need the returned text to be equal to the name of the class in the CSS file, so because
we named the class “selected” in the CSS file, we’re returning this “selected” text from within
the function.
Next, switch to the HTML file and place a reference to this “selectedClass” function inside the
li element’s class attribute:
<li class="player {{selectedClass}}">{{name}}: {{score}}</li>
The “selected” class will be applied to each .player element, thereby changing the background
color of each element to yellow.
Inside the selectedClass helper function, comment out the return statement: 'selectedClass': function(){
// return "selected" }
Then write the following:
'selectedClass': function(){ // return "selected"
return this._id }
Here, we’re using this._id to retrieve the unique ID of the player. But instead of the ID being
output to the Console, it’ll appear inside the class attribute for each of the li elements. This is
not exactly what we want but it’s important to know that, because the selectedClass
function
is being executed from inside the each block, it has access to all of the data that is being iterated
Then switch to the JavaScript file and create a “selectedClass” helper:
through (including the player’s unique ID, name, and score).
output to the Console, it’ll appear inside the class attribute for each of the li elements.
This is
not exactly what we want but it’s important to know that, because the selectedClass
 function
is being executed from inside the each block, it has access to all of the data that is being iterated
through (including the player’s unique ID, name, and score).
Knowing this, we’ll do a few things:
First, we’ll delete the return this._id statement since it was only for demonstration purposes.
Second, we’ll uncomment the return statement since we do want the selectedClass function
to return the static text of “selected”.
Third, we’ll create a “playerId” variable at the top of the function that holds the value of this._id:
'selectedClass': function(){
var playerId = this._id;
return "selected" }
Fourth, we’ll create a “selectedPlayer” variable for the “selectedPlayer” session: 'selectedClass': function(){
var playerId = this._id;
var selectedPlayer=Session.get('selectedPlayer'); return "selected"
}
Fifth, wrap the return statement in the following conditional: 'selectedClass': function(){
var playerId = this._id;
var selectedPlayer=Session.get('selectedPlayer'); if(playerId == selectedPlayer){
return "selected" }
}
If you’re having trouble following the logic though, here’s what’s going on:
When a user clicks one of the players in the list, the unique ID of that player is stored inside
the “selectedPlayer” session. The ID in that session is then matched against all of the IDs of
the players in the list. Because the player’s ID will always be unique, there can only ever be a
single match, and when there is that match, the static text of “selected” will be
returned by the
selectedClass function and placed inside the class attribute for that players li element. Based
on that class, the background color of the player’s li element will be changed to yellow.
the players in the list. Because the player’s ID will always be unique, there can only
ever be a
single match, and when there is that match, the static text of “selected” will be
returned by the
selectedClass function and placed inside the class attribute for that players li element. Based
on that class, the background color of the player’s li element will be changed to yellow. (And
because the session can only store a single value, only one player can be selected at a time.)

<b>#38: Give 5 Points (Increment)/Buttons:</b>
Inside the “leaderboard” template, we’ll create a “Give 5 Points” button that, when clicked, will
increment the score of the selected player.
To begin, place the following button inside the “leaderboard” template:
<input type="button" class="increment" value="Give 5 Points">
The button should be located outside of the each block and have a class attribute that’s set to
“increment”.
To make the button do something, add the following event to the events block that’s inside the
JavaScript file:
'click .increment': function(){
// code goes here }
The entire events block should resemble:
Template.leaderboard.events({ 'click .player': function(){
var playerId = this._id;
Session.set('selectedPlayer', playerId); },
'click .increment': function(){
// code goes here }
});
Within the click .increment event, we’ll use the unique ID of the selected player to find that
player inside the “PlayersList” collection and increment the value of that player’s score field by
5.
 'click .increment': function(){
var selectedPlayer=Session.get('selectedPlayer'); }
To access the unique ID of the selected player, use the Session.get function:
field by 5.
 'click .increment': function(){
var selectedPlayer=Session.get('selectedPlayer'); }
You can verify this functionality with a console.log statement:
'click .increment': function(){
var selectedPlayer=Session.get('selectedPlayer');
console.log(selectedPlayer); }
At this point, we want to make is so when a user selects a player from the list and clicks the
“Give 5 Points” button, the score field for that player is modified.
To do this, remove the console.log statement from the click .increment event and replace it
with the following:
PlayersList.update();
This is the Mongo update function and, between the brackets, we can define:
1. What document (player) we want to modify.
2. How we want to modify that document.
To do this, we’ll first retrieve the selected player’s document. This can be done by passing through
the unique ID of the selected player:
PlayersList.update(selectedPlayer);
The event should now resemble:
'click .increment': function(){
var selectedPlayer=Session.get('selectedPlayer');
PlayersList.update(selectedPlayer); }
To modify the document, we pass a second argument into the update function to define what
part of the document we want to change:
'click .increment': function(){
var selectedPlayer=Session.get('selectedPlayer');
PlayersList.update(selectedPlayer, {score: 5}); }
This statement will:
1. Find the document of the selected player, based on that player’s ID.
2. Update that document by changing the value of the score field to 5.
But if you test this feature, you’ll notice that it’s broken. If you select a player and click
the “Give
5 Points” button, the name of that player will disappear. The value of the score field will change
To access the unique ID of the selected player, use the Session.get function:
to 5, as planned, but the name field will be completely removed from the document.
1. Find the document of the selected player, based on that player’s ID.
2. Update that document by changing the value of the score field to 5.
But if you test this feature, you’ll notice that it’s broken. If you select a player and click
 the “Give
5 Points” button, the name of that player will disappear. The value of the score field will change
to 5, as planned, but the name field will be completely removed from the document. This might seem like a bug, but by default, the update function works by deleting the original
document and creating a new document with the data that we specify. The value of the _id field
will remain the same, but since we’ve only specified the score field inside the update statement,
that’s the only other field that remains inside the modified document.
To account for this, we need to use a Mongo operator that allows us to set the value of the score
field without deleting the original document.
First, replace the update function’s second argument with the following:
'click .increment': function(){
var selectedPlayer=Session.get('selectedPlayer');
PlayersList.update(selectedPlayer, {$set: }); }
Here, we’re using this $set operator to modify the value of a field (or multiple fields) without
deleting the original document. After the colon, we just have to pass through the fields we want
to modify (and their new values): 'click .increment': function(){
var selectedPlayer=Session.get('selectedPlayer');
PlayersList.update(selectedPlayer, {$set: {score: 5} }); }
Because of this change, the update function won’t be completely broken. If we save the file and
switch back to Chrome, we can see that selecting a player and clicking the “Give 5 Points” button
will modify the score field of that player without affecting the rest of the document. But despite this success, we still haven’t created the feature that we aimed to create. Because
while our button can set the selected player’s score field to the value of 5, that’s all it can do. No
matter how many times we click the button, the value of the field won’t increase any
To fix this problem, replace the $set operator with the $inc operator: 'click .increment': function(){
var selectedPlayer=Session.get('selectedPlayer');
further.
while our button can set the selected player’s score field to the value of 5, that’s all it further.
can do. No
matter how many times we click the button, the value of the field won’t increase any
 To fix this problem, replace the $set operator with the $inc operator: 'click .increment': function(){
var selectedPlayer=Session.get('selectedPlayer');
PlayersList.update(selectedPlayer, {$inc: {score: 5} }); }
Based on this change, whenever the update function is triggered, the value of the score field
will be incremented by whatever value we specify (in this case, that’s the value of 5).

<b>#39: Take 4 Points/Decrement:</b>
A feature that’s not present in the original Leaderboard application is the ability to decrement
scores. Such a feature would be useful though since it means we could:
1. Penalize players for not following the rules.
2. Retract points that are mistakenly awarded.
To begin, create a “Take 5 Points” button inside the “leaderboard” template:
<input type="button" class="decrement" value="Take 5 Points">
As with the “Give 5 Points” button, place it outside the each block and provide it with a unique
class attribute (such as “decrement”).
Next, switch to the JavaScript file, copy the click .increment event, and paste the code into the
same events block.
The events block should resemble:
Template.leaderboard.events({
'click .player': function(){ var playerId = this._id;
Session.set('selectedPlayer', playerId); },
'click .increment': function(){
var selectedPlayer=Session.get('selectedPlayer');
PlayersList.update(selectedPlayer, {$inc: {score: 5} }); },
'click .increment': function(){
var selectedPlayer=Session.get('selectedPlayer');
PlayersList.update(selectedPlayer, {$inc: {score: 5} }); }
});
At this point, we only need to make two changes:
First, change the selector for the newly created event from .increment to .decrement. Second, pass a value of -5 through the inc operator, rather than a value of 5. The
addition of the
PlayersList.update(selectedPlayer, {$inc: {score: 5} }); }
});
 At this point, we only need to make two changes:
First, change the selector for the newly created event from .increment to .decrement. Second, pass a value of -5 through the inc operator, rather than a value of 5. The addition of the
- reverses the functionality of the operator, so the $inc operator will now decrement the value
of the score field.
The final code for the event should resemble:
'click .decrement': function(){
var selectedPlayer=Session.get('selectedPlayer');
PlayersList.update(selectedPlayer, {$inc: {score: -5} }); }

<b>#40: Sorting Documents (sort operator):</b>
At the moment, the players in the list are ranked by the time they were inserted into the
collection, rather than being ranked by their scores.
To fix this, we’ll modify the return statement that’s inside the player helper function: 'player': function(){
return PlayersList.find() }
First, pass a pair of curly braces through the brackets of the find function: 'player': function(){
return PlayersList.find({}) }
By using these curly braces, we’re explicitly stating that we want to retrieve all of the data
from the “PlayersList” collection. This is the default behavior, so both of these statements are
technically the same:
return PlayersList.find()
return PlayersList.find({})
But by passing through the curly braces as the first argument, we can pass through a second
argument, and it’s within this second argument that we can define how we want to sort the data
that’s retrieved.
As the second argument, pass through the sort operator:
return PlayersList.find({}, {sort: })
(Unlike the $set and $inc operators, we don’t use a dollar sign at the start of this operator’s
name.)
sort the data
that’s retrieved.
As the second argument, pass through the sort operator:
return PlayersList.find({}, {sort: })
(Unlike the $set and $inc operators, we don’t use a dollar sign at the start of this operator’s
name.)
Then choose to sort by the value of the score field:
return PlayersList.find({}, {sort: {score: -1} })
By passing through a value of -1, we can sort in descending order. This means we’re sorting the
players from the highest score to the lowest score. If we passed through a value of 1, the players
would be sorted from the lowest score to the highest score.
Based on this change, the players will be ranked based on their score, but what happens if two
players have the same score?
Take “Bob” and “Bill”, for instance. If they have the same score, Bill should be ranked above Bob
because, alphabetically, his name comes first. But at the moment, that won’t happen since Bob
was added to the collection before Bill.
To fix this, pass the name field through the sort operator, but this time, pass through a value of
1 instead of -1:
return PlayersList.find({}, {sort: {score: -1, name: 1} })
The players will still be primarily ranked by their scores, but once that sorting has occurred,
the players will also be ranked by their names. This secondary sorting will occur in ascending
(alphabetical) order.

<b>#41: "showSelectedPlayer"/findOne (Individual Documents):</b>
When a user selects one of the players, that player’s name should appear beneath the list of
players. This isn’t the most useful feature, but:
1. It’s part of the original Leaderboard application.
2. It means we can talk about a couple of Meteor’s features.
Inside the JavaScript file, create a “showSelectedPlayer” helper function that’s attached to the
“leaderboard” template:
 // code goes here }
Inside the function, retrieve the unique ID of the currently selected player:
'showSelectedPlayer': function(){
Inside the JavaScript file, create a “showSelectedPlayer” helper function that’s 'showSelectedPlayer': function(){
attached to the “leaderboard” template:
 // code goes here }
Inside the function, retrieve the unique ID of the currently selected player:
'showSelectedPlayer': function(){
var selectedPlayer=Session.get('selectedPlayer'); }
Then write a return statement that returns the data from a single document inside the “PlayersList” collection. We could use the find function, but the findOne function is the preferred
alternative:
'showSelectedPlayer': function(){
var selectedPlayer=Session.get('selectedPlayer');
return PlayersList.findOne(selectedPlayer) }
By using the findOne function, we can pass through the unique ID of a document as the only
argument, and we’re able to avoid unnecessary overhead since this function will only ever
attempt to retrieve a single document. It won’t look through the entire collection like the find
function would.
With this function in place, switch to the HTML file and place a reference to the function inside
the “leaderboard” template. I’ve placed mine at the bottom of my list, between a pair of li tags:
<li>Selected Player: {{showSelectedPlayer}}</li>
But if we save the file, the output won’t look quite right, and that’s because the findOne function
is retrieving the player’s entire document. To fix this, we need to specify that we only want to
show the value of the name field, which can be done with dot notation:
<li>Selected Player: {{showSelectedPlayer.name}}</li>
We should also make it so the template doesn’t attempt to display a player’s name if a player
isn’t selected, which can be done with a simple conditional:
{{#if showSelectedPlayer}}
<li>Selected Player: {{showSelectedPlayer.name}}</li> {{/if}}

<b>#42: Forms (submit event)/preventDefault function/Inserting-removing Players (submit/remove function):</b>
We’re going to create a form that allows users to add players to the leaderboard,
{{#if showSelectedPlayer}}
<li>Selected Player: {{showSelectedPlayer.name}}</li> {{/if}}
We’re going to create a form that allows users to add players to the leaderboard, along with some other interface controls.
Inside the HTML file, create a second template named “addPlayerForm”:
<template name="addPlayerForm">
</template>
Then include this somewhere inside the “leaderboard” template:
{{> addPlayerForm}}
Within the “addPlayerForm” template, create the following two elements: 1. A text field with the name attribute set to “playerName”.
2. A submit button with the value attribute set to “Add Player”.
The template should then resemble:
<template name="addPlayerForm">
<form>
<input type="text" name="playerName"> <input type="submit" value="Add Player">
</form> </template>
We’ve already seen a couple examples of the click event, which allows us to trigger the execution
of code when the user clicks on a particular element. In a similar vein, there’s also the submit
event, which allows to trigger the execution of code when the user submits a form. To do this, create another events block inside the isClient conditional: Template.addPlayerForm.events({
// events go here });
(We need a new events block because this event will be attached to the new “addPlayerForm”
template, rather than the “leaderboard” template.)
Within this events block, create an event with the event type set to “submit” and the selector set
to “form”: Template.addPlayerForm.events({
'submit form': function(){ // code goes here
} });
Based on this code, the event’s function will trigger when the form inside the
“addPlayerForm”
Template.addPlayerForm.events({
'submit form': function(){ // code goes here
} });
Based on this code, the event’s function will trigger when the form inside the “addPlayerForm”
templateis submitted.
But why don’t we just use the click event for the form? Won’t most users click the submit button
anyway? That might be the case, but it’s important to remember that forms can be submitted in
a number of ways. In some cases, the user will click the submit button, but at other times they’ll
tap the “Return” key on their keyboard. By using the submit event type, we’re able to account
for every possible way that form can be submitted.
But as it turns out, there is actually a problem with the event, because when we submit the form:
1. The web browser refreshes the page.
2. The “Form submitted” message doesn’t appear inside the Console.
Why does this happen?
When we place a form inside a web page, the browser assumes we want to take the data from
that form and send it somewhere. The problem is, when working with Meteor, we don’t want to
send the data anywhere — we want it to remain within the current page — but since this isn’t
standard behavior as far as the browser is concerned, the web page simply refreshes. Knowing this, we must be disable the default behavior that web browsers attach to forms.
When an event is triggered from within a Meteor application, we can access information about
that event as it occurs. That might sound weird, but to show you what I mean, change the submit
form event to the following:
'submit form': function(event){
console.log("Form submitted");
console.log(event.type); }
Here, we’re passing this “event” keyword through the brackets of the event’s
 outputting the value of event.type to the Console.
This result of this is two-fold:
First, whatever keyword is passed through the brackets of event’s function as the first
function, and then
}
Here, we’re passing this “event” keyword through the brackets of the event’s
 outputting the value of event.type to the Console.
This result of this is two-fold:
First, whatever keyword is passed through the brackets of event’s function as the first parameter
becomes a reference for that event. Because we’ve passed through the “event” keyword, we’re
able to reference the event inside the event’s function using that keyword. You can, however, use
whatever keyword you prefer. (A common convention is to use “evt” or “e” instead of “event”.)
Second, the event.type part is a reference to the “type” property of the event object. As a result,
this code should output the word “submit” to the Console since that’s the type of event that’s
being triggered.
This doesn’t solve the original problem though since our page still refreshes whenever the form
is submitted and we can’t see the console.log statements.
To fix this, use the preventDefault function:
'submit form': function(event){
event.preventDefault(); console.log("Form submitted"); console.log(event.type);
}
When attached to the event object, this preventDefault function prevents the default behavior
of the event from occurring. So because we’ve attached the function to the submit form event:
1. By default, submitting the form won’t do anything.
2. We’ll need to manually define the form’s functionality.
3. The console.log statements will now work as expected.
Note: The preventDefault function does not just apply to forms. You can, for instance, take
complete control of the links within a template:
'click a': function(event){
event.preventDefault(); }
With this code in place, any a elements within the template wouldn’t behave as they
usually
would. You’d have to manually assign them functionality.
Now that we have complete control over the form, we want the submit form event to
function, and then
grab the
event.preventDefault();
}
With this code in place, any a elements within the template wouldn’t behave as they
 usually
would. You’d have to manually assign them functionality.
Now that we have complete control over the form, we want the submit form event to grab the
contents of the “playerName” text field when the form is submitted, and use that value when
adding a player to the database.
To begin, create a variable named “playerNameVar”:
'submit form': function(event){
event.preventDefault();
var playerNameVar; }
Then make this variable equal to “event.target.playerName” and output the value of the variable
to the Console:
'submit form': function(event){
event.preventDefault();
var playerNameVar = event.target.playerName; console.log(playerNameVar);
}
Here, this statement uses the event object to grab whatever HTML element has the name attribute
set to “playerName”.
But this code won’t work exactly as you might expect, since the console.log statement outputs
the raw HTML for the text field, rather than its value.
This is because we need to explicitly retrieve the value property: 'submit form': function(event){
event.preventDefault();
var playerNameVar = event.target.playerName.value; console.log(playerNameVar);
}
Based on this change, whatever the user types into the “playerName” text field will now be
output to the Console when they submit the form.
To insert the submitted player into the “PlayersList” collection, add the insert function inside
the submit form event:
PlayersList.insert({
name: playerNameVar,
score: 0 });
To insert the submitted player into the “PlayersList” collection, add the insert function
inside
the submit form event:
PlayersList.insert({
name: playerNameVar,
score: 0 });
But rather than passing through a hard-coded value to the name field, like “David” or “Bob”, pass
through a reference to the “playerNameVar” variable.
The code for the event should now resemble:
'submit form': function(event){
event.preventDefault();
var playerNameVar = event.target.playerName.value; PlayersList.insert({
name: playerNameVar,
score: 0 });
}
Since we’ve made it possible to add players to the leaderboard, it’s a good idea to make it possible
to also remove players from the leaderboard.
To achieve this, first create a “Remove Player” button from inside the “leaderboard” template:
<input type="button" class="remove" value="Remove Player">
As with the other buttons in this project, attach a unique class attribute to it so we can reference
the button from an events block.
Inside the JavaScript file, attach the following event to the “leaderboard” template: 'click .remove': function(){
// code goes here }
Retrieve the ID of the selected player from the “selectedPlayer” session:
'click .remove': function(){
var selectedPlayer=Session.get('selectedPlayer'); }
Then use the remove function to remove the selected player from the collection:
'click .remove': function(){
var selectedPlayer=Session.get('selectedPlayer');
PlayersList.remove(selectedPlayer); }
We haven’t talked about the remove function yet, but there’s nothing much to say
 about it. All
we have to do is pass through the unique ID of a document as the only argument. That document
will then be removed from the collection.
PlayersList.remove(selectedPlayer); }
We haven’t talked about the remove function yet, but there’s nothing much to say
 about it. All
we have to do is pass through the unique ID of a document as the only argument. That document
will then be removed from the collection.

<b>#43: Accounts System:</b>
We're going to create a user accounts system, which just so happens to be one of the simplest
things we can do with the framework.
With this system in place, we’ll make it so:
• Users can register and login to the application.
• Logged-out users won’t see the “Add Player” form.
• Every user will have their own, unique leaderboard.
To add a user accounts system to our project, we’ll first install a “login provider” package. These
packages make it extremely easy to add a back-end for an accounts system to an application.
Usually, for instance, creating a user accounts system would involve creating a collection for the
user’s data:
UserAccounts = new Mongo.Collection('users');
Then writing the application logic for registration and logging in, etc.
But when working with Meteor, all we have to do is switch to the command line and run the
following command:
meteor add accounts-password
Here, we’re adding this “accounts-password” package to the project. This package creates the
back-end for an accounts system that relies on an email and password for registration and logging
in.
Specifically, this package:
1. Creates a collection for storing the data of registered users.
2. Provides us with a range of useful functions we’ll soon cover.
There’s other login provider packages available that allow users to login to our application
through services like Google and Facebook, but since this adds an extra step to the process,
we’ll focus on an email and password system.
We’ve already setup the back-end for an accounts system, but what about the front- end? Are
we expected to write the interface code that allows people to register and login and
application
through services like Google and Facebook, but since this adds an extra step to the process,
we’ll focus on an email and password system.
We’ve already setup the back-end for an accounts system, but what about the front- end? Are
we expected to write the interface code that allows people to register and login and change their
account details?
Nope.
We can create a custom interface, and it’s actually a very simple thing to do, but there’s an easier
way to get up and running as soon as possible.
To instantly add the front-end of an accounts system to a project, we simply have to install the
“accounts-ui” package:
meteor add accounts-ui
Then, once installed, place the following between the body tags of the HTML file (or inside one
of the templates):
{{> loginButtons}}
Here, we’re including this “loginButtons” template, which is included with the “accounts-ui”
package. So because that package has been added to this project, we can now include this template
anywhere we want within the interface.
This is not a mere dummy interface though. Already, without any configuration, it’s possible
for users to register, login, and logout.
At the moment, unregistered users can see the “Add Player” form, which doesn’t make a lot of
sense. This form should only be accessible to registered users.
To achieve this, change the “addPlayerForm” template to the following:
<template name="addPlayerForm">
{{#if currentUser}} <form>
<input type="text" name="playerName">
<input type="submit" value="Add Player"> </form>
{{/if}} </template>
 in or not.
This object is provided by the “accounts-password” package, and the logic’s fairly simple:
Here, we’re referring to this currentUser object to check if the current user is logged-
</form>
Here, we’re referring to this currentUser object to check if the current user is logged-
{{/if}} </template>
 in or not.
This object is provided by the “accounts-password” package, and the logic’s fairly simple:
1. If the current user is logged-in, currentUser will return true.
2. If the current user is not logged-in, currentUser will return false.
To make our application somewhat useful to a wider audience, we need to make it so each
registered user can make their own, independent list of players.
To begin, place the following statement:
var currentUserId = Meteor.userId();
...inside the submit form event:
'submit form': function(event){
event.preventDefault();
var playerNameVar = event.target.playerName.value; var currentUserId = Meteor.userId(); PlayersList.insert({
name: playerNameVar,
score: 0 });
}
Here, we’re creating this “currentUserId” variable, which stores the value that’s returned by the
Meteor.userId function. This function simply returns the unique ID of the currently logged in user.
Then add a “createdBy” field inside the insert function, and pass through the “currentUserId”
variable:
PlayersList.insert({
name: playerNameVar, score: 0,
createdBy: currentUserId
});
As a result, when a user adds a player to the leaderboard, the unique ID of that user will be
associated with the player that’s being added.
First, setup another “currentUserId” variable:
'player': function(){
var currentUserId = Meteor.userId();
return PlayersList.find({}, {sort: {score: -1, name: 1}}); }
Then change the return statement so it only returns players when their createdBy field
is equal
First, setup another “currentUserId” variable:
'player': function(){
var currentUserId = Meteor.userId();
 return PlayersList.find({}, {sort: {score: -1, name: 1}}); }
Then change the return statement so it only returns players when their createdBy field is equal
to the unique ID of the currently logged-in user:
'player': function(){
var currentUserId = Meteor.userId();
return PlayersList.find({createdBy: currentUserId}, {sort: {score: -1, name: 1}}); }
This ensures that users only see players they added to the leaderboard, thereby creating the effect
that each user has their own, unique list of players.
(To see the definition of (a) "Packages", see below/#44.)

<b>#44: Packages:</b>
To extend the functionality of our Meteor projects in a matter of seconds, we can install a range
of packages, and packages are essentially plugins that:
1. Add important features to a project.
2. Reduce the amount of code we need to write.
By default, every Meteor project has local access to a number of official packages. These are
packages that most developers will need to use at some point or another, but not necessarily
inside every project. (There are also thousands of third-party packages.)

<b>#45: Meteor.users:</b>
Once the “accounts-password” package is added to the project, a collection is automatically
created to store the data of registered users. This collection is known as Meteor.users and it
works just like any collection that we might create ourselves.
Knowing this, we can use the find and fetch functions on this collection: Meteor.users.find().fetch();

<b>#46: meteor reset (Reset)/Stopping the Local Server:</b>
To give ourselves a fresh start, switch to the command line, stop the local server with CTRL
+ C, and enter the following command:
meteor reset
This will wipe the database clean, and because of the code we wrote in the previous section, all
players added to the collection at this point will be attached to the currently logged-in user.
You’ll probably find yourself using this command semi-regularly, as lots of useless data can easily
fill up a database during development.

<b>#47: autopublish:</b>
The functionality that allows us to navigate through a project’s data using the Console is
contained within an “autopublish” package that’s included with every meteor project by default.
If we remove this package, users won’t be able to access any data through the Console, but it
will also break the application.
To remove the “autopublish” package from the project, run the following command: meteor remove autopublish
(After you delete the package,) we can no longer navigate through the data inside the collection. The only
thing returned is an empty array. It looks like the data has been deleted, but that’s not the case.
It’s just been secured.
The problem is, our data is now too secure, because if we login to either of the user accounts, the
data is also inaccessible from the interface.

<b>#48: Publishing Data (Meteor.publish):</b>
Conceptually, you can think of publishing data as transmitting data from the server and into the
ether. We’re just specifying what data should be available to users. We don’t care where that
data ends up.
This code duplicates the functionality of the autopublish, meaning it’s not exactly what we
want, but it’s a step in the right direction.
 the server
that belongs to the currently logged-in user. This means:
The goal now is to make it so the Meteor.publish function only publishes data from
we
want, but it’s a step in the right direction.
 the server
that belongs to the currently logged-in user.
This means:
1. Logged-in users will only have access to their own data.
2. Logged-out users won’t have access to any data.
To achieve this, we’ll need to access the unique ID of the currently logged-in user from within the
Meteor.publish function. While inside this function though, we can’t use the Meteor.userId()
function from before. Instead, we have to use the following statement:
this.userId;
This statement returns the unique ID of the currently logged-in user.
If you’re logged-in, you’ll only see the data that belongs to the current user’s account, and if
you’re not logged-in, you won’t see any data. This is because the return statement inside the
Meteor.publish function can only return documents that contain the unique ID of the current user.
The return statement inside the player function can only ever retrieve data that is being published from the server. Therefore, specifying that we want to retrieve the user’s data in
two places is redundant. We only need to define the returned data within the Meteor.publish
function.

<b>#49: Subscribing [to] Data (Meteor.subscribe):</b>
[Because of the Meteor.publish function that’s executing on the server, we can now subscribe to
this data from inside the isClient conditional, once again making the project’s data accessible
through the browser and Console.]
If you imagine that the publish function is transmitting data into the ether, then the subscribe
function is what we use to “catch” that data.
This is the Meteor.subscribe function, and the only argument we need to pass through is the
name of a publish function:
Meteor.subscribe('thePlayers');
You’ll notice that, once again, we have access to all of the data from the project’s database,
meaning our application is back to its original state.
The goal now is to make it so the Meteor.publish function only publishes data from
through is the
name of a publish function: Meteor.subscribe('thePlayers');
You’ll notice that, once again, we have access to all of the data from the project’s database,
meaning our application is back to its original state.

<b>#50: Methods:</b>
To achieve this [See Q#12], we’ll create our first methods, and methods are blocks of code that are executed
on the server after being triggered from the client.
The syntax is similar to how we create both helpers and events.
By using this Meteor.call [Definition/Code Needed] statement, and passing through the name of the method we created, we’re able to trigger the execution of the method whenever the “Add Player” form is submitted.
The submission of the client-side form is triggering the method, but the actual code inside the method is being executed on the server.
[This means:
1. The insert function will successfully (and securely) run on the server.
2. Users still won’t be able to insert data through the Console.
For now, the important part is that, while users can add players to the list by using the form,
they’re not able to use the insert function from inside the Console. This means we’re gaining
control over how users interact with the database, which is a vital part of keeping an application
secure.]
