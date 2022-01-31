# jest-fs

Node.js fs module mock for Jest unit testing.

## Usage

```js
const jestFs = require("./jest-fs");

for (let i = 0; i <= 10; i += 1) {
  jestFs.writeFileSync(`path/to/file${i}.js`, 'console.log("test")');
}

const files = jestFs.readdirSync('path/to');

console.log(files);
```