```js
let halley = {
    _name: 'Halley',
    _behavior: 0,

    get name() {
        return this._name;
    },

    get behavior() {
        return this._behavior;
    },

    incrementBehavior() {
        this._behavior++;
    }
}
```
변수에 위와 같이 객체에 상태와 행동을 넣어줄 수 있다.
```js
class Dog {
  constructor(name) {
    this._name = name;
    this._behavior = 0;
  }

  get name() {
    return this._name;
  }
  get behavior() {
    return this._behavior;
  }   

  incrementBehavior() {
    this._behavior ++;
  }
}
```
또한 위와 같이 자바처럼 클래스를 만들 수 있다.

```js
const halley = new Dog('Halley');
console.log(halley.name); // Print name value to console
console.log(halley.behavior); // Print behavior value to console
halley.incrementBehavior(); // Add one to behavior
console.log(halley.name); // Print name value to console
console.log(halley.behavior); // Print behavior value to console
```
자바와 다른 점은 속성을 일일이 모두 명시하지 않고 생성자와 getter를 사용해서
객체에 접근이 가능한 것 같다.

클래스의 constructor() 내의 속성을 생성해준다고 이해하면 된다. [참고](https://www.codecademy.com/courses/learn-intermediate-javascript/lessons/classes/exercises/constructor-method#:~:text=3.-,Inside%20the%20Surgeon%20constructor()%2C%20create%20name%20and%20department%20properties%20and%20set%20them%20equal%20to%20your%20input%20parameters.,-Checkpoint%204%20Passed)

getter는 함수명 앞에 `get`을 붙여야하나보다. 

> 변수의 언더스코어 의미는?
> private 을 뜻하는 네이밍 컨벤션임. [참고](https://stackoverflow.com/questions/8288756/in-javascript-what-does-this-underscore-mean#:~:text=170-,It%20means%20private%20fields%20or%20private%20methods.%20Methods%20that%20are%20only%20for%20internal%20use.,-They%20should%20not)

