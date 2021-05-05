# Developer Interview Questions

## General

1. What are RESTful APIs and what methods they use? 
1. What is the difference between passing by value and passing by reference?

## HTML

1. What is the difference between `<div` and `<span` tags? 
2. Give examples of HTML tag which have been deprecated in HTML5.
3. What meta tag you should use to make a website display correctly on mobile devices? 

## CSS

## Javascript / Typescript

1. Which one or more of these data types does not support Typescript?
    1. `number`
    1. `string`
    1. `string[]`
    1. `float`
    1. `integer`
    1. `boolean`
    1. `null`
    1. `undefined`
    1. `void`
    <br>
1. What is a scope in JavaScript?
    <br>
1. How to select a HTML element in DOM?
    <br>
1. What is a promise?
    <br>
1. What are the differences between Arrow functions and Regular functions?

1. Which one or more of declaring a variable is incorrect in Typescript?
    1. `const message: string = 'text';`
    1. `const message: string;`
    1. `const message = 'text';`
    1. `const message;`
    <br>
1. How does JavaScript handle asynchronous calls?
    <br>
1. How does TypeScript support optional parameters in function?
    <br>
1. Explain Decorators in TypeScript.
    <br>
1. What are Generics in TypeScript?
    <br>
1. What are all the access modifiers that TypeScript supports?
    <br>

## React / Redux

1. What types of components exist in React?

1. How do you pass data between React components?

1. What is virtual DOM?

1. What are React hooks and where you can use them? What are hook dependencies?

1. What's a component's lifecycle? Please give examples of lifecycle methods.

1. What are the most common approaches for styling a React application?

1. How do you dispatch an action on redux state.

1. What is the purpose of redux reducers?

1. What are redux sagas and when to use them? 

## PHP

1. Mark **incorrect** option
    1. `<?php echo $value ?>`
    1. `<?= echo $value ?>`
    1. `<?= $value ?>`
    1. `<? echo $value ?>`
    
1. Assign input values with script output
    
**Script**
```
if ($a == $b)
if ($b == $c)
echo '1';
else
echo '2';
```
    
**Inputs**
```
1.) $a=1; $b=1; $c=3;
2.) $a=1; $b=2; $c=3;
3.) $a=1; $b=1; $c=1;
```
    
**Outputs**
```
a.) no output
b.) 1
c.) 2
```

1. Which one **does not** belong to *magic methods*
    1. `__kill`
    1. `__toString`
    1. `__construct`
    1. `__destruct`

1. Which one **is correct** definition of function in PHP
    1. `function foo(PDO $bar) {}`
    1. `def foo($bar) {}`
    1. `function $foo(bar) {}`
    1. `function PDO foo($bar) {}`

1. What will be the output of following code (`mixed strpos ( string $haystack , mixed $needle [, int $offset = 0 ] )`)

```php
$haystack = 'yabadabadoo';
$needle = 'yaba';
if (strpos($haystack,$needle)) {
        echo '"' . $haystack . '" contains "' . $needle . '"';
} else {
        echo '"' . $haystack . '" does not contain "' . $needle . '"';
}
```
    1. No output
    1. Throws an error
    1. "yabadabadoo" contains "yaba"
    1. "yabadabadoo" does not contain "yaba"

1. What is the difference between `Abstract Class` and `Interface`?
1. What are some of the big changes PHP has gone through in the past few years?
1. What is `composer` used for in PHP world?
1. What are the different types of errors in PHP ?
1. How can we get the IP address of the client?

###

### 1.)

Edit class `Foo` so that value of `$bar` can't be empty and will be always lowercase

```php
Class Foo
{
    public $bar;
} 
$foo = new Foo;
$foo->bar='Hello';
```

### 2.)

Change data type of `$array` to `object` .

```php
$array = [
    1, 'a',
    [
        'a' => 'A', 
        'b' => [
            'c' => [
                1, 2, 3,
                'array' => [
                    1, 2, 3, 4,
                    'c' => [
                        1, 2, 3, 4, 5,
                        'object' => [1,2,3,4,5]
                    ]
                ]
            ]
        ]
    ]
];
```

### 3.)

Write a program that prints the numbers from 1 to 100. But for multiples of **three** print `"Fizz"` instead of the number and for the multiples of **five** print `"Buzz"`. For numbers which are multiples of both **three and five** print `"FizzBuzz"`.

### 4.)

Write definition of class `Person` that could be used in following way

```php
$person = Person::make([
    'first_name' => 'Michael', 
    'last_name' => 'Knight', 
    'date_of_birth' => '1949/01/09',
]);

print $person->getFullName();                 // Michael Knight
print $person->getDateOfBirth();              // 1949/01/09
print $person->getDateOfBirth('F j, Y');      // January 9, 1949
```

### 5.)

Correct following code

```php
$result = mysql_query('SELECT * FROM customers WHERE id=' . $_GET['id']);
```

### 6.)

Order first **five** letters in following string in reverse order (keep slashes)

```php
$path = "/a/b/c/d/e/f/g/h/i";
```

<div style="page-break-after: always;"></div>

## Homeworks

### 1.) Calendar

#### Assignment

* Create calendar with possibility of creating, editing, deleting and searching events
* Possibility to define start and end of event (date and time)
* Whole day events
* Repeating events (daily, weekly, monthly, yearly)
* Events per user

#### Rules

* Do not use server side frameworks
* Time limit - **3 days**

#### Notes

* Focus on software architecture, security, user interface and data retention
* Keep in mind clean code and OOP principles
* Preferred technologies - PHP (5.6 / 7), MySQL, CSS 3

#### Solution

* Source code of application (PHP, HTML, JS, CSS, ...)
* Database dump

### 2.) RSS reader

#### Assignment

* Create RSS / Atom feed reader. If multiple users consumes same feed, refresh feed only once
* Registration and login
* Managing of feeds for users (CRUD)
* Listing feed items
** Link to original item
** Searching items
** Paging
** Mark item as read / unread / interesting / custom tags
* Server actualization of items

#### Rules

* Do not use server side frameworks
* Time limit - **3 days**

#### Notes

* Focus on software architecture, security, user interface and data retention
* Keep in mind clean code and OOP principles
* Preferred technologies - PHP (5.6 / 7), MySQL, CSS 3

#### Solution

* Source code of application (PHP, HTML, JS, CSS, ...)
* Database dump

### 3.) Blog

#### Assignment

* Create blogging tool. Articles should have perex and publication date.
* Tagging of articles, searching by tags, tag cloud
* User articles
* Title images for articles
* Article discussions (also for non registered users)

#### Rules

* Do not use server side frameworks
* Time limit - **3 days**

#### Notes

* Focus on software architecture, security, user interface and data retention
* Keep in mind clean code and OOP principles
* Preferred technologies - PHP (5.6 / 7), MySQL, CSS 3

#### Solution

* Source code of application (PHP, HTML, JS, CSS, ...)
* Database dump

### 4.) Guestbook

#### Assignment

* Create guestbook for webpage
* User can leave message with nick
* Time limit for adding two messages by same user
* Disable adding messages with more than 90% similarity to other messages
* Administrator can delete messages
* Limit the number of messages added by one user in one day

#### Rules

* Do not use server side frameworks
* Time limit - **3 days**

#### Notes

* Focus on software architecture, security, user interface and data retention
* Keep in mind clean code and OOP principles
* Preferred technologies - PHP (5.6 / 7), MySQL, CSS 3

#### Solution

* Source code of application (PHP, HTML, JS, CSS, ...)
* Database dump
