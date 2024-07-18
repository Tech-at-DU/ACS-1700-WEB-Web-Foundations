# Project Todo List
The goal of this project is to create a Todo list. You'll use HTML, CSS, and JS. 

The content of the list will be dynamic. You will be able to add new todo items, mark todo items complete, and remove completed todo items. 

## Markup 
The markup for this project can be anything you like, but will better and make more sense if we apply some semantic ideas! 

Imagine todos as a list of names and check marks. The markup might look like this: 

```HTML
<ul>
  <li>
    <span>Feed the Cat</span> 
    <label>
      Completed:
      <input type="checkbox" />
    </label>
    <button>Remove</button>
  </li>
  ...
</ul>
```

Each li block will be repeated for each todo item! 

You might add more properties like date created, and priority. 

To add new todos you'll need a form. Something like this: 

```HTML
<form>
  <label>
    New Todo: 
    <input type="text"/>
    <button>Add new Todo</button>
  </label>
</form>
```

## Styles
This should include using flex or grid to arrange the todo items. 

## JavaScript
To connect the JS you write to the HTML elements you've created you'll need to assign id names to the elements. This is an important step! Not only will it determine whether or not things will work, it will decide how you think about your code! Choosing names that make sense will make your work easier! 

**Naming things is one of the most important steps in software development!**

```html
<form id="add-todo-form">
  ...

<ul id="todo-list">
  ...
```

Get some "references" to these elements in your code: 

```JS
const addTodoForm = document.getElementById('add-todo-form')
const todoList = document.getElementById('todo-list')
```

Spelling matters! The names used as id names need to match the strings here! 

To make your Todo List functional you need create an object that represents a todo item. This will be an object, something like this: 

```JS
{
  name: 'Feed the cat',
  completed: false
}
```

You could add more properties, like the date it was created and priority. You'll need to also include html elements that can be used to display and set these! 

You'll need to define an array to hold a list of your todo items: 

```JS
const todos = [
  {
    name: 'Feed the cat',
    completed: false
  },
  {
    name: 'Walk the dog',
    completed: false
  },
  ...
]
```

To make this functional you need to add new todo objects to the todos array when the form is submitted. Something like: 

```JS

```
