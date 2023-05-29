# HTML Interview Questions And Answers

Most targeted up-to-date HTML interview questions and answers list

# Table of Contents

1. [What is the HTML5 doctype declaration?](#1-what-is-the-html5-doctype-declaration)
2. [What are semantic elements in HTML5?](#2-what-are-semantic-elements-in-html5)
3. [How do you embed a video in HTML?](#3-how-do-you-embed-a-video-in-html)
4. [How do you use local storage in HTML5?](#4-how-do-you-use-local-storage-in-html5)
5. [How do you implement drag and drop functionality in HTML?](#5-how-do-you-implement-drag-and-drop-functionality-in-html)
6. [How do you implement responsive images in HTML?](#6-how-do-you-implement-responsive-images-in-html)
7. [How do you create a progress bar in HTML?](#7-how-do-you-create-a-progress-bar-in-html)
8. [How do you embed an audio file in HTML?](#8-how-do-you-embed-an-audio-file-in-html)
9. [How do you create a tooltip in HTML?](#9-how-do-you-create-a-tooltip-in-html)
10. [How do you implement form validation in HTML?](#10-how-do-you-implement-form-validation-in-html)
11. [How do you include an external HTML file in another HTML file?](#11-how-do-you-include-an-external-html-file-in-another-html-file)
12. [How do you create a responsive navbar in HTML and CSS?](#12-how-do-you-create-a-responsive-navbar-in-html-and-css)
- [Whats more?](#whats-more)
- [Contributing](#contributing)
- [License](#license)

## 1. What is the HTML5 doctype declaration?

The HTML5 doctype declaration is <!DOCTYPE html>. It is used to specify that the document is written in HTML5.

Example:

```html
<!DOCTYPE html>
<html>
  <head>
    <title>HTML5 Document</title>
  </head>
  <body>
    <!-- Content goes here -->
  </body>
</html>
```

## 2. What are semantic elements in HTML5?

Semantic elements in HTML5 provide a meaning to the structure of a web page. They define the purpose and role of the content, making it more accessible and SEO-friendly. Some examples of semantic elements are <header>, <nav>, <section>, <article>, <footer>, etc.

Example:

```html
<header>
  <h1>Website Header</h1>
</header>
<section>
  <h2>About Us</h2>
  <p>Content goes here.</p>
</section>
<footer>
  &copy; 2022 Your Website
</footer>
```
  
## 3. How do you embed a video in HTML?
  
To embed a video in HTML, you can use the <video> tag and specify the video source using the <source> tag within it.
  
Example:

```html
<video controls>
  <source src="video.mp4" type="video/mp4">
  Your browser does not support the video tag.
</video>
```
  
## 4. How do you use local storage in HTML5?
  
Local storage in HTML5 allows web applications to store data locally on the user's browser. You can use the localStorage object to set and retrieve values.
  
Example:

```html
<script>
  // Store a value in local storage
  localStorage.setItem('key', 'value');

  // Retrieve a value from local storage
  var storedValue = localStorage.getItem('key');

  // Remove a value from local storage
  localStorage.removeItem('key');
</script>
```
  
##  5. How do you implement drag and drop functionality in HTML?
  
To implement drag and drop functionality, you can use the HTML5 Drag and Drop API. It involves handling events like dragstart, dragover, and drop.
  
Example:

```html
<div id="dragElement" draggable="true">Drag me</div>
<div id="dropZone">Drop here</div>

<script>
  var dragElement = document.getElementById('dragElement');
  var dropZone = document.getElementById('dropZone');

  dragElement.addEventListener('dragstart', function(event) {
    event.dataTransfer.setData('text/plain', 'Data to be dropped');
  });

  dropZone.addEventListener('dragover', function(event) {
    event.preventDefault();
  });

  dropZone.addEventListener('drop', function(event) {
    var data = event.dataTransfer.getData('text/plain');
    console.log('Dropped data:', data);
  });
</script>
```
  
## 6. How do you implement responsive images in HTML?
  
To implement responsive images, you can use the <picture> element along with the <source> element to provide different image sources based on the device's screen size.
  
Example:

```html
<picture>
  <source srcset="image-lg.jpg" media="(min-width: 1200px)">
  <source srcset="image-md.jpg" media="(min-width: 768px)">
  <img src="image-sm.jpg" alt="Responsive Image">
</picture>
```
  
## 7. How do you create a progress bar in HTML?
  
To create a progress bar, you can use the <progress> tag and specify the current value and maximum value using the value and max attributes, respectively.
  
Example:

```html
<progress value="50" max="100"></progress>
```
  
## 8. How do you embed an audio file in HTML?
  
To embed an audio file in HTML, you can use the <audio> tag and specify the audio source using the <source> tag within it.
  
Example:

```html
<audio controls>
  <source src="audio.mp3" type="audio/mp3">
  Your browser does not support the audio tag.
</audio>
```
  
## 9. How do you create a tooltip in HTML?
  
To create a tooltip, you can use the <span> tag with a title attribute containing the tooltip text. You can style it using CSS.
  
Example:

```html
<span title="Tooltip Text">Hover over me</span>
```
  
## 10. How do you implement form validation in HTML?
  
Form validation in HTML can be implemented using the required attribute and various input types like email, number, pattern, etc.
  
Example:

```html
<form>
  <label for="email">Email:</label>
  <input type="email" id="email" name="email" required>

  <input type="submit" value="Submit">
</form>
```
  
## 11. How do you include an external HTML file in another HTML file?
  
To include an external HTML file, you can use the HTML iframe element or server-side technologies like PHP or SSI (Server Side Includes).
  
Example using iframe:

```html
<iframe src="external.html"></iframe>
```
  
## 12. How do you create a responsive navbar in HTML and CSS?
  
To create a responsive navbar, you can use HTML for the structure and CSS for styling. CSS media queries can be used to adjust the layout based on different screen sizes.
  
Example:

```html
<nav>
  <ul>
    <li><a href="#">Home</a></li>
    <li><a href="#">About</a></li>
    <li><a href="#">Contact</a></li>
  </ul>
</nav>
```
  
CSS:

```css
nav {
  background: #333;
  padding: 10px;
}

ul {
  list-style-type: none;
  margin: 0;
  padding: 0;
}

li {
  display: inline;
  margin-right: 10px;
}

a {
  color: #fff;
  text-decoration: none;
}
```
  
## What's more?
<a href="https://interviewplus.ai/developers-and-programmers/html/questions">A comprehensive list of questions and answers</a>

## Contributing
We welcome contributions from our users to help make this resource as comprehensive and useful as possible. If you have been recently interviewed and encountered a question that is not currently covered on our website, feel free to suggest it as a new question. Your contributions will be added to our platform, and we will make sure to credit you for your contributions. We appreciate your help in making our platform a valuable tool for all job seekers.

## License
MIT License
