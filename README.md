# Ex.08 Design of Interactive Image Gallery
## Date:21.12.2024

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
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Interactive Image Gallery</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: antiquewhite;
            display: flex;
            justify-content: center;
            align-items: center;
            min-height: 100vh;
            margin: 0;
            flex-direction: column;
        }

        .gallery-container {
            text-align: center;
            width: 50%;
        }

        .gallery {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            gap: 10px;
        }

        .gallery-item {
            width: 150px;
            height: 150px;
            transition: transform 0.3s ease; /* Smooth transition */
            cursor: pointer;
        }

        footer {
            text-align: center;
            font-size: 20px;
            margin-top: 85px;
        }
    </style>
</head>
<body>
    <div class="gallery-container">
        <h1>Interactive Image Gallery</h1>
        <div class="gallery">
            <img src="kee1.jpg" alt="Image 1" class="gallery-item" id="keerthy1" onclick="zoomInOut('keerthy1')">
             <img src="kee2.jpg" alt="Image 2" class="gallery-item" id="keerthy2"onclick="zoomInOut('keerthy2')">
            <img src="kee3.jpg" alt="Image 3" class="gallery-item" id="keerthy3" onclick ="zoomInOut('keerthy3')">
            <img src="kee4.jpg" alt="Image 4" class="gallery-item" id="keerthy4" onclick ="zoomInOut('keerthy4')">
            <img src="kee5.jpg" alt="Image 5" class="gallery-item" id="keerthy5" onclick="zoomInOut('keerthy5')">
            <img src="kee6.jpg" alt="Image 6" class="gallery-item" id="keerthy6" onclick="zoomInOut('keerthy6')">
            <img src="kee7.jpg" alt="Image 7" class="gallery-item" id="keerthy7" onclick="zoomInOut('keerthy7')">
            <img src="kee8.jpg" alt="Image 8" class="gallery-item" id="keerthy8" onclick="zoomInOut('keerthy8')">
        </div>
    </div>
    <footer>
        Designed and developed by POOJA 2024
    </footer>

    <script>
        function zoomInOut(imageId) {
            var image = document.getElementById(imageId);

            // If the image is not zoomed in, zoom it in
            if (image.style.transform !== "scale(2)") {
                image.style.transform = "scale(2)"; // Zoom in
            } else {
                image.style.transform = "scale(1)"; // Zoom out
            }
        }
    </script>
</body>
</html>


```
## OUTPUT:
![alt text](<Screenshot (14).png>)
 ![alt text](<Screenshot (15).png>)
## RESULT:
The program for designing an interactive image gallery using HTML, CSS and JavaScript is executed successfully.
