## README #
* This README is a note that I wrote when I learned about HTML. I just recorded the necessary knowledge for me.

## What is this repository for? #
* Quick summary about HTML and challengces
* Learn at: https://www.lynda.com/Web-Development-tutorials/HTML-Essential-Training/170427-2.html

## 1. Introducing HTML
### The importance of HTML
- HTML provides the essential structure for web pages
- It's a markup language
- HTML uses tags to identify page content.

### Basic HTML syntax
- Elements refers the tags and their contents.
- Elements can have certain attributes.
- Nesting one element inside of another one.

### The current state of HTML
### HTML resources:
- W3Cs
- whatwg.org
- webplatform.org

### Chosing a  Code Editor:
- Dream Weaver, Coda, Sublime,..

## 2. Basic Page Structure:

## 3. Formatting page content:
- <br> : no end tag, line break
  
## 4. Structure
	<body>
		<header role="banner">
			<nav role="navigation"></nav>
		</header>

		<main role="main">
			<article>
				<header></header>
				<section></section>
				<section>
					<aside> </aside>
				</section>
				..
			</article>
		</main>

		<footer role="contentinfo"></footer>
	</body>

- The <aside> tag defines some content aside from the content it is placed in. The aside content should be related to the surrounding content.
- Description Lists: 
	<dl>
	<dt> </dt> : title
	<dd> </dd> : description
	</dl>

- DOM: Document Object Model:

## 5. Others
### A. HTML5 Local Storage
- Local storage has the same functionality as cookie, which mean it stores information on the browser.
- The biggest difference between Cookie and Local storage is that Local storage allows you to store up to 5MB of relatively large information and Local storage doesn't send info to server like Cookie.
- Both Local storage and Cookie don't affect performance of the site.
- there are 2 types of Local Storage: 	
	+ window.localStorage: storing data indefinitely, data will be stored until the user clear history
	+ window.sessionStorage: storing data for each session, data will be lost when you quit your browser.
- localStorage object: 
	+ Have to check whether the browser supports localStorage or not.
		if (typeof(Storage) !== "undefined") {
	    	//support
		} else {
		    //not support
		}
	+ set data: localStorage.setItem('key', value);
	+ get data: localStorage.getItem('key');
- sessionStorage object
	+ set data: sessionStorage.key = value;
	+ get data: sessionStoreg.key;

