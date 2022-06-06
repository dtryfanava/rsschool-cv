
# Darya Tryfanava

## Contacts 

- Telegram: @dtryfanava
- Email: tryfanav@gmail.com
- Discord: Darya Tryfanava (dtryfanava)

## About Me

I am a self-taught Junior Frontend Developer who aspires to become a Fullstack Developer in the future.

I know how to prioritize correctly and write valid and readable code. At this stage of my development, my experience is limited to a few small projects involving basic elements of the layout. I am keeping on developing in advanced grids, exploring new libraries that will help optimize web applications.

## Soft Skills

- Effective communication
- Understanding of specific documentation
- Problem-solving
- Making complex ideas easy to understand for everyone
- Project management
- Thinking from the other side of the fence
- Flexibility
- Thinking visually

## Tech Skills

### General:

- HTML5
- CSS / Sass / SCSS
- JavaScript / JQuery
- Bootstrap 5 / Flexbox
- npm
- Git / GitHub
- Wordpress

### Some Concepts:

- Databases

## Code Examples

### HTML

```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Shopping List</title>
    <link rel="stylesheet" type="text/css" href="css/style.css">
    <script src="https://ajax.googleapis.com/ajax/libs/jquery/3.6.0/jquery.min.js"></script>
    <script src="https://kit.fontawesome.com/24182292a7.js" crossorigin="anonymous"></script>
    <link href="https://fonts.googleapis.com/css2?family=Headland+One&display=swap" rel="stylesheet">

</head>
<body>
    <div id="shopping-list">
        <h2>Shopping List<i class="fa-solid fa-circle-plus" id="add"></i></h2>
        <input type="text" placeholder="Add new item">
        <ul>
            <li>Milk <i class="fa-solid fa-xmark"></i></li>
            <li> Bread<i class="fa-solid fa-xmark"></i></li>
            <li>Toffy <i class="fa-solid fa-xmark"></i></li>
            <li>Butter<i class="fa-solid fa-xmark"> </i></li>
        </ul>

    </div>
    <script type="text/javascript" src="js/javascript.js"></script>
</body>
</html>
```
### CSS

```
.done {
    color: #2c4f667d;
    text-decoration: line-through;
}

#shopping-list {
    background: #dbdbdb;
    width: 300px;
    margin: 0 auto;
    box-shadow: 0 4px 8px 0 rgba(0,0,0,0.2);
    transition: 0.3s;

}

#shopping-list:hover {
    box-shadow: 0 8px 16px 0 rgba(0,0,0,0.2);
  }

  body {
      background-image: url('../images/abstract-colorful-dots-pattern-spread-background_38782-219.webp');
      font-family: 'Headland One', serif;

      
  }

  h2{
      background: #61a7aa;
      margin: 0;
      padding: 10px 15px;
      color: rgb(255, 255, 255);
      font-weight: normal;


  }

  ul {
      list-style: none;
      margin: 0px;
      padding: 0px;
  }
  ul li:nth-child(odd) {
    background: #f9f9f9;
  }

  li{
      color: #294e69;
      height: 30px;
      line-height: 30px;
      font-size: 20px;
      padding-left: 20px;
  }

  input{
      width: 100%;
      margin: auto;
      padding: 0px;
      box-sizing:border-box;
      color: #61a7aa;
      font-family: 'Headland One', serif;
      font-size: 20px;
  }

  input:focus {
      border: 2px solid #61a7aa;
      outline: none;
  }

  i {
      float: right;
      color: #ba647a;
      padding-right: 20px;
      align-items: center;
      width: 0;
      }

#add {
      float: right;
      color: #ffffff;
      padding-right: 20px;
      align-items: center;
      width: 0;

}


```

### JavaScript

```
$('ul').on('click', 'li', function() {
    $(this).toggleClass('done');
})


$('ul').on('click', 'i',function() {
    console.log('done');
    event.stopPropagation();
    $(this).parent().fadeOut(function(){
        $(this).remove();
    }
        );
})

$('input').keypress(function(event){
    if(event.which === 13) {

        var itemText = $(this).val();
        $(this).val('');
        $('ul').append('<li> ' + itemText + '</li>');
    }
})

$('h2 i').click(function(){
   $('input').fadeToggle(); 
})

```

### SCSS

```
* {
  margin: 0;
  padding: 0;
}

$color-primary: #f9ed69; //yellow color
$color-secondary: #f0a85d; //orange color
$color-tertiory: #b83b5e; //pink color
$color-text-dark: #333; //grey color
$color-text-light: #fff; //white color

$width-button: 150px;

@mixin clearfix {
  &::after {
  content:"";
  clear: both;
  display: table;
}}

@mixin style-link-text($color) {
  text-decoration: none;
  text-transform: uppercase;
  color: $color;
}

nav {
  margin: 30px;
  background-color: $color-primary;
  @include clearfix;
}


.navigation{
  list-style: none;
  li {
    display: inline-block;
    margin-left: 30px;
    
    &:first-child {
      margin: 0;
    }
    
    a:link {
      @include style-link-text($color-text-dark);
    }
  }
}


.button {
  float: right;
} 


%button-placeholder {
  padding: 10px;
  display: inline-block;
  text-align: center;
  border-radius: 100px;
  width: $width-button;
  @include style-link-text($color-text-light);
}


.btn-main {
  &:link {
    @extend %button-placeholder;
    background-color: $color-secondary;
  }
  
  &:hover {
    background-color: darken($color-secondary, 15%);
  }
}

.btn-hot {
  &:link {
    @extend %button-placeholder;
    background-color: $color-tertiory;
    
  }
  
  &:hover {
    background-color: lighten($color-tertiory, 10%);
  }
}

```

## Experience

Coming soon...

## Education

- RS School (JS/Frontend Development Course)
- Udemy Courses
- FreeCodeCamp / HTMLAcademy / Codecademy
- IT Institute, Belarusian State University of Informatics and Radioelectronics (Web design, Web development)
- Buckinghamshire New University (Project Management)
- FabLab Denmark (Engineering creativity centers and business support hubs)
- Minsk State Linguistic University (German and English foreign languages, Public Relations major)
- Youtube

## Languages

- English(Upper-Intermediate / Advanced)
- German(Upper-Intermediate)

