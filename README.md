# Project Title: Library of Congress API

One Paragraph of the project description

Initially appeared on
[gist](https://gist.github.com/PurpleBooth/109311bb0361f32d87a2). But the page cannot open anymore so that is why I have moved it here.

## Authors

  - **Billie Thompson** - *Provided README Template* -
    [PurpleBooth](https://github.com/PurpleBooth)

See also the list of
[contributors](https://github.com/PurpleBooth/a-good-readme-template/contributors)
who participated in this project.


## Getting Started

These instructions will give you a copy of the project up and running on
your local machine for development and testing purposes. See deployment
for notes on deploying the project on a live system.

### Prerequisites

Requirements for the software and other tools to build, test and push 
- [Example 1](https://www.example.com)
- [Example 2](https://www.example.com)

### Installing

A step by step series of examples that tell you how to get a development
environment running

Say what the step will be

    Give the example

And repeat

    until finished

End with an example of getting some data out of the system or using it
for a little demo

The completed application should meet the following criteria:

* As a user, I can submit a search query from the application to request data and receive a response from the Library of Congress.

* As a user, I can either perform a generic search for data in all formats or I can select a format in the form to help filter results.

* As a user, I can see all of the results of my search displayed on a separate page.

* As a user, I can conduct additional searches from the results page as well.

To learn about how to use this API, check out the Requests section of the [Library of Congress API documentation](https://libraryofcongress.github.io/data-exploration/).

### The Homepage

The homepage (`index.html`) should have the following:

* A simple, well thought-out UI.

* A form with a text input field to capture a search query and an option select dropdown to capture the format of the search query. The options in the dropdown should be a list of the possible format values listed in the [Library of Congress API documentation on requests](https://libraryofcongress.github.io/data-exploration/requests.html#format).

* A browser event listener attached to the form to execute a function on submission, which will capture both form values and redirect the user to a search results page with those values included in the URL as query parameters. This will use the browser's `location.replace()` method.

* If there is no format selected from the dropdown, the URL should look something like the following example:

  ```http
  /search-results.html?q=dogs&format=
  ```

* If there is a format selected from the dropdown, the URL should look something like the following example:

  ```http
  /search-results.html?q=dogs&format=photos
  ```

### The Search Results Page

The search results page (`search-results.html`) should have and do the following:

* On page load, if there are query parameters, immediately parse them and use them in a request URL to fetch data from the Library of Congress API.

* If there is a value for the format query parameter, use the format endpoint to search for something based on the chosen format. For more information, see the [Library of Congress API documentation on the format endpoint](https://libraryofcongress.github.io/data-exploration/requests.html#format).

* If there is no value for the format query parameter, use the search endpoint to search for all types of data. For more information, see the [Library of Congress API documentation on the search endpoint](https://libraryofcongress.github.io/data-exploration/requests.html#search).

* The response from the API request will then be displayed on the page. It is up to you and your team to determine which data should be displayed from the overall `response` object, but you must use data from the `results` property in the `response` object. For more information, see the [Library of Congress API documentation on responses](https://libraryofcongress.github.io/data-exploration/responses.html).

* The same form from the homepage should be here as well. Instead of redirecting a user to another page, however, it will perform a search right on the page and display the new results.

## Assets

The following image demonstrates the homepage's appearance and functionality:

![The home page shows a search bar with the ability to select a format from a dropdown menu.](./Images/01-homepage.png)

The following image demonstrates the search results page's appearance and functionality:

![The search results page displays results from a search conducted in the form on the left side of the page.](./Images/02-search-results-page.png)

## Deployment

Add additional notes to deploy this on a live system

## Built With

  - [Contributor Covenant](https://www.contributor-covenant.org/) - Used
    for the Code of Conduct
  - [Creative Commons](https://creativecommons.org/) - Used to choose
    the license

## Contributing

Please read [CONTRIBUTING.md](CONTRIBUTING.md) for details on our code
of conduct, and the process for submitting pull requests to us.

## Versioning

We use [Semantic Versioning](http://semver.org/) for versioning. For the versions
available, see the [tags on this
repository](https://github.com/PurpleBooth/a-good-readme-template/tags).

## Acknowledgments

  - Hat tip to anyone whose code is used
  - Inspiration
  - etc


