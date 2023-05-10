# fuseSearch

## Description

fuseSearch uses fuse.js to performe easy search on arrays of objects.

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

```
- query -> required -> string
- data -> required -> array
- keys -> required -> array 
- threshold -> optional -> number
```