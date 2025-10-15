# Ex.08 Design of Interactive Image Gallery
## Date:13/10/2025

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
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Interactive Image Gallery</title>
</head>
<body>
    <header style="text-align: center; background-color: #222; color: white; padding: 1rem 0;">
        <h1>3D Images</h1>
    </header>

   <br>
   <br>

        <div style="display: inline-block; margin-right: 20px;" onclick="openModal(this)">
            <img src="imageS.jpeg" style="height: 200px;">
        </div>
       
        <div style="display: inline-block; margin-right: 20px;" onclick="openModal(this)">
            <img src="imageA.jpeg" style="height: 200px;">
        
        <div style="display: inline-block; margin-right: 20px;" onclick="openModal(this)">
            <img src="imageC.jpeg" style="height: 200px;">
        </div>
        <div style="display: inline-block; margin-right: 20px;" onclick="openModal(this)">
            <img src="imageD.jpeg" style="height: 200px;">
        </div>
        <div style="display: inline-block; margin-right: 20px;" onclick="openModal(this)">
            <img src="imageE.jpeg" style="height: 200px;">
        </div>
    </div>

    <div id="modal" style="display: none; position: fixed; z-index: 1; left: 0; top: 0; width: 100%; height: 100%; background-color: rgba(0,0,0,0.9);">
        <span style="position: absolute; top: 15px; right: 35px; color: white; font-size: 40px; font-weight: bold; cursor: pointer;" onclick="closeModal()">&times;</span>
        <img id="modalImage" style="display: block; margin: 5% auto; max-width: 80%;">
    </div>

    <script>
        function openModal(element) {
            var modal = document.getElementById("modal");
            var modalImg = document.getElementById("modalImage");
            modal.style.display = "block";
            modalImg.src = element.querySelector("img").src;
        }

        function closeModal() {
            document.getElementById("modal").style.display = "none";
        }
    </script>
</body>
</html>

## OUTPUT:
<img width="1907" height="964" alt="Screenshot 2025-10-15 133957" src="https://github.com/user-attachments/assets/efbff104-7da1-4354-b5f7-d184c7f081ff" />


## RESULT:
The program for designing an interactive image gallery using HTML, CSS and JavaScript is executed successfully.
