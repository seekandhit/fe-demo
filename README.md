# SeekandHit FE Position Demo Project

Base project for job candidates applying for frontend developer position at [Seekandhit](https://seekandhit.com/).

## Project goal

This project is an opportunity to demonstrate both your development skills and your determination to get a job done right. The task is to build a generic `Autocomplete` component. You should design its API based on these requirements:

- component has a default style, but it can be extended through props
- client provides either a list of items to search through, or a search function and a search results object
- search items can be an array of strings or objects
- in case of objects, client must provide getter functions to determine which property to use as a label, and which property to use as search value
- it can be used **uncontrolled**: client provides a list of items to search in, optional getter functions as described above, and a callback when a value is selected from the list. Default search function is used internally to pick a search result from the provided list.
- it can be used **controlled**: client provides a custom search function (instead of a list of search items) and a list of search results. Custom search function will be used instead of the default one, and component will display the results passed as props.

A complete solution would include both the implementation of the component and a few examples demonstrating the controlled and uncontrolled use cases. Bonus points are awarded if the custom search function is async. Feel free to style the component as you see fit.

Third party packages can be used, as long as they don't help with rendering. Meaning it is OK to use a package for [fuzzy filtering](https://www.npmjs.com/package/fuse.js), but it is not OK to use complete or half-complete dropdown components like [downshift](https://www.npmjs.com/package/downshift).

## Criteria

When reviewing your solution, we will pay attention to these kind of details:

- component behavior
- potential performance issues
- code readability
- component API design & documentation
- test coverage

## Development

Fork this repo and install the dependencies using `npm i`. This project was bootstrapped with [Create React App](https://github.com/facebookincubator/create-react-app), so all the available documentation applies to this project too. Base scripts are:

- `npm start` - start the dev server
- `npm run build` - build the production version of the app
- `npm test` - run the tests in interactive mode
