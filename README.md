# Ex.08 Design of Interactive Image Gallery
# Date: 13.05.2025
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
gallery.html
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Interactive Photo Gallery</title>
    <style>
        
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f4f4f9;
        
        }

        h1 {
            text-align: center;
            margin: 20px 0;
        }

        .gallery-container {
            max-width: 100%;
            margin: 0 auto;
            padding: 20px;
        }


        .gallery {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 15px;
        }

        .gallery-item {
            position: relative;
            overflow: hidden;
            border-radius: 10px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
            cursor: pointer;
        }

        .gallery-item img {
            width:  100%;
            height: auto;
            display: flex;
            transition: transform 0.3s ease;
        }

        .gallery-item:hover img {
            transform: scale(1.05);
        }

       
        .lightbox {
            display: none;
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background-color: white;
            justify-content: center;
            align-items: center;
            z-index: 1000;
        }

        .lightbox img {
            max-width: 100%;
            max-height: 100%;
            border: 5px solid white;
            border-radius: 10px;
        }

        .lightbox:target {
            display: flex;
        }

       
        .close {
            position: absolute;
            top: 20px;
            right: 20px;
            font-size: 30px;
            color: white;
            text-decoration: none;
            font-weight: bold;
        }

        .close:hover {
            color: #ff5050;
        }
        .footer{
            position: fixed;
            background-color: rgb(101, 214, 239);
            text-align: center;
            bottom: 0;
            width:100%;
        }
    </style>
</head>
<body>
    <h1>Interactive Photo Gallery</h1>
    <div class="gallery-container">
        <div class="gallery">
            
            <div class="gallery-item">
                <a href="#img1"><img src="Screenshot 2025-05-13 162058.png" alt="Image 1"></a>
            </div>
            
            <div class="gallery-item">
                <a href="#img2"><img src="Screenshot 2025-05-13 162126.png" alt="Image 2"></a>
            </div>
           
            <div class="gallery-item">
                <a href="#img3"><img src="Screenshot 2025-05-13 162201.png" alt="Image 3"></a>
            </div>

            <div class="gallery-item">
                <a href="#img5"><img src="Screenshot 2025-05-13 162305.png" alt="Image 5"></a>
            </div>
            <div class="gallery-item">
                <a href="#img6"><img src="Screenshot 2025-05-13 162522.png" alt="Image 5"></a>
            </div>
            <div>
            <footer class="footer">Designed by Harine S</footer>
            </div>
            
        </div>
        </div>
    </div>

    
    <div id="img1" class="lightbox">
        <a href="#" class="close">&times;</a>
        <img src="Screenshot 2025-05-13 162058.png" alt="Image 1">
    </div>
    <div id="img2" class="lightbox">
        <a href="#" class="close">&times;</a>
        <img src="Screenshot 2025-05-13 162126.png">
     </div>
     <div id="img3" class="lightbox">
        <a href="#" class="close">&times;</a>
        <img src="Screenshot 2025-05-13 162201.png">
     </div>
     
    </div>
    <div id="img5" class="lightbox">
        <a href="#" class="close">&times;</a>
        <img src="Screenshot 2025-05-13 162305.png"> 
    </div>
    <div id="img6" class="lightbox">
        <a href="#" class="close">&times;</a>
        <img src="Screenshot 2025-05-13 162522.png">
    </div>


 </body>
```
# OUTPUT:

![Screenshot 2025-05-13 165148](https://github.com/user-attachments/assets/44e15cc4-7ea6-47ff-a67e-1f42f41278c5)


![image](https://github.com/user-attachments/assets/40f628bc-91b2-4ed4-90e8-29c03e77c799)


# RESULT:
The program for designing an interactive image gallery using HTML, CSS and JavaScript is executed successfully.
