```js
let user = {
  name: 'Arya',
  sibling: ['Robb', 'Ryan', 'John'],
};
let allBrothers = ['Robb', 'Ryan', 'John'];
let brothersCopy = user.sibling;
let usename = user.name;
let newUser = user;
```

1. Memory representation

- Create the memory representation of the above snippet on notebook.
- Take a photo/screenshot and add it to the folder `code`

<!-- To add this image here use ![name](./hello.jpg) -->
`![name](./hello.jpg)`
2. Answer the following with reason:

- `user == newUser;` // true Both are using same address to access the same data and both are non-primitive
- `user === newUser;`// true  Both are using same address to access the same data and both are non-primitive
- `user.name === newUser.name;`// true  Both are using same address to access the same data and both are non-primitive
- `user.name == newUser.name;`// true  Both are using same address to access the data and both are non-primitive
- `user.sibling == newUser.sibling;`// true  Both are using same address to access the same data and both are non-primitive
- `user.sibling === newUser.sibling;`// true  Both are using same address to access the same data and both are non-primitive
- `user.sibling == allBrothers;` //false Both are having different address 
- `user.sibling === allBrothers;` //false Both are having different address 
- `brothersCopy === allBrothers;` //false Both are having different address 
- `brothersCopy == allBrothers;` //false Both are having different address 
- `brothersCopy == user.sibling;`//true Both are using same address to access the data and both are non-primitive
- `brothersCopy === user.sibling;`// true Both are using same address to access the same data and both are non-primitive
- `brothersCopy[0] === user.sibling[0];`// true Both are using same address to access the data and both are non-primitive
- `brothersCopy[1] === user.sibling[1];` // true Both are using same address to access the data and both are non-primitive
- `user.sibling[1] === newUser.sibling[1];`// true Both are using same address to access the data and both are non-primitive
 