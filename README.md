# Ex.08 Design of Interactive Image Gallery
## Date:16.10.2025

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
```javascript

function openImage(imgElement) {
  const popup = document.getElementById("popup");
  const popupImage = document.getElementById("popupImage");
  
  popupImage.src = imgElement.src;
  popup.style.display = "flex";
}

function closeImage() {
  document.getElementById("popup").style.display = "none";
}

css

body {
  font-family: 'Poppins', sans-serif;
  background: linear-gradient(135deg, #ffe6f0, #e6f7ff);
  text-align: center;
  padding: 20px;
}

h1 {
  color: #333;
  margin-bottom: 30px;
}

.gallery {
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
  gap: 15px;
}

.gallery img {
  width: 500px;
  height: 500px;
  border-radius: 12px;
  box-shadow: 0 4px 10px rgba(0, 0, 0, 0.2);
  transition: transform 0.3s, box-shadow 0.3s;
  cursor: pointer;
}

.gallery img:hover {
  transform: scale(1.1);
  box-shadow: 0 6px 20px rgba(0, 0, 0, 0.3);
}

/* Popup image styling */
.popup {
  display: none;
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background-color: rgba(0, 0, 0, 0.8);
  justify-content: center;
  align-items: center;
}

.popup img {
  max-width: 200%;
  max-height: 200%;
  border-radius: 10px;
  box-shadow: 0 0 20px #fff;
}

html

<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Interactive Image Gallery</title>
  <link rel="stylesheet" href="gallary.css">
</head>
<body>
  <h1> My Interactive Gallery </h1>

  <div class="gallery">
    <img src="cannon.png" alt="Nature 1" onclick="openImage(this)">
    <img src="head.png" alt="Nature 2" onclick="openImage(this)">
    <img src="xlr8.png" alt="Nature 3" onclick="openImage(this)">
    <img src="upgrade.png" alt="Nature 4" onclick="openImage(this)">
    <img src="stone.png" alt="Nature 5" onclick="openImage(this)">
  </div>

  <!-- Popup Image View -->
  <div id="popup" class="popup" onclick="closeImage()">
    <img id="popupImage" src="">
  </div>

  <script src="galley.js"></script>
</body>
</html>
```
## OUTPUT:
![Screenshot_16-10-2025_104744_github com](https://github.com/user-attachments/assets/9da275ef-079f-41e0-b023-2be317fc9292)
![Screenshot_16-10-2025_10480_github com](https://github.com/user-attachments/assets/4bb55b07-5e70-49ad-a6bd-f7186344f2ff)
![Screenshot_16-10-2025_104816_github com](https://github.com/user-attachments/assets/3f8ab567-73af-4fbf-b717-d6a1fb54fe04)

## RESULT:
The program for designing an interactive image gallery using HTML, CSS and JavaScript is executed successfully.
