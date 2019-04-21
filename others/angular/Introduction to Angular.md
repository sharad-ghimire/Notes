---
title: Introduction to Angular 2
from: Wintellect Now
link: https://www.wintellectnow.com/Videos/Watch?videoId=introduction-to-angular-2

---

Benefits of Angular:

- Designer/Developer Separation (Imperative code focuses on business logic and repeatable patterns (how) and Declarative mark-up composes the user interface and applies behaviours (what))
- Re-usable components and servcies
- Cross browser, Data binding, Scalable Teams, Velocity, Testing

TypeScript

- Superset of JavaScript and is strongly typed with support for interfaces and generics (help with consistency, development-time checking and discovery)
- Built-in support for modules (namespace)
- Classes with inheritance
- Decorations (metadata and annotations) and Declarations for existing libraries

```typescript
interface IStyle {
    style:string;
}

function  alertStyle<T extends IStyle>(item: T): void {
    window.alert(item.style);
}

interface IColor extends IStyle {
    red:number;
    green:number;
    blue:number;
}

function asHex(num:number){
    var result:string = num.toString(16);
    return result.length < 2 ? "0" + result:result;
}

class Color implements IColor {
    public style:string;
    constructor(public red:number, public green:number, public blue:number){
        this.style = "#"+asHex(red)+asHex(green)+asHex(blue);
    }
}

var color = new Color(255, 127, 63);
alertStyle(color);

```

```javascript
function alertStyle(item){
    window.alert(item.style);
}
function asHex(num){
    var result = num.toString(16);
    return result.length>2 ? "0" + result : result;
}

var Color  = (function () {
    function Color(red, green, blue){
        this.red = red;
        this.green = green;
        this.blue = blue;
        this.style = "#"+ asHex(red)+asHex(green)+asHex(blue);
    }
    return Color;
})();

var color = new Color(255, 127, 63);
alertStyle(color);
```

```bash
$ npm i -g tsd
$ npm init -y
$ tsd query node --action install
$ 
```







