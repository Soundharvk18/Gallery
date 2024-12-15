# Ex.08 Design of Interactive Image Gallery
# Date:6/12/24
# AIM:
To design a web application for an inteactive image gallery with minimum five images.

# DESIGN STEPS:
## Step 1:
Clone the github repository and create Django admin interface.

## Step 2:
Change settings.py file to allow request from all hosts.

## Step 3:
Use CSS for positioning and styling.

## Step 4:
Write JavaScript program for implementing interactivity.

## Step 5:
Validate the HTML and CSS code.

## Step 6:
Publish the website in the given URL.

# PROGRAM :
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Gallery</title>
    <style>
        #flexbox
        {
            /* border: 5px solid pink; */
            padding: 116px;
            background-image: url("footback.jpeg");
            background-repeat: no-repeat;
            background-size: cover;
        }
        #container1
        {
            /* margin-left:25%; */
            display: flex;
            background-color: whitesmoke; 
            gap: 20px;
            justify-content: center;
            padding: 20px;
            box-shadow: 0 2px 3px;
        }
        #container2
        {
            gap: 20px;
            display: flex;
            background-color: whitesmoke; 
            justify-content: center;
            /* border: 5px inset black; */
            padding: 10px;
            box-shadow:0 2px 3px;
        }
        .img
        {
            height: 190px;
            width: 260px;
            /* transform: rotate(-10deg); */
            image-rendering:optimizeQuality;    
            border: 2px inset whitesmoke;    
            border-radius: 10px;
            box-shadow:  0 0 10px black ;
            transition: 0.5s;
        }
        .img:hover
        {
            content: 'hello';
            transform: scale(1.3);
        }
        #divs
        {
            display: inline;
        }
        #image
        {
            z-index: 100;
            display: none;
            background: rgba(0,0,0,0.5);
            position: fixed;
            width: 100%;
            /* transform: rotate(20deg); */
            height: 100%;
            top: 0;
            bottom: 0;
            align-items: center;
            justify-content: center;    
        }
        #image img{
            width: 600px;
            height: auto;
        }
        #title
        {
            
            border-radius: 10px;
            width: 500px;
            box-shadow: 0 3px 10px;
            position: absolute;
            top: 20px;
            left: 500px;
        }
    </style>
</head>
<body>
    <section id="image">
            <img src="footback.jpeg" alt="" id="display" onclick="closes()">
    </section>
<div id="flexbox">

    <h1 align="center" style="color: azure;" ><span id="title">GREATEST SOCCERS</span></h1>

    <div id="container1">
        <div class="divs"><img class="img" src="messi.jpg" onclick="opens(this.src)" alt=""></div>
        <div class="divs"><img class="img" src="ronaldo.jpg" onclick="opens(this.src)"   alt=""></div>
        <div class="divs"><img class="img" src="neymar.jpg"  onclick="opens(this.src)"  alt=""></div>
        <div class="divs" ><img class="img" src="pele.jpg" onclick="opens(this.src)"   alt=""></div>
    </div>
    <div id="container2">
        <div class="divs" ><img class="img" src="haland.webp" onclick="opens(this.src)"  alt=""></div>
        <div class="divs"><img class="img" src="mbappe.jpg" onclick="opens(this.src)"  alt=""></div>
        <div class="divs" ><img class="img" src="vinicius.webp" onclick="opens(this.src)"  alt=""></div>
       <div class="divs"><img class="img" src="harry.webp" onclick="opens(this.src)"  alt=""> </div>
    </div>
    
</div>
<footer align="center" style="background-color:rgb(242, 238, 238)">
    <p>Designed & Developed by soundharvk18 &copy; </p>
</footer>
    <script>
            var a =document.getElementById("image");
            var b=document.getElementById("display");
            function opens(c)
            {
                a.style.display='flex';
                b.src=c;
            }
            function closes()
            {
                a.style.display='none';
            }
    </script>
</body>
</html>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             
```
# OUTPUT:

![Screenshot 2024-12-15 224640](https://github.com/user-attachments/assets/42d88ecf-fe47-4c6c-9417-e4a7ebc7a9c8)
![Screenshot 2024-12-15 223219](https://github.com/user-attachments/assets/471654c7-554f-40f3-af67-16e0313ed8b3)
![Screenshot 2024-12-15 223205](https://github.com/user-attachments/assets/4a012be0-3b0b-48b9-a8ba-4b4c53200871)
![Screenshot 2024-12-15 222817](https://github.com/user-attachments/assets/67fe7e5b-e3a0-4e12-9310-92a56f7ef613)


# RESULT:
The program for designing an interactive image gallery using HTML, CSS and JavaScript is executed successfully.
