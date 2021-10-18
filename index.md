## Introduction

### What is Bootstrap?

Bootstrap is a popular CSS Framework for developing mobile-first websites. Bootstrap, the world’s hottest front-end open supply toolkit, allows you to quickly style and customize sites. Bootstrap includes Sass variables and mixins, a responsive grid system, in-depth prebuilt components, and powerful JavaScript plugins.

### Why use Bootstrap?

Not only is Bootstrap easy to use and speeds up the website development process, but it is also FREE! The code is open source and well documented as well. While it may seem daunting at first Bootstrap is easy to use and easy to learn. With Bootstrap you no longer have to write custom media queries for all your custom styles. You simply just need to add the classes you want to your HTML elements. Bootstrap also includes everything you need to style your website from icons to pre-built components and themes!

## Let's Get Started!

Below we will walk through how to install and use Bootstrap and customize to your needs with a simple walk-through and using basic examples.

### How to Get Started with Bootstrap?

As mentioned before Bootstrap is a free front-end open-source toolkit. To get started with Bootstrap all you need to do is visit the website [Bootstrap](https://getbootstrap.com). Once at the site click the ***"Get Started"*** button (see image below).

![Bootstrap Homepage](/img/bootstrap-homepage.png)

For this tutorial, we will be using Bootstrap in our project through `<link>`'s in the `<head>` of our HTML files. It is also assumed you have an understanding of HTML5 and how it works. Bootstrap's docs provide a perfect starter template for exactly what we want to do here. Scroll down on the same page the ***"Get Started"*** button took you to (see image below).

![Bootstrap Homepage](/img/starter-template.png)

Create an HTML file in your favorite text editor and save it as *index.html*. Go ahead and copy and paste the starter template code into the *index.html* file. The code should look exactly how it does on the Bootstrap page (see code block below).

```
<!doctype html>
<html lang="en">
 <head>
 <!-- Required meta tags -->
 <meta charset="utf-8">
 <meta name="viewport" content="width=device-width, initial-scale=1">

 <!-- Bootstrap CSS -->
 <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/css/bootstrap.min.css" rel="stylesheet" integrity="sha384-1BmE4kWBq78iYhFldvKuhfTAU6auU8tT94WrHftjDbrCEXSU1oBoqyl2QvZ6jIW3" crossorigin="anonymous">

 <title>Hello, world!</title>
 </head>
 <body>
 <h1>Hello, world!</h1>

 <!-- Optional JavaScript; choose one of the two! -->

 <!-- Option 1: Bootstrap Bundle with Popper -->
 <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/js/bootstrap.bundle.min.js" integrity="sha384-ka7Sk0Gln4gmtz2MlQnikT1wXgYsOg+OMhuP+IlRH9sENBO0LRn5q+8nbTov4+1p" crossorigin="anonymous"></script>

 <!-- Option 2: Separate Popper and Bootstrap JS -->
 <!--
 <script src="https://cdn.jsdelivr.net/npm/@popperjs/core@2.10.2/dist/umd/popper.min.js" integrity="sha384-7+zCNj/IqJ95wo16oMtfsKbZ9ccEh31eOz1HGyDuCQ6wgnyJNSYdrPa03rtR1zdB" crossorigin="anonymous"></script>
 <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/js/bootstrap.min.js" integrity="sha384-QJHtvGhmr9XOIpI6YVutG+2QOK9T+ZnN4kzFN1RtK3zEFEIsxhlmWl5/YESvpZ13" crossorigin="anonymous"></script>
 -->
 </body>
</html>
```

A few of the options the Bootstrap template offers to you are commented out. For this basic project let's go ahead with ***"Option 1: Bootstrap Bundle with Popper"***. Go ahead and delete Option 2. Your *index.html* file should now look like this:

```
<!doctype html>
<html lang="en">
 <head>
 <!-- Required meta tags -->
 <meta charset="utf-8">
 <meta name="viewport" content="width=device-width, initial-scale=1">

 <!-- Bootstrap CSS -->
 <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/css/bootstrap.min.css" rel="stylesheet" integrity="sha384-1BmE4kWBq78iYhFldvKuhfTAU6auU8tT94WrHftjDbrCEXSU1oBoqyl2QvZ6jIW3" crossorigin="anonymous">

 <title>Hello, world!</title>
 </head>
 <body>
 <h1>Hello, world!</h1>

 <!-- Optional JavaScript; choose one of the two! -->

 <!-- Option 1: Bootstrap Bundle with Popper -->
 <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/js/bootstrap.bundle.min.js" integrity="sha384-ka7Sk0Gln4gmtz2MlQnikT1wXgYsOg+OMhuP+IlRH9sENBO0LRn5q+8nbTov4+1p" crossorigin="anonymous"></script>

 </body>
</html>
```

The Bootstrap [getting started introduction](https://getbootstrap.com/docs/5.1/getting-started/introduction/) article talks about popper, components requiring JavaScript, etc. For now, ignore all this as our project will not be using it. The Bootstrap framework allows developers to easily layout their site and fills content with pre-made components. We will focus on building a simple landing page using Bootstrap layout and components. Let's head to [the layout docs](https://getbootstrap.com/docs/5.1/layout/grid/) for the next part. Read through this as it is the base for a lot of Bootstrap and how it works.

Before we dive into Bootstrap layout, go ahead and open your *index.html* file. No need to host the file on a live server or open it locally (however if you'd like to go ahead); simply open it in your web browser. See the video below for opening your *index.html* file in your web browser (example video is on mac OS):

![Opening index.html](/img/opening-index-html.mov)

### Next Steps: Components & Layout

It is pretty bare, but let's fix that! Let's add a navbar to the top of our page. Head over to [Navbar](https://getbootstrap.com/docs/5.1/components/navbar/) under components on the left side. This is another doc explaining how the Bootstrap Navbar component works and its styles/customizations.

![Navigating to navbar](/img/layout-to-navbar.png)

Let's go ahead and use one of the example header/navbar Bootstrap provides (see [Bootstrap Examples](https://getbootstrap.com/docs/5.1/examples/)). To easily copy and paste the example go ahead and click the ***"Download examples"*** button. Each of the Bootstrap examples comes with its CSS stylesheet, so we will also be adding those to our *index.html* file as we go. For the header/navbar we will add the following code to our *index.html* file.

1. First lets link our new stylesheet ([headers.css](/examples/headers.css)).

    1. Now link the stylesheet in the `<head> </head>` tags of the *index.html*
 
    ```
    <link rel="stylesheet" href="headers.css">
    ```

1. Next lets change our title from `<title>Hello world!</title>` to `<title>My Bootstrap Site</title>`

 ```
 <title>My Bootstrap Site</title>
 ```

1. Now let's paste the example header/navbar right under our `<body>` tag. It looks bulky due to the default Bootstrap SVG icons the example contains, but we will leave them in for simplicity's sake.

 ```
 <svg xmlns="http://www.w3.org/2000/svg" style="display: none;">
 <symbol id="bootstrap" viewBox="0 0 118 94">
 <title>Bootstrap</title>
 <path fill-rule="evenodd" clip-rule="evenodd" d="M24.509 0c-6.733 0-11.715 5.893-11.492 12.284.214 6.14-.064 14.092-2.066 20.577C8.943 39.365 5.547 43.485 0 44.014v5.972c5.547.529 8.943 4.649 10.951 11.153 2.002 6.485 2.28 14.437 2.066 20.577C12.794 88.106 17.776 94 24.51 94H93.5c6.733 0 11.714-5.893 11.491-12.284-.214-6.14.064-14.092 2.066-20.577 2.009-6.504 5.396-10.624 10.943-11.153v-5.972c-5.547-.529-8.934-4.649-10.943-11.153-2.002-6.484-2.28-14.437-2.066-20.577C105.214 5.894 100.233 0 93.5 0H24.508zM80 57.863C80 66.663 73.436 72 62.543 72H44a2 2 0 01-2-2V24a2 2 0 012-2h18.437c9.083 0 15.044 4.92 15.044 12.474 0 5.302-4.01 10.049-9.119 10.88v.277C75.317 46.394 80 51.21 80 57.863zM60.521 28.34H49.948v14.934h8.905c6.884 0 10.68-2.772 10.68-7.727 0-4.643-3.264-7.207-9.012-7.207zM49.948 49.2v16.458H60.91c7.167 0 10.964-2.876 10.964-8.281 0-5.406-3.903-8.178-11.425-8.178H49.948z"></path>
 </symbol>
 <symbol id="home" viewBox="0 0 16 16">
 <path d="M8.354 1.146a.5.5 0 0 0-.708 0l-6 6A.5.5 0 0 0 1.5 7.5v7a.5.5 0 0 0 .5.5h4.5a.5.5 0 0 0 .5-.5v-4h2v4a.5.5 0 0 0 .5.5H14a.5.5 0 0 0 .5-.5v-7a.5.5 0 0 0-.146-.354L13 5.793V2.5a.5.5 0 0 0-.5-.5h-1a.5.5 0 0 0-.5.5v1.293L8.354 1.146zM2.5 14V7.707l5.5-5.5 5.5 5.5V14H10v-4a.5.5 0 0 0-.5-.5h-3a.5.5 0 0 0-.5.5v4H2.5z"/>
 </symbol>
 <symbol id="speedometer2" viewBox="0 0 16 16">
 <path d="M8 4a.5.5 0 0 1 .5.5V6a.5.5 0 0 1-1 0V4.5A.5.5 0 0 1 8 4zM3.732 5.732a.5.5 0 0 1 .707 0l.915.914a.5.5 0 1 1-.708.708l-.914-.915a.5.5 0 0 1 0-.707zM2 10a.5.5 0 0 1 .5-.5h1.586a.5.5 0 0 1 0 1H2.5A.5.5 0 0 1 2 10zm9.5 0a.5.5 0 0 1 .5-.5h1.5a.5.5 0 0 1 0 1H12a.5.5 0 0 1-.5-.5zm.754-4.246a.389.389 0 0 0-.527-.02L7.547 9.31a.91.91 0 1 0 1.302 1.258l3.434-4.297a.389.389 0 0 0-.029-.518z"/>
 <path fill-rule="evenodd" d="M0 10a8 8 0 1 1 15.547 2.661c-.442 1.253-1.845 1.602-2.932 1.25C11.309 13.488 9.475 13 8 13c-1.474 0-3.31.488-4.615.911-1.087.352-2.49.003-2.932-1.25A7.988 7.988 0 0 1 0 10zm8-7a7 7 0 0 0-6.603 9.329c.203.575.923.876 1.68.63C4.397 12.533 6.358 12 8 12s3.604.532 4.923.96c.757.245 1.477-.056 1.68-.631A7 7 0 0 0 8 3z"/>
 </symbol>
 <symbol id="table" viewBox="0 0 16 16">
 <path d="M0 2a2 2 0 0 1 2-2h12a2 2 0 0 1 2 2v12a2 2 0 0 1-2 2H2a2 2 0 0 1-2-2V2zm15 2h-4v3h4V4zm0 4h-4v3h4V8zm0 4h-4v3h3a1 1 0 0 0 1-1v-2zm-5 3v-3H6v3h4zm-5 0v-3H1v2a1 1 0 0 0 1 1h3zm-4-4h4V8H1v3zm0-4h4V4H1v3zm5-3v3h4V4H6zm4 4H6v3h4V8z"/>
 </symbol>
 <symbol id="people-circle" viewBox="0 0 16 16">
 <path d="M11 6a3 3 0 1 1-6 0 3 3 0 0 1 6 0z"/>
 <path fill-rule="evenodd" d="M0 8a8 8 0 1 1 16 0A8 8 0 0 1 0 8zm8-7a7 7 0 0 0-5.468 11.37C3.242 11.226 4.805 10 8 10s4.757 1.225 5.468 2.37A7 7 0 0 0 8 1z"/>
 </symbol>
 <symbol id="grid" viewBox="0 0 16 16">
 <path d="M1 2.5A1.5 1.5 0 0 1 2.5 1h3A1.5 1.5 0 0 1 7 2.5v3A1.5 1.5 0 0 1 5.5 7h-3A1.5 1.5 0 0 1 1 5.5v-3zM2.5 2a.5.5 0 0 0-.5.5v3a.5.5 0 0 0 .5.5h3a.5.5 0 0 0 .5-.5v-3a.5.5 0 0 0-.5-.5h-3zm6.5.5A1.5 1.5 0 0 1 10.5 1h3A1.5 1.5 0 0 1 15 2.5v3A1.5 1.5 0 0 1 13.5 7h-3A1.5 1.5 0 0 1 9 5.5v-3zm1.5-.5a.5.5 0 0 0-.5.5v3a.5.5 0 0 0 .5.5h3a.5.5 0 0 0 .5-.5v-3a.5.5 0 0 0-.5-.5h-3zM1 10.5A1.5 1.5 0 0 1 2.5 9h3A1.5 1.5 0 0 1 7 10.5v3A1.5 1.5 0 0 1 5.5 15h-3A1.5 1.5 0 0 1 1 13.5v-3zm1.5-.5a.5.5 0 0 0-.5.5v3a.5.5 0 0 0 .5.5h3a.5.5 0 0 0 .5-.5v-3a.5.5 0 0 0-.5-.5h-3zm6.5.5A1.5 1.5 0 0 1 10.5 9h3a1.5 1.5 0 0 1 1.5 1.5v3a1.5 1.5 0 0 1-1.5 1.5h-3A1.5 1.5 0 0 1 9 13.5v-3zm1.5-.5a.5.5 0 0 0-.5.5v3a.5.5 0 0 0 .5.5h3a.5.5 0 0 0 .5-.5v-3a.5.5 0 0 0-.5-.5h-3z"/>
 </symbol>
 </svg>

 <main>
 <header class="p-3 bg-dark text-white">
 <div class="container">
 <div class="d-flex flex-wrap align-items-center justify-content-center justify-content-lg-start">
 <a href="/" class="d-flex align-items-center mb-2 mb-lg-0 text-white text-decoration-none">
 <svg class="bi me-2" width="40" height="32" role="img" aria-label="Bootstrap"><use xlink:href="#bootstrap"/></svg>
 </a>
 
 <ul class="nav col-12 col-lg-auto me-lg-auto mb-2 justify-content-center mb-md-0">
 <li><a href="#" class="nav-link px-2 text-secondary">Home</a></li>
 <li><a href="#" class="nav-link px-2 text-white">Features</a></li>
 <li><a href="#" class="nav-link px-2 text-white">Pricing</a></li>
 <li><a href="#" class="nav-link px-2 text-white">FAQs</a></li>
 <li><a href="#" class="nav-link px-2 text-white">About</a></li>
 </ul>
 
 <form class="col-12 col-lg-auto mb-3 mb-lg-0 me-lg-3">
 <input type="search" class="form-control form-control-dark" placeholder="Search..." aria-label="Search">
 </form>
 
 <div class="text-end">
 <button type="button" class="btn btn-outline-light me-2">Login</button>
 <button type="button" class="btn btn-warning">Sign-up</button>
 </div>
 </div>
 </div>
 </header>
 </main>
 ```

Your final *index.html* file should look like this:

```
<!doctype html>
<html lang="en">
 <head>
 <!-- Required meta tags -->
 <meta charset="utf-8">
 <meta name="viewport" content="width=device-width, initial-scale=1">

 <!-- Bootstrap CSS -->
 <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/css/bootstrap.min.css" rel="stylesheet" integrity="sha384-1BmE4kWBq78iYhFldvKuhfTAU6auU8tT94WrHftjDbrCEXSU1oBoqyl2QvZ6jIW3" crossorigin="anonymous">
 
 <!-- Stylesheets -->
 <link rel="stylesheet" href="headers.css">

 <title>My Bootstrap Site</title>
 </head>
 <body>
 <svg xmlns="http://www.w3.org/2000/svg" style="display: none;">
 <symbol id="bootstrap" viewBox="0 0 118 94">
 <title>Bootstrap</title>
 <path fill-rule="evenodd" clip-rule="evenodd" d="M24.509 0c-6.733 0-11.715 5.893-11.492 12.284.214 6.14-.064 14.092-2.066 20.577C8.943 39.365 5.547 43.485 0 44.014v5.972c5.547.529 8.943 4.649 10.951 11.153 2.002 6.485 2.28 14.437 2.066 20.577C12.794 88.106 17.776 94 24.51 94H93.5c6.733 0 11.714-5.893 11.491-12.284-.214-6.14.064-14.092 2.066-20.577 2.009-6.504 5.396-10.624 10.943-11.153v-5.972c-5.547-.529-8.934-4.649-10.943-11.153-2.002-6.484-2.28-14.437-2.066-20.577C105.214 5.894 100.233 0 93.5 0H24.508zM80 57.863C80 66.663 73.436 72 62.543 72H44a2 2 0 01-2-2V24a2 2 0 012-2h18.437c9.083 0 15.044 4.92 15.044 12.474 0 5.302-4.01 10.049-9.119 10.88v.277C75.317 46.394 80 51.21 80 57.863zM60.521 28.34H49.948v14.934h8.905c6.884 0 10.68-2.772 10.68-7.727 0-4.643-3.264-7.207-9.012-7.207zM49.948 49.2v16.458H60.91c7.167 0 10.964-2.876 10.964-8.281 0-5.406-3.903-8.178-11.425-8.178H49.948z"></path>
 </symbol>
 <symbol id="home" viewBox="0 0 16 16">
 <path d="M8.354 1.146a.5.5 0 0 0-.708 0l-6 6A.5.5 0 0 0 1.5 7.5v7a.5.5 0 0 0 .5.5h4.5a.5.5 0 0 0 .5-.5v-4h2v4a.5.5 0 0 0 .5.5H14a.5.5 0 0 0 .5-.5v-7a.5.5 0 0 0-.146-.354L13 5.793V2.5a.5.5 0 0 0-.5-.5h-1a.5.5 0 0 0-.5.5v1.293L8.354 1.146zM2.5 14V7.707l5.5-5.5 5.5 5.5V14H10v-4a.5.5 0 0 0-.5-.5h-3a.5.5 0 0 0-.5.5v4H2.5z"/>
 </symbol>
 <symbol id="speedometer2" viewBox="0 0 16 16">
 <path d="M8 4a.5.5 0 0 1 .5.5V6a.5.5 0 0 1-1 0V4.5A.5.5 0 0 1 8 4zM3.732 5.732a.5.5 0 0 1 .707 0l.915.914a.5.5 0 1 1-.708.708l-.914-.915a.5.5 0 0 1 0-.707zM2 10a.5.5 0 0 1 .5-.5h1.586a.5.5 0 0 1 0 1H2.5A.5.5 0 0 1 2 10zm9.5 0a.5.5 0 0 1 .5-.5h1.5a.5.5 0 0 1 0 1H12a.5.5 0 0 1-.5-.5zm.754-4.246a.389.389 0 0 0-.527-.02L7.547 9.31a.91.91 0 1 0 1.302 1.258l3.434-4.297a.389.389 0 0 0-.029-.518z"/>
 <path fill-rule="evenodd" d="M0 10a8 8 0 1 1 15.547 2.661c-.442 1.253-1.845 1.602-2.932 1.25C11.309 13.488 9.475 13 8 13c-1.474 0-3.31.488-4.615.911-1.087.352-2.49.003-2.932-1.25A7.988 7.988 0 0 1 0 10zm8-7a7 7 0 0 0-6.603 9.329c.203.575.923.876 1.68.63C4.397 12.533 6.358 12 8 12s3.604.532 4.923.96c.757.245 1.477-.056 1.68-.631A7 7 0 0 0 8 3z"/>
 </symbol>
 <symbol id="table" viewBox="0 0 16 16">
 <path d="M0 2a2 2 0 0 1 2-2h12a2 2 0 0 1 2 2v12a2 2 0 0 1-2 2H2a2 2 0 0 1-2-2V2zm15 2h-4v3h4V4zm0 4h-4v3h4V8zm0 4h-4v3h3a1 1 0 0 0 1-1v-2zm-5 3v-3H6v3h4zm-5 0v-3H1v2a1 1 0 0 0 1 1h3zm-4-4h4V8H1v3zm0-4h4V4H1v3zm5-3v3h4V4H6zm4 4H6v3h4V8z"/>
 </symbol>
 <symbol id="people-circle" viewBox="0 0 16 16">
 <path d="M11 6a3 3 0 1 1-6 0 3 3 0 0 1 6 0z"/>
 <path fill-rule="evenodd" d="M0 8a8 8 0 1 1 16 0A8 8 0 0 1 0 8zm8-7a7 7 0 0 0-5.468 11.37C3.242 11.226 4.805 10 8 10s4.757 1.225 5.468 2.37A7 7 0 0 0 8 1z"/>
 </symbol>
 <symbol id="grid" viewBox="0 0 16 16">
 <path d="M1 2.5A1.5 1.5 0 0 1 2.5 1h3A1.5 1.5 0 0 1 7 2.5v3A1.5 1.5 0 0 1 5.5 7h-3A1.5 1.5 0 0 1 1 5.5v-3zM2.5 2a.5.5 0 0 0-.5.5v3a.5.5 0 0 0 .5.5h3a.5.5 0 0 0 .5-.5v-3a.5.5 0 0 0-.5-.5h-3zm6.5.5A1.5 1.5 0 0 1 10.5 1h3A1.5 1.5 0 0 1 15 2.5v3A1.5 1.5 0 0 1 13.5 7h-3A1.5 1.5 0 0 1 9 5.5v-3zm1.5-.5a.5.5 0 0 0-.5.5v3a.5.5 0 0 0 .5.5h3a.5.5 0 0 0 .5-.5v-3a.5.5 0 0 0-.5-.5h-3zM1 10.5A1.5 1.5 0 0 1 2.5 9h3A1.5 1.5 0 0 1 7 10.5v3A1.5 1.5 0 0 1 5.5 15h-3A1.5 1.5 0 0 1 1 13.5v-3zm1.5-.5a.5.5 0 0 0-.5.5v3a.5.5 0 0 0 .5.5h3a.5.5 0 0 0 .5-.5v-3a.5.5 0 0 0-.5-.5h-3zm6.5.5A1.5 1.5 0 0 1 10.5 9h3a1.5 1.5 0 0 1 1.5 1.5v3a1.5 1.5 0 0 1-1.5 1.5h-3A1.5 1.5 0 0 1 9 13.5v-3zm1.5-.5a.5.5 0 0 0-.5.5v3a.5.5 0 0 0 .5.5h3a.5.5 0 0 0 .5-.5v-3a.5.5 0 0 0-.5-.5h-3z"/>
 </symbol>
 </svg>

 <main>
 <header class="p-3 bg-dark text-white">
 <div class="container">
 <div class="d-flex flex-wrap align-items-center justify-content-center justify-content-lg-start">
 <a href="/" class="d-flex align-items-center mb-2 mb-lg-0 text-white text-decoration-none">
 <svg class="bi me-2" width="40" height="32" role="img" aria-label="Bootstrap"><use xlink:href="#bootstrap"/></svg>
 </a>
 
 <ul class="nav col-12 col-lg-auto me-lg-auto mb-2 justify-content-center mb-md-0">
 <li><a href="#" class="nav-link px-2 text-secondary">Home</a></li>
 <li><a href="#" class="nav-link px-2 text-white">Features</a></li>
 <li><a href="#" class="nav-link px-2 text-white">Pricing</a></li>
 <li><a href="#" class="nav-link px-2 text-white">FAQs</a></li>
 <li><a href="#" class="nav-link px-2 text-white">About</a></li>
 </ul>
 
 <form class="col-12 col-lg-auto mb-3 mb-lg-0 me-lg-3">
 <input type="search" class="form-control form-control-dark" placeholder="Search..." aria-label="Search">
 </form>
 
 <div class="text-end">
 <button type="button" class="btn btn-outline-light me-2">Login</button>
 <button type="button" class="btn btn-warning">Sign-up</button>
 </div>
 </div>
 </div>
 </header>
 </main>

 <!-- Optional JavaScript; choose one of the two! -->

 <!-- Option 1: Bootstrap Bundle with Popper -->
 <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/js/bootstrap.bundle.min.js" integrity="sha384-ka7Sk0Gln4gmtz2MlQnikT1wXgYsOg+OMhuP+IlRH9sENBO0LRn5q+8nbTov4+1p" crossorigin="anonymous"></script>

 </body>
</html>
```

Congratulations you have your header! Now it's time to add some content and a footer. We'll quickly copy and paste this example content as we did before for the header/navbar. The copy and pasting is not the important part here though, be sure to look through the example and play with the classes in the HTML elements. These classes are predefined by Bootstrap's styling and all do different things. Some are for layout, some are for style, and much more. Don't be afraid to get your hands messy playing around with these and see what they do! See [Bootstrap Customize](https://getbootstrap.com/docs/5.1/customize/overview/) for more information.

Let's add a hero to our page using the following code:

1. Add the stylesheet to your *index.html* file as we did before with the header/navbar

 ```
 <link rel="stylesheet" href="heroes.css">
 ```

1. Now add the hero's HTML under the `</main>` tag but still in between the `<body> </body>` tags of the file. Note: you will need to put the proper path to `<img src="bootstrap-themes.png" class="d-block mx-lg-auto img-fluid" alt="Bootstrap Themes" width="700" height="500" loading="lazy">` in your own file. If you downloaded the Bootstrap examples as suggested earlier you can simply copy the image from the example into your directory. I will also link them here:

 * [Image](/img/bootstrap-docs.png)
 
 * [Headers stylesheet](/examples/headers.css)

 * [Heroes stylesheet](/examples/heroes.css)

 ```
 <div class="container col-xxl-8 px-4 py-5">
 <div class="row flex-lg-row-reverse align-items-center g-5 py-5">
 <div class="col-10 col-sm-8 col-lg-6">
 <img src="bootstrap-themes.png" class="d-block mx-lg-auto img-fluid" alt="Bootstrap Themes" width="700" height="500" loading="lazy">
 </div>
 <div class="col-lg-6">
 <h1 class="display-5 fw-bold lh-1 mb-3">Responsive left-aligned hero with image</h1>
 <p class="lead">Quickly design and customize responsive mobile-first sites with Bootstrap, the world’s most popular front-end open source toolkit, featuring Sass variables and mixins, responsive grid system, extensive prebuilt components, and powerful JavaScript plugins.</p>
 <div class="d-grid gap-2 d-md-flex justify-content-md-start">
 <button type="button" class="btn btn-primary btn-lg px-4 me-md-2">Primary</button>
 <button type="button" class="btn btn-outline-secondary btn-lg px-4">Default</button>
 </div>
 </div>
 </div>
 </div>
 ```

 * This is good however the button is blue! This doesn't match our header's primary button (Sign-up) which is yellow. That's because of the class of the button in the hero `<button type="button" class="btn btn-primary btn-lg px-4 me-md-2">Primary</button>`. The `class="btn-primary"` defaults to Bootstrap's blue primary color. We want to to be yellow so lets change the class from `class="btn-primary"` to `class="btn-warning"`. This will give us the classic Bootstrap yellow!

 ```
 <button type="button" class="btn btn-warning btn-lg px-4 me-md-2">Primary</button>
 ```

 * So far your hero code should look something like this

 ```
 <div class="container col-xxl-8 px-4 py-5">
 <div class="row flex-lg-row-reverse align-items-center g-5 py-5">
 <div class="col-10 col-sm-8 col-lg-6">
 <img src="../img/bootstrap-docs.png" class="d-block mx-lg-auto img-fluid" alt="Bootstrap Themes" width="700" height="500" loading="lazy">
 </div>
 <div class="col-lg-6">
 <h1 class="display-5 fw-bold lh-1 mb-3">Responsive left-aligned hero with image</h1>
 <p class="lead">Quickly design and customize responsive mobile-first sites with Bootstrap, the world’s most popular front-end open source toolkit, featuring Sass variables and mixins, responsive grid system, extensive prebuilt components, and powerful JavaScript plugins.</p>
 <div class="d-grid gap-2 d-md-flex justify-content-md-start">
 <button type="button" class="btn btn-warning btn-lg px-4 me-md-2">Primary</button>
 <button type="button" class="btn btn-outline-secondary btn-lg px-4">Default</button>
 </div>
 </div>
 </div>
 </div>
 ```


 * And your page should look like this

 ![Homepage Header and Hero](/img/header-and-hero.png)

Lastly, let's add a footer to your page using the same method as above.

 1. Add the stylesheet to your *index.html* file as we did before with the header/navbar ([Footer's stylesheet](/examples/headers.css))

 ```
 <link rel="stylesheet" href="footers.css">
 ``` 

 1. First we will need to add in our social media svgs. Go ahead and add these svgs into the `<svg>` tag at the top of our file under the last `</symbol>` tag.

 ```
 <symbol id="facebook" viewBox="0 0 16 16">
 <path d="M16 8.049c0-4.446-3.582-8.05-8-8.05C3.58 0-.002 3.603-.002 8.05c0 4.017 2.926 7.347 6.75 7.951v-5.625h-2.03V8.05H6.75V6.275c0-2.017 1.195-3.131 3.022-3.131.876 0 1.791.157 1.791.157v1.98h-1.009c-.993 0-1.303.621-1.303 1.258v1.51h2.218l-.354 2.326H9.25V16c3.824-.604 6.75-3.934 6.75-7.951z"/>
 </symbol>
 <symbol id="instagram" viewBox="0 0 16 16">
 <path d="M8 0C5.829 0 5.556.01 4.703.048 3.85.088 3.269.222 2.76.42a3.917 3.917 0 0 0-1.417.923A3.927 3.927 0 0 0 .42 2.76C.222 3.268.087 3.85.048 4.7.01 5.555 0 5.827 0 8.001c0 2.172.01 2.444.048 3.297.04.852.174 1.433.372 1.942.205.526.478.972.923 1.417.444.445.89.719 1.416.923.51.198 1.09.333 1.942.372C5.555 15.99 5.827 16 8 16s2.444-.01 3.298-.048c.851-.04 1.434-.174 1.943-.372a3.916 3.916 0 0 0 1.416-.923c.445-.445.718-.891.923-1.417.197-.509.332-1.09.372-1.942C15.99 10.445 16 10.173 16 8s-.01-2.445-.048-3.299c-.04-.851-.175-1.433-.372-1.941a3.926 3.926 0 0 0-.923-1.417A3.911 3.911 0 0 0 13.24.42c-.51-.198-1.092-.333-1.943-.372C10.443.01 10.172 0 7.998 0h.003zm-.717 1.442h.718c2.136 0 2.389.007 3.232.046.78.035 1.204.166 1.486.275.373.145.64.319.92.599.28.28.453.546.598.92.11.281.24.705.275 1.485.039.843.047 1.096.047 3.231s-.008 2.389-.047 3.232c-.035.78-.166 1.203-.275 1.485a2.47 2.47 0 0 1-.599.919c-.28.28-.546.453-.92.598-.28.11-.704.24-1.485.276-.843.038-1.096.047-3.232.047s-2.39-.009-3.233-.047c-.78-.036-1.203-.166-1.485-.276a2.478 2.478 0 0 1-.92-.598 2.48 2.48 0 0 1-.6-.92c-.109-.281-.24-.705-.275-1.485-.038-.843-.046-1.096-.046-3.233 0-2.136.008-2.388.046-3.231.036-.78.166-1.204.276-1.486.145-.373.319-.64.599-.92.28-.28.546-.453.92-.598.282-.11.705-.24 1.485-.276.738-.034 1.024-.044 2.515-.045v.002zm4.988 1.328a.96.96 0 1 0 0 1.92.96.96 0 0 0 0-1.92zm-4.27 1.122a4.109 4.109 0 1 0 0 8.217 4.109 4.109 0 0 0 0-8.217zm0 1.441a2.667 2.667 0 1 1 0 5.334 2.667 2.667 0 0 1 0-5.334z"/>
 </symbol>
 <symbol id="twitter" viewBox="0 0 16 16">
 <path d="M5.026 15c6.038 0 9.341-5.003 9.341-9.334 0-.14 0-.282-.006-.422A6.685 6.685 0 0 0 16 3.542a6.658 6.658 0 0 1-1.889.518 3.301 3.301 0 0 0 1.447-1.817 6.533 6.533 0 0 1-2.087.793A3.286 3.286 0 0 0 7.875 6.03a9.325 9.325 0 0 1-6.767-3.429 3.289 3.289 0 0 0 1.018 4.382A3.323 3.323 0 0 1 .64 6.575v.045a3.288 3.288 0 0 0 2.632 3.218 3.203 3.203 0 0 1-.865.115 3.23 3.23 0 0 1-.614-.057 3.283 3.283 0 0 0 3.067 2.277A6.588 6.588 0 0 1 .78 13.58a6.32 6.32 0 0 1-.78-.045A9.344 9.344 0 0 0 5.026 15z"/>
 </symbol>
 ```
 
 
 1. Now add the footer HTML under the last `<div>` of the hero HTML. Notice how some of the classes are changed from the default Bootstrap footer example! The outside `<div>` has `class="container-fluid"` on it in order to make it full width while footer has the `class="container"` on it to contain the elements inside the viewport. This looks nice as it matches our menu. The Bootstrap logo is also changed to white using the text-light class and the social media icons are changed to yellow using the text-warning class as we demonstrated before with the Primary button in the Hero.

 ```
 <div class="container-fluid bg-dark">
 <footer class="container d-flex flex-wrap bg-dark justify-content-between align-items-center py-3 my-4">
 <div class="col-md-4 d-flex align-items-center">
 <a href="/" class="mb-3 me-2 mb-md-0 text-light text-decoration-none lh-1">
 <svg class="bi" width="30" height="24"><use xlink:href="#bootstrap"/></svg>
 </a>
 <span class="text-muted">&copy; 2021 Company, Inc</span>
 </div>
 
 <ul class="nav col-md-4 justify-content-end list-unstyled d-flex">
 <li class="ms-3"><a class="text-warning" href="#"><svg class="bi" width="24" height="24"><use xlink:href="#twitter"/></svg></a></li>
 <li class="ms-3"><a class="text-warning" href="#"><svg class="bi" width="24" height="24"><use xlink:href="#instagram"/></svg></a></li>
 <li class="ms-3"><a class="text-warning" href="#"><svg class="bi" width="24" height="24"><use xlink:href="#facebook"/></svg></a></li>
 </ul>
 </footer>
 </div>
 ```

Now you have a basic landing page built from Bootstrap components and styled with Bootstrap classes! 

![Final Product](/img/final-product.png)

This is a very basic example and uses a lot of copy and pasting. Be sure to try building your components and web pages using Bootstrap practice! It is challenging at first, but you can pick it up easily. For more information and additional resources view the section below.

## Additional Resources

* [Tutorial Video](https://www.youtube.com/watch?v=1nxSE0R27Gg)

* [Getting Started W3](https://www.w3schools.com/bootstrap/bootstrap_get_started.asp)

* [What is Bootstrap](https://www.hostinger.com/tutorials/what-is-bootstrap/)

* [Background of Bootstrap](https://en.wikipedia.org/wiki/Bootstrap_(front-end_framework))

* [index.html file](https://github.com/enetum/blog/blob/main/examples/index.html)