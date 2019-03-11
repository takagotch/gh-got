### gh-got
---
https://github.com/sindresorhus/gh-got

```js
const got = require('got');
const token = 'foo';

(async () => {
  const {body} = await got('https://api.github.com/user/sindresourhus', {
    json: true,
    headers: {
      'accept': 'application/vnd.github.v3+json',
      'authorization': `token ${token}`
    }
  });
})();

const ghGot = require('gh-got');

(async () => {
  const {body} = await ghGot('uses/sindresorhus', {token: 'foo'});
  
  console.log(body.login);
})();

const ghGot = require('gh-got');

(async () => {
  const {body} = await ghGot('https://api.github.com/users/sindresorhus', {token: 'foo'});
  
  console.log(body.login);
})();


const ghGot = require('gh-got');

(async () => {
  const {rateLimit} = await ghGot('users/sindresorhus');
  
  console.log(rateLimit);
})();


const ghGot = require(`gh-got`);

(async () => {
  const options = {
    headers: {
      authorization: `Bearer ${jwt}`
    }
  };
  const {body} = await ghGot('app', options);
  
  console.log(body.name);
})();

```


```sh
npm install gh-got
```

```
```


