# fuseSearch

## Description

fuseSearch is a function that utilizes fuse.js library to perform easy search operations on arrays of objects. It is designed to simplify the process of searching and filtering data.

The function performs several validations on the provided arguments to ensure their correctness and validity. These validations help maintain the integrity of the search process.

Upon completion, fuseSearch returns an array of objects in the exact same format as the input array. This ensures consistency and allows for easy integration with existing data structures and workflows.

## Install 

```Javascript
npm i fuse-search
```

## Import

```Javascript
require('fuse-search');
```

## Usage 

```Javascript
const fuseSearch = require('fuse-search');

const query = 'John';
const data = [{name: 'John', age: 18}, {name: 'Alex', age: 21}];
const keys = ['name'];
const threshold = 0.4; 

const search = fuseSearch(query, data, keys, threshold);

console.log(search);

[output] > [{name: 'John', age: 18}];
```

## Arguments

| Argument   | Required | Type   | Description                                      |
|------------|----------|--------|--------------------------------------------------|
| query      | required | string | Represents the query.                            |
| data       | required | array  | Contains the data.                               |
| keys       | required | array  | Specifies the keys.                              |
| threshold  | optional | number | Represents the threshold (default: 0.6).         |


## Repository

[git@github.com:GkChris/fuse-search.git](https://github.com/GkChris/fuse-search.git)

