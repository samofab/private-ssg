
# Playing with static site generators
Using:
- wintersmith
- wintersmith-nunjucks
- wintersmith-livereload
- http://prose.io
```
$ npm install -g wintersmith
$ npm install -g wintersmith-nunjucks 
$ npm install -g wintersmith-livereload 
$ wintersmith new <path>
$ cd <path>
$ wintersmith preview
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





