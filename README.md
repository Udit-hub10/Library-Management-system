# Library-Management-system

This is a Library API Backend for the management of users and the book

# Routes and the Endpoint

## /users
GET: Get all the list of user in the system
POST: Create?register a new user

## /users{id}

GET: Get user by their ID
PUT: Updating a user by their ID
DELETE: Deleting a user by their ID(check if the user still has an issued book) && (is there any fine/penalty to be collected)

## /users/subscription-details/{id}
GET:Get a user subscription detail by thier ID
    >>Date of subscription
    >>Valid till ?
    >>Fine if any ?


## /books
GET:Get all the books in the system
POST: Add a new book to the system

## /books/{id}
GET:Get a book by its id
PUT:Update a book by its id
Delete: Delete a book by its id

## /books/issued
GET: Get all issued book

## books/issued/withfine
GET: Get all issued books with their fine amount

## Subscription type

    >>Basics{3 month}
    >>Standard{6 month}
    >>Premium{ 12 months}

>>If a user missed the renewal date, then user should be collected with $100
>>If a user missed subscription,then user is expected to pay $100
>>If auser both renewal and miss subscription, then the collected amount should be $200

## Commands:
npm init
npm i express
npm i nodemon --save-dev