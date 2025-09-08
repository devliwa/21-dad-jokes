# 21 Dad Jokes Project

A fun JavaScript project that fetches and displays random dad jokes.  
This project is great for practicing API requests, working with JSON data, and updating the DOM dynamically.

---

## Features
- Fetches a new joke at the click of a button  
- Displays jokes in a clean and simple layout  
- Uses a public jokes API for fresh, random jokes  

---

## Built With
- **HTML5** for structure  
- **CSS3** for styling  
- **JavaScript (ES6)** for functionality  
- **Fetch API** for retrieving jokes  

---

## Demo Preview
[21 Dad Jokes Project](https://devliwa.github.io/21-dad-jokes/)
<img width="1279" height="636" alt="Screenshot 2025-09-08 at 11 02 51 AM" src="https://github.com/user-attachments/assets/ad24543a-c017-4689-b2a3-0f6946a7f919" />


---

## What I Learned
- How to use the Fetch API to get data from a public API  
- Parsing and displaying JSON data in the DOM  
- Handling async/await for cleaner asynchronous code  

#### HTML Structure

- div.container
  - button.btn
  - p.result(dummy text)

#### External Data

- the main idea the same, just external data

#### What is an API?

[What is an API?](https://www.freecodecamp.org/news/what-is-an-api-in-english-please-b880a3214a82/)

- https://www.course-api.com/javascript-store-products
- get store products

- https://www.course-api.com/javascript-store-single-product?id=rec43w3ipXvP28vog
- get single store product

- https://randomuser.me/api/
- random user

#### Docs

- important
- search engine
- test in the browser

#### Dad Jokes Docs

- [Dad Jokes](https://icanhazdadjoke.com/api)

- random joke
- https://icanhazdadjoke.com/

#### Select Elements

- select btn, result
- check if both elements selected
- listen for click events

#### FetchDadJoke Function

- create async function
- setup fetch
- set result.textContent = joke

```js
const fetchDadJoke = async () => {
  const response = await fetch(url, {
    headers: {
      Accept: 'application/json',
      'User-Agent': 'learning app',
    },
  });

  const data = await response.json();
  result.textContent = data.joke;
};
```

#### Loading

- set result equal to - 'Loading...'

#### Error Handling

- try/catch block
- set result equal to - 'There was an error..'

#### Check Status

- Fetch - only throws an error if cannot resolve
- Error response still a response
- check response.ok property
- throw new Error('Whoops!')
