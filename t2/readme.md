
# Playing with static site generators
Using:
- wintersmith
- wintersmith-nunjucks
- wintersmith-livereload
- http://prose.io
```
$ npm install wintersmith -g
$ wintersmith new <path>
$ cd <path>
$ wintersmith preview
$ npm install -g wintersmith-nunjucks
```
To config.json add:
```
"plugins": ["wintersmith-nunjucks"]
```

When done editing:
```
$ wintersmith build
```
To config.json add:
```
"plugins": ["wintersmith-livereload"]
```
To head of  main template (e.g. layout.html) add:
```
{{ env.helpers.livereload() | safe }}
```





