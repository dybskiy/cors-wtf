CORS W.T.F.?! or 'What is the best way to play with cors locally?'
========
1.
Install `http-server`:
```bash
npm install -g http-server
http-server --cors
```
2.
Simple example ajax call that requires CORS:
```javascript
$.ajax({
  type: 'GET',
  url: 'https://api.github.com/',
  crossDomain: true
}).done(function (data) {
  console.log(data);
});
```

PS: don't try this with ```url: 'http://www.nytimes.com'``` as you'll spend a lot of time trying to figure out why it's not working, which is the reason for this repo to exist.


## Just works™
