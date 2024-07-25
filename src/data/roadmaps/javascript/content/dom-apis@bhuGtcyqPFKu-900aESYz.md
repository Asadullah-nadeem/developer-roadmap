### 1. **DOM Tree Structure**

The DOM represents the document as a tree structure, where each node is an object representing part of the document. Nodes can be elements, attributes, text, etc.

### 2. **Common DOM APIs**

#### **Selecting Elements**

- **`document.getElementById(id)`**: Returns the element with the specified `id`.
  ```javascript
  const element = document.getElementById('myId');
  ```

- **`document.getElementsByClassName(className)`**: Returns a live HTMLCollection of elements with the specified class name.
  ```javascript
  const elements = document.getElementsByClassName('myClass');
  ```

- **`document.getElementsByTagName(tagName)`**: Returns a live HTMLCollection of elements with the specified tag name.
  ```javascript
  const elements = document.getElementsByTagName('div');
  ```

- **`document.querySelector(selector)`**: Returns the first element that matches the specified CSS selector.
  ```javascript
  const element = document.querySelector('.myClass');
  ```

- **`document.querySelectorAll(selector)`**: Returns a NodeList of elements that match the specified CSS selector.
  ```javascript
  const elements = document.querySelectorAll('div.myClass');
  ```

#### **Manipulating Elements**

- **`element.innerHTML`**: Gets or sets the HTML content inside an element.
  ```javascript
  element.innerHTML = '<p>New content</p>';
  ```

- **`element.textContent`**: Gets or sets the text content inside an element.
  ```javascript
  element.textContent = 'New text content';
  ```

- **`element.setAttribute(name, value)`**: Sets the value of an attribute on the specified element.
  ```javascript
  element.setAttribute('src', 'image.jpg');
  ```

- **`element.getAttribute(name)`**: Gets the value of an attribute on the specified element.
  ```javascript
  const src = element.getAttribute('src');
  ```

- **`element.classList.add(className)`**: Adds a class to the element's list of classes.
  ```javascript
  element.classList.add('newClass');
  ```

- **`element.classList.remove(className)`**: Removes a class from the element's list of classes.
  ```javascript
  element.classList.remove('oldClass');
  ```

- **`element.style.property`**: Gets or sets the value of a CSS property.
  ```javascript
  element.style.backgroundColor = 'blue';
  ```

#### **Creating and Inserting Elements**

- **`document.createElement(tagName)`**: Creates a new element with the specified tag name.
  ```javascript
  const newDiv = document.createElement('div');
  ```

- **`element.appendChild(child)`**: Appends a child node to the element.
  ```javascript
  element.appendChild(newDiv);
  ```

- **`element.insertBefore(newNode, referenceNode)`**: Inserts a new node before a reference node.
  ```javascript
  element.insertBefore(newDiv, existingDiv);
  ```

- **`element.removeChild(child)`**: Removes a child node from the element.
  ```javascript
  element.removeChild(child);
  ```

- **`element.replaceChild(newChild, oldChild)`**: Replaces an old child node with a new child node.
  ```javascript
  element.replaceChild(newDiv, oldDiv);
  ```

#### **Event Handling**

- **`element.addEventListener(type, listener)`**: Adds an event listener to the element.
  ```javascript
  element.addEventListener('click', function() {
      alert('Element clicked!');
  });
  ```

- **`element.removeEventListener(type, listener)`**: Removes an event listener from the element.
  ```javascript
  element.removeEventListener('click', function() {
      alert('Element clicked!');
  });
  ```

#### **Traversal**

- **`element.parentNode`**: Returns the parent node of the element.
  ```javascript
  const parent = element.parentNode;
  ```

- **`element.children`**: Returns a live HTMLCollection of the element's child elements.
  ```javascript
  const children = element.children;
  ```

- **`element.firstChild`**: Returns the first child node of the element.
  ```javascript
  const firstChild = element.firstChild;
  ```

- **`element.lastChild`**: Returns the last child node of the element.
  ```javascript
  const lastChild = element.lastChild;
  ```

- **`element.nextSibling`**: Returns the next sibling node of the element.
  ```javascript
  const nextSibling = element.nextSibling;
  ```

- **`element.previousSibling`**: Returns the previous sibling node of the element.
  ```javascript
  const previousSibling = element.previousSibling;
  ```

### Summary

The DOM API provides a rich set of methods and properties for interacting with and manipulating HTML and XML documents. Understanding these APIs allows developers to create dynamic and interactive web pages by selecting, modifying, creating, and deleting elements, as well as handling events and traversing the DOM tree.


## Resources

- [MDN Web Docs: Document Object Model (DOM)](https://developer.mozilla.org/en-US/docs/Web/API/Document_Object_Model)
- [freeCodeCamp: What is DOM in JavaScript?](https://www.freecodecamp.org/news/what-is-dom-in-javascript/)
- [GeeksforGeeks: DOM - Document Object Model](https://www.geeksforgeeks.org/dom-document-object-model/)
- [W3Schools: JavaScript HTML DOM](https://www.w3schools.com/js/js_htmldom.asp)
```
