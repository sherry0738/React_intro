# [React Workshop Intro](https://github.com/sherry0738/React_intro)
### Setup
We use React and ES6 and JSX in a normal index.html file with no npm or webpack in sight.

1. Make `hello world` displays on the browser with only html. Maybe something more. like creating a Person Card

```js

    <div className="person">
      <h1>Sherry</h1>
      <p>Position: dev intern</p>
    </div>
     <div className="person">
      <h1>XXX</h1>
      <p>Position: OOOOO</p>
    </div>
```

2. Add a reference to an external library by using CDN when experimenting with a new library, like our case here. so remove the html element added above and replace it with the following:

```js

<div id="d1"></div>
<script src="https://cdnjs.cloudflare.com/ajax/libs/react/15.4.2/react.js"></script>
<script src="https://cdnjs.cloudflare.com/ajax/libs/react/15.4.2/react-dom.js"></script>
<script src="https://cdnjs.cloudflare.com/ajax/libs/babel-standalone/6.21.1/babel.min.js"></script>
<script type="text/babel">

function PersonCard() {
  return (
  	<div>
      <div class="person">
        <h1>Sherry</h1>
        <p>Position: dev intern</p>
      </div>
       <div class="person">
        <h1>XXX</h1>
        <p>Position: OOOOO</p>
      </div>
   </div>
  );
}
</script>
```

Maybe some CSS styling to make our person cards looks better:

```css
.person {
  display: inline-block;
  margin: 10px;
  border: 1px solid #ccc;
  box-shadow: 0 2px 2px #eee;
  width: 200px;
  padding:20px;
  background-color: aqua;
}
```

3.Now you just created a reuseable component `PersonCard` after using reactDOM to render code to the browser, let's make it even better to help you understand this all about. 

```js 

var app = (
<div>
    <PersonCard name="Sherry" position="dev intern"/>
    <PersonCard name="XXX" position="OOOOO"/>
  </div>
);

ReactDOM.render(app, document.querySelector('#app'));
```
4.Done :)
