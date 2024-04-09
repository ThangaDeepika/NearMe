# Ex04 Places Around Me
## Date: 

## AIM
To develop a website to display details about the places around my house.

## DESIGN STEPS

### STEP 1
Create a Django admin interface.

### STEP 2
Download your city map from Google.

### STEP 3
Using ```<map>``` tag name the map.

### STEP 4
Create clickable regions in the image using ```<area>``` tag.

### STEP 5
Write HTML programs for all the regions identified.

### STEP 6
Execute the programs and publish them.

## CODE
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <style>
        img{
            margin: 0;
        }
    </style>
</head>
<body>
    <img src="ecr.png" width="230" height="230" usemap="#MAPNEW" onmousemove="coordinate(event)">
    <MAP name ="MAPNEW">
        <area shape="RECT" coords="80,20,133,43" href="https://www.iskconchennai.org/" title="ISKCON Temple">
        <area shape="RECT" coords="80,120,134,144" href="https://www.dakshinachitra.net/" title="Dakshina Chitra Heritage Museum">
        <area shape="RECT" coords="123,53,170,170" href="https://www.top-rated.online/cities/Tiruporur/place/p/7459188/ECR+view+point" title="ECR view point">
        <area shape="RECT" coords="76,206,144,234" href="https://madrascrocodilebank.org/" title="The Madras Crocodile Bank">
        
    </MAP> <br>
    X-coordinate <input type="text" id="X" style="width: 8%; background-color:hsla(180, 100%, 50%, 0.281);"><br> <br>
    Y-coordinate  <input type="text" id="Y" style="width: 8%; background-color:hsla(180, 100%, 50%, 0.281);">

    <script>
        function coordinate(event)
        {
            let x=event.clientX;
            let y=event.clientY;
            document.getElementById("X").value=x;
            document.getElementById("Y").value=y;

        }
    </script>
    
</body>
</html>
```
## OUTPUT
![Screenshot 2024-04-09 180700](https://github.com/ThangaDeepika/NearMe/assets/125663099/73debf02-83e5-4149-998f-2ef11cfc6365)
## RESULT
The program for implementing image maps using HTML is executed successfully.
