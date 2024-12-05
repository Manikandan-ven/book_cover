# Ex.06 Book Front Cover Page Design
# Date:
# AIM:
To design a book front cover page using HTML and CSS.

# DESIGN STEPS:
## Step 1:
Create a Django Admin project.

## Step 2:
Create an app in the Django interface.

## Step 3:
Create a folder named 'static' in the app folder.

## Step 4:
Create a new HTML file in the static folder.

## Step 5:
Write the HTML code with relevant CSS properties.

## Step 6:
Choose the appropriate style and color scheme.

## Step 7:
Insert the images in their appropriate places.

## Step 8:
Publish the website in the LocalHost.

# PROGRAM:
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <style>* {
        margin: 0;
        padding: 0;
        box-sizing: border-box;
    }
    
    body {
        font-family: sans-serif;
        line-height: 1;
        color: white;
    }
    
    a {
        text-decoration: none;
    }
    
    li {
        list-style: none;
    }
    
    
    .expert-insight {
        margin: 10px 50px;
    }
    
    
    .custom-hr {
        width: 30%;
        margin: 0;
        border: none;
        border-top: 3px solid rgb(44, 41, 40);
        margin-left: 0;
    }
    
    .heading {
        margin: 10px 50px;
        font-size: 4rem;
    }
    
    .sub-heading {
        margin: 10px 50px;
        font-size: 1.4rem;
        font-weight: 550;
        line-height: 1;
    }
    
    
    .spiral-image {
        width: 600px;
        padding: 0px;
        margin: 0px;
    }
    
    
    .editon-image-div {
        margin: 10px 50px;
        display: flex;
        justify-content: space-between;
        align-items: end;
    }
    
    .third-edition {
        font-size: x-large;
        font-weight: 800;
        color: rgb(248, 70, 0);
    }
    
    .ben-image {
        width: 350px;
        
    }
    
    .custom-full-hr {
        border: 1px solid rgb(248, 70, 0);
    }
    
    .author-div {
        margin: 10px 50px;
    }
    
    .author-div {
        display: flex;
        justify-content: space-between;
        padding: 20px 0;
    }
    
    .ben-frain {
        font-size: 1.6rem;
        font-weight: 600;
    }
    
    .packt {
        font-size: 2rem;
        font-weight: 515;
        text-decoration: underline;
    }
    .one{
        width: 600px;
        height: 800px;
        background-color: rgb(9, 9, 9);
    }
    </style>
</head>

<body>
    <center>
    <div class="one">
    <p class="expert-insight">EXPERT INSIGHT</p>
    <hr class="custom-hr">
    <h1 class="heading">Responsive Web <br> Design with <br> HTML5 and CSS</h1>
    <p class="sub-heading">Develop future-proof responsive websites <br> using the latest HTML5 and CSS3 techniques</p>
    <div class="spiral-image-div">
        <img src="sp3.png"height="40%" width="35%">
    </div>
    <div class="editon-image-div">
        <p class="third-edition">Third Edition</p>
        <img src="pic7.png"height="45%" width="35%">
    </div>
    <hr class="custom-full-hr">
    <div class="author-div">
        <p class="ben-frain">MANIKANDAN V</p>
        <p class="packt">Packt</p>
    </div>
</div>
    </center>
</body>

</html>
```
# OUTPUT:

# RESULT:![Uploading Screenshot 2024-12-05 141003.png…]()

The program for designing book front cover page using HTML and CSS is completed successfully.
