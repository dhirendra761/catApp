## RECIPE SELECTION PAGE

## OVERVIEW & PROBLEM

Provide the user a way for them to select 3 cats to form a clowder. When the
user selects a cat, it should look like this. The user should also have the
ability to unselect a cat. Once the user has selected a clowder (a group of 3
cats), a function of your own implementation should provide a response to tell
you whether the one selected is a valid clowder like the one in the
representative the endpoint below: 
GET _http://quantcats.herokuapp.com/clowder?cat=<id1>&cat=<id2>&cat=<id3>_ Example:

  **http://quantcats.herokuapp.com/clowder?cat=1ttg&cat=2wsb&cat=3brr**

{ 
  valid: true, 
  id: "1ttg,2wsb,3brr" 
}

## SOLUTION

the solution is done using react hooks. There further areas of improvment in
solution:

- useClowderManagement can be better managed using useReducer
- utilities function can be used so as to test the functions in custome hook
  which are not exposed by the hook
- usability can be improved masking the user interaction when a request is in
  progress

## INSTRUCTIONS

1. Clone this repository
   `git clone https://github.com/hellofreshdevtests/dhirendra761-recipe-selection-react-test.git`
2. Install the dependencies using `npm install`
3. Run the dev server `npm start`
4. Then access http://localhost:3000/

## TEST

All the tests are available in same folders around the files. There is unit
tests for the validators and snapshot tests for the components.

To run the tests use: `npm run test`

## CONTRIBUTOR

- Dhirendra Singh <dhirendrasingh.822@gmail.com>

## REMARK

This project was bootstrapped with
[Create React App](https://github.com/facebook/create-react-app).
