# Todo List App

## Welcome! 👋

## Table of contents

- [Overview](#overview)
  - [The Challenge](#the-challenge)
  - [How to Setup the Project](#how-to-setup-the-project)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My Process](#my-process)
  - [Built With](#built-with)
  - [What I Learned](#what-i-learned)
  - [Continued Development](#continued-development)
  - [Useful Resources](#useful-resources)
- [Author](#author)
- [Acknowledgments](#acknowledgments)
- [Got Feedback for Me?](#got-feedback-for-me)

## Overview

### The Challenge

Manage your tasks efficiently with our interactive Todo List app! 

This user-friendly frontend application allows users to:
- View an optimal layout depending on their device's screen size.
- See hover states for interactive elements.
- Perform actions such as adding new todos, marking them as complete, deleting them, filtering by status (all/active/complete), clearing completed todos, and toggling between light and dark mode.
- Drag and drop to reorder items on the list.

### How to Setup the Project

To set up the project locally, follow these steps:

1. Clone the repository using GitHub Desktop or Git Bash:
    ```bash
    git clone https://github.com/soumya-123-code/Todo-app_frontend_project.git
    ```
2. Open the project folder in your code editor.
3. Run the project using a live server extension or deploy it using Netlify, Vercel, or another web hosting service.

### Screenshot

![Design Preview](./design/active-states-dark.jpg)

### Links

- Solution URL: [GitHub Repository](https://github.com/soumya-123-code/Todo-app_frontend_project)
- Live Site URL: [Live Site](https://todo-list-project-application.netlify.app/)

## My Process

### Built With

- HTML5
- CSS3
- JavaScript

All required assets are in the `/design` folder. The `style-guide.md` file contains details such as color palette and fonts.

### What I Learned

This project enhanced my understanding of implementing CRUD operations in web applications. The logic can be adapted to any tech stack. Here's an example:

```js
function removeTodo(e) {
  if (e.target.nodeName !== "IMG") return;
  const removedItem = e.target.parentNode.previousElementSibling.children[2].textContent;
  todoArray = todoArray.filter((todo) => todo.todoItem !== removedItem);

  if (window.confirm(`Are you sure you want to delete: ${removedItem}`)) {
    e.target.parentNode.parentNode.remove();
    handleEmptyMessage();
    getTodoCount();
  } else return;
  saveToLocalStorage(todoArray);
}
```

### Continued Development

This project highlighted areas where I can improve:
- Mastering CSS Flexbox and Grid for layout structuring.
- Deepening my understanding of `fetch` and `async/await` in JavaScript.
- Implementing state management for larger applications.

By focusing on these areas, I aim to enhance my skills and become a better full-stack developer.

### Useful Resources

- [Harkirat Singh Course Notes](https://github.com/soumya-123-code/harkirat-singh-course_code_and_notes) - Comprehensive notes from all lectures, including code snippets and insights.
- [My Development Notes](https://github.com/soumya-123-code/cwh-web-dev-playlist_code_and_notes) - Notes from my early development days. Star the repository if you find it useful! ✨💫
- [MDN Hover State Documentation](https://developer.mozilla.org/en-US/docs/Web/CSS/:hover) - A valuable resource for understanding CSS hover states.

## Author

**Soumya Ranjan Nayak**

- Website - [Soumya Ranjan Nayak](https://soumya-123-code.github.io/itsmesoumya)
- LeetCode - [@soumya_ranjan](https://leetcode.com/u/soumya_ranjan/)
- LinkedIn - [Soumya Ranjan Nayak](https://www.linkedin.com/in/soumya-ranjan-nayak-50069a15a)

## Acknowledgments

A huge thank you to the open-source community and developers who provide free learning resources and support through forums and discussions.

## Got Feedback for Me?

I love receiving feedback! If you have suggestions or ideas, feel free to reach out via email at soumya050794[at]gmail[dot]com.

If you enjoyed this project, consider sharing it with others.

**Stay organized and productive!** 📝✅

