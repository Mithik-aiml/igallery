# Ex.08 Design of Interactive Image Gallery
## Date:17-05-2025
## Name:G.Mithik jain
## Ref No:212224240087

## AIM:
To design a web application for an inteactive image gallery with minimum five images.

## DESIGN STEPS:

### Step 1:
Clone the github repository and create Django admin interface.

### Step 2:
Change settings.py file to allow request from all hosts.

### Step 3:
Use CSS for positioning and styling.

### Step 4:
Write JavaScript program for implementing interactivity.

### Step 5:
Validate the HTML and CSS code.

### Step 6:
Publish the website in the given URL.

## PROGRAM :

```
<!DOCTYPE html>
<html lang="en">
<head>
   <meta charset="UTF-8" />
   <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
   <title>Interactive Image Gallery</title>
   <style>
       body {
           font-family: Arial, sans-serif;
           text-align: center;
           margin: 20px;
           background-color: #412c5d;
       }

       .gallery {
           display: flex;
           flex-wrap: wrap;
           justify-content: center;
           gap: 15px;
       }

       .gallery img {
           width: 150px;
           height: auto;
           border-radius: 8px;
           cursor: pointer;
           transition: transform 0.3s ease;
      }

      .gallery img:hover {
           transform: scale(1.05);
      }

      .lightbox {
           display: none;
           position: fixed;
           z-index: 999;
           top: 0; left: 0;
           width: 100%; height: 100%;
           background: rgba(203, 188, 188, 0.8);
           justify-content: center;
           align-items: center;
      }

      .lightbox-img {
           max-width: 80%;
           max-height: 80%;
      }
  
      .close {
           position: absolute;
           top: 30px;
           right: 50px;
           font-size: 40px;
           color: white;
           cursor: pointer;
      }
   </style>
</head>
<body>
    h1>Interactive Image Gallery</h1>
    <div class="gallery">
       <img src="image1.jpg" alt="Image 1" />
       <img src="image2.jpg" alt="Image 2" />
       <img src="image3.jpg" alt="Image 3" />
       <img src="image4.jpg" alt="Image 4" />
       <img src="image5.jpg" alt="Image 5" />
    </div>

    <div id="lightbox" class="lightbox">
       <span class="close">&times;</span>
       <img class="lightbox-img" id="lightbox-img" src="" alt="Expanded" />
    </div>

    <scripts>
        const galleryImages = document.querySelectorAll('.gallery img');
        const lightbox = document.getElementById('lightbox');
        const lightboxImg = document.getElementById('lightbox-img');
        const closeBtn = document.querySelector('.close');

        galleryImages.forEach(img => {
           img.addEventListener('click', () => {
               lightbox.style.display = 'flex';
               lightboxImg.src = img.src;
           });
        });
    </scripts> 
</body>
</html>

```  

## OUTPUT:

![Screenshot 2025-05-17 122501](https://github.com/user-attachments/assets/f8a8bfa7-e3bf-41d3-956b-9395b3f74497)

## RESULT:
The program for designing an interactive image gallery using HTML, CSS and JavaScript is executed successfully.
