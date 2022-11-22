# Lord of the rings SDK

 Author :Saraan Asim
 Github: saraanasim
 Linkedin: https://www.linkedin.com/in/saraan-asim/

## About

This SDK provides information about the **Lord of the Rings triology, movies, characters , quotes and much more**. All you have to do is to **install the package** and **call the end-points**. This SDK makes use of the api https://the-one-api.dev/. Kindly register and get your api key from here.

## References
This SDK has been made possible because of The One api dev (https://the-one-api.dev/). It has been built on top of it.

## Installation

Please install this SDK by entering this command in console

npm install @saraanasim/lotr-sdk

## Creating an Instance

Create an instance in this way

const client = new LOTR({
  apiKey: "your-api-key",
});

Then use it by calling one of the given Methods.

client
  .getAllChaptersOfSingleBook("6091b6d6d58360f988133bc8")
  .then((res) => {
    console.log("All Books are: ", res);
  })
  .catch((err) => {
    console.log("Encountered error: ", err);
  });
## Methods

There are 5 catagories about which users can get information.

1. **Books**
2. **Movies**
3. **Characters**
4. **Chapters**
5. **Quotes**

- ### Books
* Get all books = getAllBooks()
* Get a single book by id = getBookById(book id (string))
* Get all chapters of a single book = getAllChaptersOfSingleBook(book id (string))
- ### Movies
* Get all movies = getAllMovies()
* Get a single movie by id = getMovieById(movie id (string))
* Get all quotes of a single movie = getAllQuotesOfSingleMovie(movie id (string))
- ### Characters
* Get all characters = getAllCharacters()
* Get a single character by id = getCharacterById(character id (string))
* Get all quotes of a single character = getAllQuotesOfSingleCharacter(character id (string))
- ### Chapters
* Get all chapters = getAllChapters()
* Get a single chapter by id = getChaptersByBookId(chapter id (string))
- ### Quotes
* Get all quotes = getAllQuotes()
* Get a single quote by id = getQuotesById(quote id (string))





