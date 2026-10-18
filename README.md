# Python Music Library System

## Description

This project is a Python-based simulation of a music library system. It demonstrates advanced Object-Oriented Programming (OOP) concepts, specifically the use of **Class Attributes** and **Class Methods** to track shared state across multiple instances of a class.

The core of the application is the `Song` class, which not only stores individual song details but also automatically tallies statistics (total songs, unique artists, unique genres, and counts per artist/genre) every time a new song is created.

## Features

When a new `Song` object is instantiated, the following class-level attributes are automatically updated:
**`count`**: Tracks the total number of `Song` objects created.
**`genres`**: Maintains a list of unique genres across all songs.
**`artists`**: Maintains a list of unique artists across all songs.
**`genre_count`**: A dictionary tracking how many songs belong to each genre (e.g., `{"Pop": 3, "Rap": 1}`).
**`artist_count`**: A dictionary tracking how many songs each artist has (e.g., `{"Beyonce": 2, "Jay Z": 1}`).

## Requirements

Python 3.8 or higher
`pytest` for running the test suite

## Installation & Setup

To get this project running on your local machine, follow these steps:

1. **Clone the repository:**

```bash
  git clone https://github.com/YourUsername/python-music-library-system-lab.git
  cd python-music-library-system-lab
```

Set up the environment: (Using Pipenv)

```bash
pipenv install
pipenv shell
```

## Usage & Testing

This lab is test-driven. To verify that the Song class is accurately tracking data, run the test suite from the root directory:

```bash
pytest -x lib/testing/
```

(The -x flag tells pytest to stop after the first failure, which is helpful for test-driven development).

## Completed Work

Below is a screenshot showing all tests passing successfully:

![Screenshot](/img/Screenshot%20From%202026-10-18%2009-56-24.png)

## Contributing

This project was completed as part of a Moringa School Object-Oriented Programming lab.

## License

This project is open-source and available under the MIT License.