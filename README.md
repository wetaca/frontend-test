# Front-End
Write a front end for this project's API.

It must allow the user to:
- view the available offer (names, prices, photos)
- select which dishes she wants to buy
- review the total amount to be payed

## Sample Server
Sample graphql server to use as a backend for the front-end technical test

## TL;DR
```
npx yarn
node index
```
Server will be running at localhost:4000 and can be queried from the browser
like:
```
const query = `query dishes {
  dishes {
    name
    price
    image
  }
}`

fetch('http://localhost:4000', {
  method: 'POST',
  headers: { 'Content-Type': 'application/json' },
  body: JSON.stringify({ query }),
})
```
Please note this is just an example of usage.
