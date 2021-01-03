# typescript

https://www.typescripttutorial.net/

### start

install typescript

```
yarn global add typescript
```

check install
```
tsc --v
```

"app.ts" to "app.js"
```
tsc app.ts
```

### default structure


function structure
```javascript
const funcName = (inputParam: type): type => {
    // pass
}
```

example
```javascript
const showData = (name: string, cost: number): number => {
    console.log(`name: ${name} cost: ${cost}`);
    return 1;
}
```

### interface

```javascript
interface Data {
    num1: number,
    num2: number
};

const showData = (name: string, cost: number): Data => {
    console.log(`name: ${name} cost: ${cost}`);

    return {
        'num1': 33, 
        'num2': 44
    };
}
```

### data type

default 

```javascript
let name: string = 'hello';
let age: number = 20;
let big: bigint = 9007199254740991n;
let active: boolean = true;
let test1: undefined;
let test2: null;
```

default array

```javascript
let names: (string)[] = ['1', '2', '3'];
```

dynamic type array

```javascript
let names: (string|number)[] = ['1', '2', 3];
```

tuple  

##### tuple is fixed ordering

```javascript
let names: [string, number] = ['1', 3];
```

any

```javascript
let test: any = 333;
```

void

```javascript
let useless: void;

useless = undefined;
useless = null;
```

fixed type

```javascript
let fixedValue: 333;
fixedValue = 333; // valid
fixedValue = 444; // invalid
```