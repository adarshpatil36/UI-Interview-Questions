# UI Interview Questions

### React<br/>
- Code Splitting<br/>
- New features of React<br/>
- Will component did mount  be called on every rerender<br/>
- Alternative for redux<br/>
- -> Mobex<br/>
- Drawback of redux<br/>
- What is react uni-directional data flow?<br/>
- It is possible to make bi-directional flow in react ?<br/>
- Explain context overview along with its proper use<br/>
- Actions are synchronous<br/>
- Why do we need to return a new state from the reducer instead of changing the existing one.<br/>
- What are Error Boundaries<br/>
- -> Error Boundaries to handle error at global level and to handle errors at component level we have error handling lifecycle methods<br/><br/>
- And what is component did catch?<br/>
-  Difference between useContext & redux.<br/>
-  Make redux actions async without using Thunk and Saga.<br/>
- Life cycle methods.<br/>
- Name some of the patterns you react usages?<br/>
- Can we update state without using setstate?<br/>
- How can we ensure that the state updated in setstate is previous state only?<br/>
- Does setstate ensures synchronous update of state?<br/>
- How to use a call back inside setstate?<br/>
- What are react hooks useEffect(),useState(),useRef(),useContext(), useSelectors?<br/>
- How to implement inversion of control in react?<br/>
- What are controlled inputs and what are uncontrolled inputs?<br/>
- What is reconciliation in react?<br/>
- How to share data across the components using context api and also using render props?<br/>
- What are prop types in react?<br/>
- How can you pass props from child to parent component?<br/>
- How to use createRef() in react?<br/>
- What is a pure function?<br/>
- What is an HOC (higer order component)? Give an example of any HOC you have
implemented in your project?<br/>
- What is lazy loading in react?<br/>
- What all can be done inside the render() method?<br/>
- Why there is a different package called as react dom?<br/>
- What is a middleware?<br/>
- Tell me what is redux thunk and why there is a need to use thunk or any middleware?<br/>
<br/>

### JavaScript
- What are Interceptors (VIMP Question)<br/>
- Explain various Design Patterns and which patterns are you using in your project and why<br/>
- Controlled vs uncontrolled components<br/>
- Promise vs async await<br/>
- -> async await uses generators internally<br/>
- Ways to force update the state<br/>
- -> setState uses observables internally to re-render the data<br/>
- Event Loop explanation in case of executing async function and what happens when it encounters the await keyword<br/>
- Drawback of arrow functions<br/>
- Different ways to create objects<br/>
- Explain prototypical inheritance in deep with example<br/>
- ES6 Features<br/>
- Copying of Objects<br/>
- Currying Functions<br/>
- Throttling and Debouncing<br/>
- Promise.race() and all functions related to Promise<br/>
- How to run ‘use strict’ code in chrome console<br/>
- -> Use IFFY<br/>
- JIT compiler concept<br/>
- CORS<br/>
- CSRF<br/>
-  What are closures and give an example of any inbuilt function in JS which uses closures concept.<br/>
-  Achieving spread operator functionality without using spread operator.<br/>
-  Axios vs fetch<br/>
<br/>

### CSS<br/>
- Different types of positions and display<br/>
- -> Sticky: Fixed + Relative<br/>
- Difference between inline, inline-block display<br/>
- Ways to place a box at the center of the screen<br/>
- Explain Box Modal in detail<br/>
- What new things are introduced in the css3 version also which is the latest css version and why are we not using the latest css version.<br/>
- Explain all specificity rules in css in detail with example<br/>
- Difference between justify content and align content in terms of axis<br/>
- Explain shadow dom<br/>
- Explain box sizing<br/>
- Line height property<br/>
- Example of different types of libraries equivalent to css<br/>
- -> LESS and SCSS (Css preprocessors)<br/>
- Explain use and features of CSS preprocessors<br/>
- Pseudo elements vs Pseudo Classes<br/>
- Use of Pseudo elements vs Pseudo Classes also give examples of it<br/>
- Types of css selectors<br/>
- Difference between grid and flex and which is better to use<br/>
- What are media queries and may ask you to write one of them<br/>
- Visibility hidden and display none difference<br/>
- Give examples of css combinators<br/>
<br/>

### HTML<br/>
- New tags introduced in html5<br/>
- What will get rendered if I place footer and then header tag<br/>
- (header and then footer or vice versa)<br/>
- What do you mean by semantic tags<br/>
- Name some of the semantic tags<br/>
- Different types of storages in html5<br/>
- Difference between session storage, local storage and cookies<br/>
- Which is the recommended way to store api key or any authentication key<br/>
- Figure sourceset Tag<br/>
- Meta tag in html and its use<br/>
- Inline vs block tag (conceptual difference)<br/>
- Examples of Inline and block tag<br/>
- Explain different HTTP methods<br/>
- Difference between PUT vs POST<br/>
- Give examples of idempotent http methods and what does this idempotent mean<br/>
- What is accessibility and how will you achieve it<br/>

### Code Snippets<br/>

```
let name ="Helllo"
function myFunc(){
    let name ="Test"
    console.log(this.name) // undefined 
}
myFunc()
```
<br/>

```
var obj = {
    name: "Google",
    getName: ()=>{
            console.log(this.name) // undefined
    }
}
obj.getName()
```
<br/>

```
var obj = {
    name: "Google",
    getName: function(){
            console.log(this.name) // Google
    }
}
obj.getName()
```
<br/>

```
var obj = {}
obj[{key:"name"}] = "Adarsh"
obj[{key:"surname"}] = "Patil"
console.log(obj[{key:"name"}]) // Patil
```
<br/>

```
var arr = [10, 2, 30, 23, 32];
console.log(typeof arr); // Object
```
<br/>

```
console.log(1<2<3);
console.log(3>2>1);
```
<br/>

```
var a = 10;
(function(){
    console.log(a);
    var a = 20;
})();
```
<br/>

```
console.log(true + true);
console.log(true + false);
```
<br/>

```
var a = {name: 'React', age:8}
var b = {name: 'React', age:8}
console.log(a==b)
console.log(a===b)
```
<br/>

```
var a = {label: 'a'};
var b = {label: 'b'};
m[a] ='x';
m[b] = 'y';
```
<br/>

```
var obj1 = {a: 10};
var obj2 = obj1;
obj2.a = 90;
console.log(obj1.a)
```
<br/>

```
var x = 10;
(function(){
delete x;
return x;
})();
```
<br/>

```
var arr = [1, 2, 3, 4, 6, 7];
arr[10] = 99;
delete arr[10];
console.log(arr.length)
```
<br/>

```
(function(){
var a = b = 3;
})
console.log(a);
```
<br/>

```
var name = "Adarsh"
function outer(){
    function inner(){
        console.log(this.name) // Adarsh
    }
  inner();
}
outer();
```
<br/>

```
['1', '7', '11'].map(parseInt) // [1,NaN,3]
```
<br/>

```
arr = [1,5,6,1,0,1];
console.log(arr+99) // 1,5,6,1,0,199
```
<br/>

```
let obj ={}
obj[[]] = 12
obj[[[]]] = 80

console.log(obj[[]],obj[[[]]])  // 80 80
```
<br/>

```
var b=1;
function outer(){
  var b=2
     function inner(){
        b++;
        var b=3;
        console.log(b)  // 3
    }inner();
}outer();

```
<br/>
It's all about two queues in JS <br/>
- MacroTask (Default One) <br/>
- Microtask (Callbacks/async calls) <br/> <br/>

Note: setTimeout() lies in the macrotask

```
const promise1 = new Promise((resolve, reject) => {
  console.log(1);
  resolve('success')
});
promise1.then(() => {
  console.log(3);
});
console.log(4);

// 1 4 3
```
<br/>

```
const promise1 = new Promise((resolve, reject) => {
  console.log(1);
});
promise1.then(() => {
  console.log(3);
});
console.log(4);

// 1 4
```
<br/>

```
const promise1 = new Promise((resolve, reject) => {
    console.log(1)
    resolve('resolve1')
})
const promise2 = promise1.then(res => {
    console.log(res)
})
console.log('promise1:', promise1);
console.log('promise2:', promise2);

//  Try it out 😜
```
<br/>

```
const fn = () => (new Promise((resolve, reject) => {
    console.log(1)
    resolve('success')
}));

fn().then(res => {
    console.log(res)
});

console.log(2)

// 1 2 success
```
<br/>

```
console.log('start')
setTimeout(() => {
    console.log('setTimeout')
})
Promise.resolve().then(() => {
    console.log('resolve')
})
console.log('end')

// start end setTimeout resolve
```
<br/>

```
const promise = new Promise((resolve, reject) => {
    console.log(1);
    setTimeout(() => {
        console.log("timerStart");
        resolve("success");
        console.log("timerEnd");
    }, 0);
  console.log(2);
});

promise.then((res) => {
  console.log(res);
});

console.log(4);

// 1 2 4 timerStart timerEnd success
```
<br/>

```
const timer1 = setTimeout(() => {
    console.log('timer1');

const timer3 = setTimeout(() => { 
    console.log('timer3')
  }, 0)
}, 0)

const timer2 = setTimeout(() => {
  console.log('timer2')
}, 0)

console.log('start')

// start timer1 timer2 timer3
