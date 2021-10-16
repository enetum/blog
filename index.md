## Introduction

### What is Bootstrap?

Bootstrap is a popular CSS Framework for developing mobile-first websites. Bootstrap, the world’s hottest front-end open supply toolkit, allows you to quickly style and customize sites. Bootstrap includes Sass variables and mixins, responsive grid system, in depth prebuilt components, and powerful JavaScript plugins.

### Why use Bootstrap?

Not only is Bootstrap easy to use and speeds up the website development process, but it is also FREE! The code is open source and well documented as well. While it may seem daunting at first Bootstrap is easy to use and easy to learn. With Bootstrap you no longer have to write custom media queries for all your custom styles. You simply just need to add the classes you want to your HTML elements. Bootstrap also includes everything you need to style your website from icons to pre-built components and themes!

## Let's Get Started!

Below we will walk through how to install and use Bootstrap and customize to your needs with a simple walk through and using basic examples.

### How to Get Started with Bootstrap?

As mentioned before Bootstrap is a free front-end open source toolkit. To get started with Bootstrap all you need to do is visit the website [Bootstrap](https://getbootstrap.com). Once at the site click the ***"Get Started"*** button (see image below).

![Bootstrap Homepage](/img/bootstrap-homepage.png)

For this tutorial we will be using Bootstrap in our project through <link>'s in the <head> of our HTML files. It is also assumed you have an understanding of HTML5 and how it works. Bootstrap's docs provide a perfect starter template for exactly what we want to do here. Scroll down on the same page the ***"Get Started"*** button took you too (see image below).

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

The Bootstrap [getting started introduction](https://getbootstrap.com/docs/5.1/getting-started/introduction/) article talks about popper, components requiring JavaScript, etc. For now ignore all this as are project will not be using it. The Bootstrap framework allows developers to easily layout their site and fill content with pre-made components. We will focus on building a simple landing page using Bootstrap layout and components. Let's head to [the layout docs](https://getbootstrap.com/docs/5.1/layout/grid/) for the next part. Read through this as it is the base for a lot of Bootstrap and how it works.

Before we dive into Bootstrap layout, go ahead and open your index.html file. No need to host the file on a live server or open it locally (however if you'd like to go ahead); simply open it in your web browser. See the video below for opening your index.html file in your web browser (example video is on mac OS):

![Opening index.html](/img/opening-index-html.mov)

It is pretty bare, but let's fix that! Let's add a navbar to the top of our page. Head over to [Navbar](https://getbootstrap.com/docs/5.1/components/navbar/) under components on the left side. This is another doc explaining how the Bootstrap Navbar component works and its styles/customizations.

![Navigating to navbar](/img/layout-to-navbar.png);

## Additional Resources
