# navbar-tutorial
How to create navigational bar in your Webpage


<img alt="example" src="https://www.elegantthemes.com/blog/wp-content/uploads/2017/02/hover-effect-one.gif">

A **Navigation Bar** helps the visitors in accessing information easily.
It is the UI element on a webpage that include links for the other section of website.

 In most cases, the navigation bar is part of the main website template, which means it is displayed on most, if not all, of the pages within the website.
 
 With CSS, boring HTML menus can be transformed into good-looking navigation bars. I will explain how to build a basic navigation bar using CSS.
 
 ## How to create a horizontal nav-bar
 
 - First we will create a header tag. Then we will create a div tag with a class name logo and add h1 tag and then we close our div tag.
 
 #### EXAMPLE
 
 ```HTML
 <div class="logo"><h1>Dilnaz Kaur</h1></div>
 ```
 
 - Then, we will add our **search-bar** in another div with class **search-box** and add form tag in it and inside form tag we will use input tag to create interactive
 controls for forms in order to accept data from the user.
 
  #### EXAMPLE
  
 ```HTML
  <div class="search-box">
            <form action="">
             <input type="text" name="search" id="srch" placeholder="
             Search">
             <button type="submmit"><i class="fa fa-search"></i></button>
            </form>
  </div>
  ```
  
  - Then create an unordered list with links.
  
   #### EXAMPLE
   
  ```HTML
            <ul>
            <li><a href="#home">Home</a></li>
            <li><a href="about.html">About</a></li>
            <li><a href="contac.html">Contact</a></li>
            <li><a href="#Services">Services</a></li>
            <li><a href="#facebook"><i class="fab fa-facebook-f"></i></a></li>
            <li><a href="#twitter"><i class="fab fa-twitter"></i></a></li>
            <li><a href="#instagram"><i class="fab fa-instagram"></i></a></li>
          </ul>
```
It's done for HTML.

## Now we are going to design our navigational bar

Create a seprate file for CSS. I had created two different files: one for style and other for reset to organise my code properly.

- First we have to reset the webpage. Also you can provide google font link here!

 #### EXAMPLE
 
```CSS
@import url('https://fonts.googleapis.com/css2?family=Poppins:200,300,400,500,600,700,800,900&display=swap');

*{
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: 'Poppins',sans-serif;
    list-style-type: none;
}

body{
    background-color: rgb(246, 234, 244);
}
```

- Then, we will set height and width for our navbar and some other elements.

#### EXAMPLE

```CSS
header{
    width: 100%;
    height: 15vh;
    bottom: 30px;
    margin-top: 20px;
    display: flex;
    justify-content: space-between;
    align-items: center;
    position: relative;
    z-index: 99;
    box-shadow: 0 0 10px #000;
    background: rgba(211, 183, 214, 0.885);
}
```
- Now, we will organise our social icons and logo 

#### EXAMPLE

```CSS
i{
  color: #fff;
  cursor: pointer;
}

header .logo{
  flex: 1;
  color: rgb(26, 25, 25);
  margin-left: 50px;
  text-transform: uppercase;
}
```

- Here, we will set our search-box. 

#### EXAMPLE 

```CSS
header .search-box{
  flex: 1;
  position: relative;
}

.search-box input{
  width: 100%;
  height: 40px;
  border: none;
  outline: none;
  background-color: #f2f2ff;
  border-radius: 30px;
  color: rgb(246, 240, 240);
  font-size: 16px;
  text-align: center;
  padding-left: 5px;
  padding-right: 40px;
}

.search-box button{
  cursor: pointer;
  width: 40px;
  height: 40px;
  border-radius: 30px;
  border: none;
  position: absolute;
  top: 0;
  right: 0;
  transform: scale(0.9);
  background-color: green;
}
```

- Now, we will set our list horizontaliy and add **space-evenly** and add **hover** effect to the list.

#### EXAMPLE 

```CSS
header ul{
  flex: 2;
  display: flex;
  justify-content: space-evenly;
}

header ul li a {
  text-decoration: none;
  color: #fff;
  font-weight: 600;
  text-transform: uppercase;
  padding: 10px 15px;
}

header ul li a:hover{
  border-bottom: 2px solid cadetblue;
}
```

##### Now, our final navbar is ready to display.
