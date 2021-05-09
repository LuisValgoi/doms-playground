# Reference
https://www.youtube.com/watch?v=7Tok22qxPzQ&ab_channel=theroadmap

# Challenge
Given the following structure, how the HTML will be able to render a heading?

> It renders through the usage of the DOM!

```html
<!DOCTYPE html>
<html lang="en">
<head>
      <meta charset="UTF-8">
      <meta http-equiv="X-UA-Compatible" content="IE=edge">
      <meta name="viewport" content="width=device-width, initial-scale=1.0">
      <title>Document</title>
</head>
<body>
      <h1>Something</h1>
</body>
</html>
```


# DOM
`Document Object Model` its an in memory representation of out HTML elements in forms of objects and a three.

![image](https://user-images.githubusercontent.com/8363610/117586939-b7ab5d00-b0f1-11eb-8c71-4012280904a7.png)

### DOM API
Its all the methods that we use when we want to query, modify, see objects inside our dom.

Its referenced here: https://dom.spec.whatwg.org/ & https://developer.mozilla.org/pt-BR/docs/Web/API/Document/querySelector

For instance: `document.querySelector('h1').style.fontSize('100px')`

# Shadow DOM

Its a feature that keeps the markup structure, style, and behavior hidden and separate from other code on the page so that different parts do not clash.

For instance, when we want to render a video, how the buttons of `play`, `pause` and `settings` are not appearing?

> It renders through the usage of the SHADOW DOM!

https://developer.mozilla.org/en-US/docs/Web/Web_Components/Using_shadow_DOM

![image](https://user-images.githubusercontent.com/8363610/117587370-00641580-b0f4-11eb-937e-d71bb91a740f.png)

### Shadow DOM in action

You can enable and see the shadow DOM methods and objects by enabling in the Inspector Seetings.

![image](https://user-images.githubusercontent.com/8363610/117587442-5df86200-b0f4-11eb-9fdc-3ffd387ec814.png)

![image](https://user-images.githubusercontent.com/8363610/117587481-85e7c580-b0f4-11eb-9ac2-4e44bfa35d8c.png)


### Shadow DOM Benefits

It let us create custom components (a.k.a: web components) or in other words, create scoped DOM Trees inside our elements.

We can create components which has a specificity and a behavior withouth affect others elements around it and, hidding its structure

For instance: `<video>` its a Web Component.

# Virtual DOM

It's an abstraction on top of the actual DOM where a "virtual" object tree (representation of a UI) is kept in memory and synced with the "real" DOM.

### VDOM Benefits 

Since its a in memory DOM representation, its updates are much quicker then updating the real DOM.

After that, occurs a `reconciliation` action, where it analysis all the places wihch will be affected and syncronize them with DOM.

https://pt-br.reactjs.org/docs/reconciliation.html

https://www.treinaweb.com.br/blog/o-que-e-dom-virtual-dom-e-shadow-dom/