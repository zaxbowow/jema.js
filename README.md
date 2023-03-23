# schema.js
JSONSchema validator

## Features

🚀 Performant  
🕊️ Lightweight (< 4kb brotli)  
🤝 Works in the Browser (deno should work too, not yet tested)  
📦 No dependencies  
🆗 JSONSchema draft-2020-12 (only this)  

## Ussage

```javascript
const schema = new Schema({ type: 'number' });
await schema.deref(); // Dereference remote schemas


schema.validate(3) // true
schema.validate('3') // false

schema.error('3') // get first error (stops on first error)
schema.errors('3') // all errors (iterator);
```

## Install

```javascript
import {Schema} from '../schema.js';
```

## Todo

- Better error messages (with schema path)  
- Fix a few bugs in the test suite: [link](https://rawcdn.githack.com/nuxodin/schema.js/d640d0ec40a42343367bc3fafc566010edb53947/tests/test-suite.html)

## About

- MIT License, Copyright (c) 2022 <u1> (like all repositories in this organization) <br>
- Suggestions, ideas, finding bugs and making pull requests make us very happy. ♥
