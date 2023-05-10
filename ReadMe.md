# fuseSearch

## Description

fuseSearch uses fuse.js to performe easy search on arrays of objects.

Several validations are performed on the given arguments in order to validate.

Returns an array of objects in the exact same format as the input array.

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
const threshold = 0.4; // Default 0.6

const search = fuseSearch(query, data, keys, threshold);

console.log(search);

[output] > [{name: 'John', age: 18}];
```

## Arguments 

- query -> required -> string
- data -> required -> array
- keys -> required -> array 
- threshold -> optional -> number

## Repository

[git@github.com:GkChris/fuse-search.git](https://github.com/GkChris/fuse-search.git).

