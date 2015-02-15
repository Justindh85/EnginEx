![EnginEx.js :The Best Embedded Server-side JavaScript You Will Ever Use!](http://i.imgur.com/agsSZY5.png)
---------------------------
### TABLE OF CONTENTS
 * About Justin D Harlan
 * About EnginEx.js
	 * What is EnginEx.js?
	 * EnginEx.js Features
	 * Introduction to EnginEx.js
	 * Requirements of EnginEx.js
	 * Installation of EnginEx.js
	 * EnginEx.js Basic API
	 * Basic Usage of EnginEx.js in a HTML File
 * A Simple Example of a Website
	 * Configuring The Server
	 * Putting together the HTML Files
 * Conclusion
 * License

### Author: Justin D Harlan

There are many title you can give me, title such as designer, developer, programmer, coder, and even software engineer. Those title are fine and all but the reality is that they are just titles to me, or name with narrow perspective of the passion it take to push forwards beyond preconceive boundaries. In truth like so many others that believe as I do being a programmer may not be enough, but being a problem solver that is something more than just a simple coder. I am a Problem solver and the programming is only one of my tools. In the last decade I have used graphic design, web design, video editing, 3D modeling, After Affects, Photoshop, ActionScript 2.0/3.0, HTML, CSS, JavaScript, PHP, jQuery, MYSQL, WordPress, XML, ffmpeg, video brodcasting, networking, NOSQL, JSON, Node.js and many more things to push the limits and produce a solution. All these thing are tools to get a favorable result. I am passionate about what I do is an understatement because I because I seek to be the best version of me. For the record how do I see myself when I think of what the best version of me is, well that is simple. The best version of me is building and/or fixing what ever I can.

### What is EnginEx.js?
***EnginEx.js*** ( MIT license ) is a high performance template engine framework, written in ECMAScript which is popularly known to most as JavaScript. ***EnginEx.js*** is created and maintained by ***Justin Duane Harlan***

### EnginEx.js Features

- Full support for ECMAScript 5.1 ([ECMA-262](http://www.ecma-international.org/publications/standards/Ecma-262.htm "ECMAScript® Language Specification")) 
- Uses [***Node.js***](http://nodejs.org/ "Node.js") full JavaScript language and it's API inside ***EnginEx.js*** Embedded server-side JavaScript.
- Block Statements inside ***EnginEx.js*** Embedded server-side JavaScript actively  interacts with HTML (very much like PHP).
- The include method not only includes the files, it also allows for ***EnginEx.js*** Embedded server-side JavaScript to interact with the scope that the include method was are called in, from within the included file.
- As I mentioned before, ***EnginEx.js*** allows for the uses [***Node.js***](http://nodejs.org/ "Node.js") full JavaScript language and it's API. So just to be clear yes you can use `process` and `require` along with many other tools that come along with [***Node.js***](http://nodejs.org/ "Node.js").

### Introduction to EnginEx.js
There are so many people that is raving about logic-less templates. Well ***EnginEx.js*** is not about that. I not saying you cant produces logic-less templates with my software, I'm just saying that my software is about embedding sever side JavaScript directly in to the HTML code to give developers a better option and a easier work flow method than writing server-side files and HTML files. With the ability to create actual class documents With the ability to modify the HTML code before the prepossessing stage it will give you the power to produce website with the capabilities more closer to PHP development style than any other view engine before. 

***EnginEx.js*** is a view engine that  mirrors the way PHP's embeds server-side script into HTML code. The main benefits to using ***EnginEx.js*** is the ability to load the run included files from a file. When using the include function to load files you can create template files and [***Node.js***](http://nodejs.org/ "Node.js")  server-side script class files. ***EnginEx.js*** allows for the embedded [***Node.js***](http://nodejs.org/ "Node.js") Script to be modified and the page to be refreshed, without having restarting [***Node.js***](http://nodejs.org/ "Node.js").

The purpose of the development of ***EnginEx.js*** is to increase developers work flow with less complex applications and allowing the learning curve to sharply decrease for my fellow PHP developers. [***Node.js***](http://nodejs.org/ "Node.js") is note difficult to learn but using [***Node.js***](http://nodejs.org/ "Node.js") is more of the equivalent a PHP developer creating and configure the server to handle every module and component of Apache MYSQL without PHP. To cut to the chase [***Node.js***](http://nodejs.org/ "Node.js") And Express is the Apache where MongoDB is the MYSQL and ***EnginEx.js*** is the PHP in WAMP/LAMP configurations. So if you understand how important is PHP to WAMP/LAMP configurations then you can see the importance of ***EnginEx.js***.

If you are familiar with PHP then you will appreciate ***EnginEx.js*** because of one of its for most focus points is to make PHP developers learning curve for [***Node.js***](http://nodejs.org/ "Node.js") less complex, being that I am very fond of PHP and can't help but to miss some of the benefits of its language. So to resolve an the yearning of missing some of the strong benefits of PHP I wrote ***EnginEx.js*** to merge the gaps in [***Node.js***](http://nodejs.org/ "Node.js") development for PHP developers.

**Requirements of EnginEx.js**

[***Node***](http://nodejs.org/ "Node.js") 0.8.0 +

[***Express***](http://expressjs.com/ "Express.js") 4.0.x +

>`> npm install express`

**Installation of EnginEx.js**

You can install ***EnginEx.js*** NPM

NPM download Command
>`> npm install enginex`
**EnginEx.js Basic API**
EnginEx.js has some built-in  functions and objects that you may find very useful

**include( path)  #method**

- Argument:
	- Type: String Literals or String properties of the ``window`` object.
- Description: This method excepts an file path to insert in to the document. The include method makes it is possible to insert the text/code/markup of one file into the current document before the server executes it what makes the include method in EnginEx.js is that it keeps all of the include file's embedded server-side JavaScript in scope same scope just like in PHP making it more flexible to design patterns, and yes you can also make HTML in to embedded server-side JavaScript class files.
- ***! Warning !***: The only two values that this method can except is an Sting literal with no concatenations and the ``window`` object with no concatenations . This object is not editable because if the ``window`` object was edited it can make the include method unstable when using it with the include method.

Example Usages

	// Including CSS files into the document.
	<styles><?njs include('directory/file.css'); ?></styles>

	// Including JavaScript files into the document.
	<script> var a='text'; <?njs include('directory/file.js'); ?></script>

	// Including HTML files into the document.
	<div><?njs include('directory/file.html'); ?></div>

	// Including text files into the document.
	<div><?njs include('directory/file.txt'); ?><div>

	// Including HTML files into the document with the window object.
	// The include method can only accept String Literals or
    // values from the "window" object and can not have any
    // type of concatenation expression
	<div><?njs include(window.some_property); ?></div>

**echo( String )  #method**

- Argument:
	- Type: String.
- Description: This method excepts a text, code, and/or markup to insert in to the html file. The echo method makes it is possible to insert the text/code/markup from a string into the current document before the server executes it.

Example Usage:

	//Inserting CSS code into the document.
	<styles><?njs echo('body{color:black;}'); ?></styles>

	//Inserting JavaScript code into the document.
	<script> var a='text'; <?njs echo('var b=a;'); ?></script>

	//Inserting HTML code into the document.
	<div><?njs echo('<p>Text Goes Here</p>'); ?></div>

	//Inserting text into the document.
	<div><?njs echo('Text Goes Here'); ?><div>
		
**window #object**

- Description: The ``window`` object holds the options value when [***Express.js***](http://expressjs.com/ "Express.js") render method pass options to EnginEx.js.
- ***! Warning !***: The ``window`` object is frozen before the HTML document is complied. This object is not editable, because if the ``window`` object was edited it can make the include method unstable when using it with the include method, So you should repeat after me, ***"I [state your name] would not, could not, and should not attempt to modify the window object on the HTML side of EnginEx.js, and if I could, I doom my application to being possibly unstable and unreliably and I do so at my own risk."***

Example Usage:

	// Example of Express.js render method passing options to EnginEx.js.
	router.get('/',function(req,res){
	var options ={property: 'values'};
		res.render( 'index.html', options);
	});

	// Example of using the options pasted EnginEx.js in the template.
	// Inserting HTML code into the document.
	<div><p><?njs echo(window.property); ?></p></div>
	// results in "<div><p>values</p></div>"

**globals #object**


- Description: The `globals` object get and set properties or methods set by the user in EnginEx.js.

Example Usage:

	// Example using the "globals" object in EnginEx.js htm;.
	globals['property']='value';
	var a = globals.property==='value'; //a=true
	// Example of using the options pasted EnginEx.js in the template.
	globals['method']=function(a){ var b=a+1; return b;}
	var c = globals.method(1)===2; //c=true

###Basic Usage of EnginEx.js in a HTML File
When using EnginEx.js inside the HTML file you can enter and escape the [***Node.js***](http://nodejs.org/ "Node.js") server-side JavaScript by the opening tag `<?njs` and closing tag `?>`. 

	<?njs /*Node.js embedded server-side JavaScript goes in here…*/ ?>
The code above is an basic example of how to use the server-side JavaScript tag in your HTML code you can see that it is very much like PHP's server-side script tags.

	<?php /*embedded server-side script for PHP goes in here…*/ ?>
The reason for this is because I wanted PHP developers to be comfortable with its syntax and also because the developers that will be using ***EnginEx.js*** will have an rare ability to use ***EnginEx.js***'s embedded server-side JavaScript much like a PHP developer would use php.
##A Simple Example of a Website
This Section is an example how to make an simple website with a ***EnginEx.js*** as your view engine. What you will also learn in this section is that ***EnginEx.js*** goes farther beyond the limits of your average view engine to open up a new world of possibilities.
###Configuring The Server
When configuring ***EnginEx.js*** , it is important that you remember that ***EnginEx.js*** was developed to work with the Express module and is also Express-compliant. Below is an outline of the web directory and it's files.

The **folders** are in a **bold** font style and the *files* are in a *italic* font style.
>
- /**root directory (http://localhost:3000)**
	- /**node_modules**
	- /**public**
		- /**css**
			- /*styles.css*
		- /**img**
		- /**js**
			- /*jquery-1.11.1.min.js*
		- /**views**
			- /**partials**
				- /*contents.html*
				- /*footer.html*
				- /*head.html*
				- /*header.html*
			- /**pages**
				- *about.html*
				- *contact.html*
				- *home.html*
				- *services.html*
			- /*index.html*
	- /*server.js*

After you have your directories setup, then you should make sure you install [***Express.js***](http://expressjs.com/ "Express.js") and ***EnginEx.js*** before we begin if you already haven't. If you haven't install them yet, here are the install commands.

	npm install express	
and

	npm install enginex

### server.js
The basic set for the [***Node.js***](http://nodejs.org/ "Node.js") server is very straight forward and it's as simple as adding a plugin, serious it should have to get any easier you are actually going to just set up a server. So lets begin, most of the information you need to know is documented in the file as comments being that I expect the reader to be familiar with [***Node.js***](http://nodejs.org/ "Node.js") and [***Express.js***](http://expressjs.com/ "Express.js"). This example website will literal only need two module to start of with, Which you should already have installed.

    //server.js
	// Require EnginEx.js
	var enginex			= require('enginex');
	// Require Express.js
    var express			= require('express');
    var app				= express();
    var router			= express.Router();
	// Setting the port value in Express.js
    app.set('port', process.env.PORT || 3000);
	// Initiate the server with Express.js
    var server = app.listen(app.get('port'),function(){

		// Assigning the server's host address 
		// to the host varialble.
    	var host = server.address().address;

		// Assigning the server's port number 
		// to the host varialble.
    	var port = server.address().port;

		// Registering the engine in Express.js
		// to EnginEx.js.
    	app.engine('html', enginex.__engine);
    	// !!You may also use!! "app.engine('html', engine.__express);".

		// Setting the default engine extension to use when omitted.
    	app.set('view engine', 'html');

		// Setting the directories for EnginEx.js, where the view files are stored (HTML files).
    	app.set('views',__dirname + '/public/views');

		// Setting the static content for EnginEx.js from the "public" directory
    	router.use(express.static(__dirname + '/public'));

		// Stating in Node.js Shell that the Server is loaded and ready.
    	console.log('Magic happens at http://%s:%s', host, port);
		
		// Below are router object returned from for the "express.Router()" method.
		// all the router render the index.html file first as its entry point
		// in to the website.

		// This router points to the url http://localhost:3000 or http://localhost:3000/
		// which is the home page.
    	router.get('/',function(req,res){

			// The first argument of the res.render method is the path to the index.html file.
			// The second argument of the res.render method is an object that is sent to 
			// EnginEx.js. The second argument can be accessed in the html files in the 
			// "window" object.

			// The second argument's node property is an object with 3 properties, of course
			// course you can set this object to anything even to "{}" or add properties to
			// pass along to the "window" object in your template through EnginEx.js.
			// but once you are coding in your template the "window" object is frozen and
			// you can not modify add or remove from it.
			//    1). title: Is the page title.
			//    2). page: Is the path to the page's content template
			//    3). server: Holds the server information.
    		res.render('index.html',{node:{title:'Home',page:'pages/home.html',server:server}});
    	});

		// This router points to the url http://localhost:3000/home
		// which is also the home page.
    	router.get('/home',function(req,res){
    		res.render('index.html',{node:{title:'Home',page:'pages/home.html',server:server}});
    	});

		// This router points to the url http://localhost:3000/about
    	router.get('/about',function(req,res){
    		res.render('index.html',{node:{title:'About',page:'pages/about.html',server:server}});
    	});

		// This router points to the url http://localhost:3000/services
    	router.get('/services',function(req,res){
    		res.render('index.html',{node:{title:'Contact',page:'pages/services.html',server:server}});
    	});

		// This router points to the url http://localhost:3000/contact
    	router.get('/contact',function(req,res){
    		res.render('index.html',{node:{title:'Contact',page:'pages/contact.html',server:server}});
    	});
		// Calls the router object before loading a page.
    	app.use(router);
    });

###Putting together the HTML Files
This example website is based on a [***RESTfull Architecture***](http://en.wikipedia.org/wiki/Representational_state_transfer "Representational State Transfer") style of web design. The purpose of the example is show the simplicity and the possibilities of using ***EnginEx.js***. While displaying its ease of using ***EnginEx.js*** to develop website PHP developers should see how easy it would be to translate most websites from PHP to Node.js using  ***EnginEx.js***.
**index.html**

Below is the index.html file

	<?njs //index.html ?>
	<?njs 
		// Including the header.html
		// The header.html contains the upper contents
		// of the html file including the head element.
		// The include method can only accept String Literals or
		// values from the "window" object and can not have any
		// type of concatenation expression. *SEE "include" in the
		// EnginEx.js Basic API section of the EnginEx.js Documentation
		// or in the read me file.
		include('partials/header.html'); 
	?>
	<div id="page-content">
		<div id="admin_menu">
			<ul class="menu_items">
			<?njs 
				// Loops have been an major part of the computer revolution
				// and it would abslutely be a shame to stop now. Even when you 
				// exit out of the server-side JavaScript it will still loop the
				// html code along with the server-side JavaScript, but wait
				// there is more! This feature also applies to not only for 
				// loops but with all statements with a block statment.
			?>
			<?njs for(var i=0; i<10;i++){ ?>
				<li><div id="menu_item<?njs echo(i); ?>" options-pageID="" options-page="" class='menu_item'>menu item #<?njs echo(i); ?></div></li>
				<?njs 
					// With EnginEx.js it allows you to use the full ability
					// of Node.js such as the require method. Yes thats right,
					// how amazing is that? You can require methods directly
					// from your html file.
					require('../../public/js/test.js').test(i);
				}; ?>
			</ul>
		</div>
		<?njs 
			// Including the content.html
			// The content.html contains the relative page content
			// of the html file in the body.
		?>
		<div id="admin_page">
			<?njs include('partials/content.html'); ?>
		</div>
	</div>
	<?njs 
		// Including the footer.html
		// The footer.html contains the footer content
		// of the html file at the bottom of the page.
		include('partials/footer.html'); 
	?>

-------------------------------------------------

**header.html**

	<?njs //header.html ?>
	<!DOCTYPE html>
	<!--[if lt IE 7 ]><html class="ie ie6" lang="en"> <![endif]-->
	<!--[if IE 7 ]><html class="ie ie7" lang="en"> <![endif]-->
	<!--[if IE 8 ]><html class="ie ie8" lang="en"> <![endif]-->
	<!--[if (gte IE 9)|!(IE)]><html lang="en"><![endif]-->
	<?njs 
		// Including the head.html
		// The head.html contains the head element an it's contents.
	?>
	<?njs include("partials/head.html"); ?>
	<body>
		<div id="header_bar"></div>	
		<header>
			<div class="common_width">			
				<ul id="header_nav">
					<li><a href="http://localhost:3000/page/home">Home</a></li>
					<li><a href="http://localhost:3000/page/about">About</a></li>
					<li><a href="http://localhost:3000/page/services">Services</a></li>
					<li><a href="http://localhost:3000/page/contact">Contact</a></li>
				</ul>
			</div>
		</header>

-------------------------------------------------

**head.html**

	<?njs //head.html ?>
	<head>
		<meta charset="utf-8">
		<title>Example EnginEx.js Website By Justin Duane Harlan</title>
		<meta name="description" content="Example">
		<meta name="author" content="Justin Duane Harlan">
		<meta http-equiv="content-type" content="text/html; charset=UTF8">
		<meta name="viewport" content="width=device-width, initial-scale=1, maximum-scale=1">
		<link rel="stylesheet" href="http://localhost:3000/css/styles.css">
		<script src="http://localhost:3000/js/jquery-1.11.1.min.js"></script>
	</head>

-------------------------------------------------

**content.html**

	<?njs //content.html ?>
	<div id="admin-content">
		<div id="admin-content-head">
			<h1 class="title"><?njs echo(window.node.title); ?></h1>
		</div>
		<?njs if(true){ ?>
			<div id="admin-content-body">
				<?njs include(window.node.page); ?>
			</div>
		<?njs } ?>
		<hr/>
		<div id="admin-content-foot">			
			<?njs echo(window.node.title); ?>
		</div>
	</div>

-------------------------------------------------

**footer.html**

	<?njs //footer.html ?>
			<footer>
				<div class="common_width">
					<div id="copyright">
						<p>&#169; Copyright, All Rights Reserved.</p>
					</div>
					<ul id="footer_nav">
	    				<li><a href="http://localhost:3000/page/home">Home</a></li>
	    				<li><a href="http://localhost:3000/page/about">About</a></li>
	    				<li><a href="http://localhost:3000/page/services">Services</a></li>
	    				<li><a href="http://localhost:3000/page/contact">Contact</a></li>
					</ul>
				</div>
			</footer>
		</body>
	</html>

-------------------------------------------------

**home.html**

	<?njs //home.html ?>
	<div id="home" class='page home'>
		<p>Home page contents goes here...</p>
	</div>

-------------------------------------------------

**about.html**

	<?njs //about.html ?>
	<div id="about" class='page about'>
		<p>About page contents goes here...</p>
	</div>

-------------------------------------------------

**services.html**

	<?njs //services.html ?>
	<div id="services" class='page services'>
		<p>Services page contents goes here...</p>
	</div>

-------------------------------------------------

**contact.html**

	<div id="contact" class='page contact'>
		<p>Contact page contents goes here...</p>
	</div>

-------------------------------------------------

**styles.css**

	html {
		/* $rembase = 10px */
	    font-size: 62.5%
	}
	body{
		/*
		$fontbase = 16px
		$line-height-base = 26px
		*/
		font-size: 16px; /* fallback */
		font-size: 1.6rem;
		line-height: 1.625; /* $line-height-base ÷ $fontbase */
	}
	h1,
	h2 {
		font-size: 26px; /* fallback */
		font-size: 2.6rem;
		line-height: 1; /* $line-height-base ÷ 26 */
	}
	
	h3,
	h4 {
		font-size: 18px; /* fallback */
		font-size: 1.8rem;
		line-height: 1.444; /* $line-height-base ÷ 18 */
	}
	ul {	
		margin:0;
	}
	html, body{
		margin: 0;
		background-color: #333;
	}
	/*body*/
	/*header*/
	#header_bar {
		height: 5px;
		width: 100%;
		background-color: #808080;
		box-shadow: 0px 118px 256px 64px #ddd;	
		-webkit-box-shadow: 0px 118px 256px 64px #ddd;
		-moz-box-shadow: 0px 118px 256px 64px #ddd;
	}
	header {
		width: 100%;
		height: 50px;
		background-color: #ccc;
	}
	#header_nav {
		float: right;
		font-size: 1em;
		width: auto;
		text-align:center;
		margin-right: 80px;
	}
	#header_nav li {
		float: left;
		list-style: none;
		display:inline-block;
		padding: 0 10px;
		height: 45px;
	}
	#header_nav li a{
		color: #fff;
		line-height: 45px;
		text-decoration: none;
	}
	/*content*/
	#page-content{	
		width: 100%;
		height: 700px;
	}
	#menu{
		float: left;
		clear: none;
		width: 200px;
		height: 100%;
		vertical-align: top;
	}
	#menu ul.menu_items{
		list-style: none;
	}
	#menu ul.menu_items li>div.menu_item{
		color:white;
	}
	/* Admin Page Content area */
	#page{
		clear: none;
		margin-left: 200px;
		width: calc(100% - 200px);
		height: 100%;
		vertical-align: top;
	}
	#content{
		width: 100%;
		vertical-align: top;
	}
	#content-head{
		width: 100%;
	}
	#content-head h1.title{
		display: inline-block;
		width: auto;
	}
	#content-body{
		float: left;
		background-color: #888;
		width: 100%;
	}
	#content-body .template .section-row{
		width: 100%;
		clear: none;
	}
	#content-body .template .section-column{
		display: inline-block;
		clear: none;
	}
	#content-body .template{
		clear: both;
		width: 100%;
	}
	#content-body #home{
		background-color: #fff;
		width: 100%;
	}
	#content-body #header_row{
		background-color: #555;
		margin: 5px;
		width: 100%;
		height: 30px;
	}
	#content-foot{
		clear: both;
		width: 100%;
	}
	/*footer*/
	footer {
		display: inline-block;
		background-color: #ccc;
		width: 100%;
	}
	#copyright{
		color: #4a4a4a;
		font: 15px 'Georgia', serif;
		display: inline-block;
		left: 0;
		margin: 30px 0 0 80px;
		clear: none;
	}
	#footer_nav{
		display: inline-block;
		list-style: none;
		float: right;
		margin: 40px 80px 0 0;
		clear: none;
	}
	#footer_nav li{
		display: inline-block;
	}
	#footer_nav li:after {
		padding: 0 10px;
	    content: "|";
	}
	#footer_nav li:last-child:after {
	    content: "";
	}
	#footer_nav a{
		color: #4a4a4a;
		font: 15px 'Arial',sans-serif;
		text-decoration: none;
	}

-------------------------------------------------

## Conclusion

Well as I hope you can see that here are thousands of possible applications that can be produced by EnginEx.js and EnginEx.js does not just a novelty but a real actual beneficial tool that can that can improve the development of any project that has an user interface.

## License

The MIT License (MIT)

Copyright (c) 2015 Justin Duane Harlan

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in
all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
THE SOFTWARE.
