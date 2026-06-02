# Ex.05 Book Front Cover Page Design
## Date:

## AIM:
To design a book front cover page using HTML and CSS.

## DESIGN STEPS:

### Step 1:
Create a Django Admin project.

### Step 2:
Create an app in the Django interface.

### Step 3:
Create a folder named 'static' in the app folder.

### Step 4:
Create a new HTML file in the static folder.

### Step 5:
Write the HTML code with relevant CSS properties.

### Step 6:
Choose the appropriate style and color scheme.

### Step 7:
Insert the images in their appropriate places.

### Step 8:
Publish the website in the LocalHost.

## PROGRAM:
index.html
'''html
{% load static %}
<!DOCTYPE html>
<html>
<head>
    <title>Book Cover Page</title>

    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;600;800&display=swap" rel="stylesheet">

    <style>

        body{
            margin:0;
            height:100vh;
            display:flex;
            justify-content:center;
            align-items:center;
            background:#d9d9d9;
            font-family:'Poppins', sans-serif;
        }

        .cover{
            width:420px;
            height:700px;
            background-image:url("{% static 'images/cover.png' %}");
            background-size:cover;
            background-position:center;
            position:relative;
            color:white;
            border:6px double gold;
            border-radius:10px;
            overflow:hidden;
            box-shadow:0 0 30px rgba(0,0,0,0.6);
        }

        .overlay{
            width:100%;
            height:100%;
            background:linear-gradient(
                rgba(0,0,40,0.7),
                rgba(0,80,120,0.5)
            );
            backdrop-filter:blur(3px);
            padding:20px;
            box-sizing:border-box;
        }

        .top{
            font-size:18px;
            font-weight:bold;
            letter-spacing:2px;
        }

        .line{
            width:120px;
            border:1px solid gold;
            margin-top:8px;
        }

        h1{
            text-align:center;
            margin-top:60px;
            font-size:38px;
            line-height:60px;
            color:#00ffff;
            text-shadow:
                0 0 10px #00ffff,
                0 0 20px #00ffff;
            font-weight:800;
        }

        .subtitle{
            margin-top:40px;
            font-size:15px;
            line-height:28px;
            width:75%;
            color:#f0f0f0;
        }

        .photo{
            position:absolute;
            right:25px;
            bottom:130px;
            width:120px;
            height:150px;
            border:4px solid gold;
            object-fit:cover;
            transform:rotate(-5deg);
            box-shadow:0 0 15px rgba(255,255,255,0.5);
        }

        .badge{
            position:absolute;
            top:20px;
            right:20px;
            background:#ff6600;
            color:white;
            padding:8px 15px;
            border-radius:20px;
            font-size:13px;
            font-weight:bold;
        }

        .side-text{
            position:absolute;
            left:-70px;
            top:330px;
            transform:rotate(-90deg);
            letter-spacing:4px;
            font-size:18px;
            font-weight:bold;
            color:gold;
        }

        .bottom{
            position:absolute;
            bottom:20px;
            left:20px;
            right:20px;
        }

        .release{
            font-size:17px;
            font-weight:bold;
        }

        .bottomline{
            border:1px solid gold;
            margin-top:8px;
            margin-bottom:10px;
        }

        .author{
            float:left;
            font-size:17px;
            font-weight:bold;
        }

        .logo{
            float:right;
            font-size:17px;
            font-weight:bold;
        }

    </style>
</head>

<body>

    <div class="cover">

        <div class="badge">
            2026 Edition
        </div>

        <div class="side-text">
            AI • ML • DATA SCIENCE
        </div>

        <div class="overlay">

            <div class="top">
                SEC INSIGHT
            </div>

            <div class="line"></div>

            <h1>
                THE FUTURE<br>
                OF AI<br>
                & DATA<br>
                SCIENCE
            </h1>

            <div class="subtitle">
                Exploring Artificial Intelligence,
                Machine Learning, Predictive Analytics,
                and next-generation data-driven
                technologies shaping the future.
            </div>

            <img src="https://via.placeholder.com/120x150" class="photo">

            <div class="bottom">

                <div class="release">
                    SPECIAL RELEASE
                </div>

                <div class="bottomline"></div>

                <div class="author">
                    Saranraj R
                </div>

                <div class="logo">
                    SEC
                </div>

            </div>

        </div>

    </div>

</body>
</html>
```


## OUTPUT:
![alt text](<Screenshot 2026-06-02 133247.png>)

## RESULT:
The program for designing book front cover page using HTML and CSS is completed successfully.
