# Single Line JavaScript App

Create a server side rendered JavaScript app in a single line of bash, thanks to [Next](https://github.com/zeit/next.js/).

Check out the result here - [single-line-js-app.now.sh/](https://single-line-js-app.now.sh/)

### The line

```
$ mkdir myapp && cd myapp && echo '{ "name": "myapp", "scripts": { "dev": "next" } }' > package.json && npm install next react react-dom --save && mkdir pages && echo 'export default () => ( <div>😀</div> )' > pages/index.js && npm run dev
```

### Explanation

Create application directory

```
$ mkdir myapp
$ cd myapp
```

Create package.json file with `next` script

```
$ echo '{ "name": "myapp", "scripts": { "dev": "next" } }' > package.json
```

Install `next`, `react`, and `react-dom`

```
$ npm install next react react-dom --save
```

Create pages directory for file system routing

```
$ mkdir pages
```

Create index route with basic component

```
$ echo 'export default () => ( <div>😀</div> )' > pages/index.js
```

Run that bad boy 😎

```
$ npm run dev
```

Thanks to @zeit for such an [awesome framework](https://github.com/zeit/next.js).
