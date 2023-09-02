<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>class button</title>
    <Style>
        /*1st div start*/
        .btn1 .button{
            text-align: center;
            text-decoration: none;
            display: inline-block;
            padding:15px 20px;
            background-color: rgb(109, 228, 79);
            border: none;
            font-size: 30px;
            border-radius: 5px;
            cursor: pointer;
            margin:2px 4px;
            
        }
        /*1st div end*/

        /*2nd div start*/
        .btn2{
            background-color:rgb(231, 185, 129);
            margin: 1px;
            padding:40px 20px;
              
        }
        .btn2 .btncolors{
            margin:10px 5px;
            padding:15px 25px;
            display: inline-block;
            font-size: 30px;
            text-align: center;
            float: left;
            cursor: pointer;
            border:none;
            color:white;
            border-radius: 8px;
        }

        .none{background-color: none; }
        .green{background-color: green;}
        .blue{background-color: blue;}
        .red{background-color: red;}
        .grey{background-color: gray;}
        .black{background-color: black;}
        /*2nd div end*/

        /*3rd div start*/
        .btn3{
            padding: 100px;
            display:inline-block;
            color:black;
            background-color: rgb(211, 192, 168);
            float: left;
        }
        .btn3 .effect{
            background-color: aliceblue;
            font-size: 30px ;
            padding: 15px 30px;
            margin: 3px 6px;
            color:black;
            font-weight: bold;
            display: inline-block;
            cursor: pointer;
            transition-duration: 0.6s;
            border-radius: 6px;

        }
        .green{border:3px solid green;}
        .green:hover{background-color: green; color: beige;}
        .blue{border:3px solid blue;}
        .blue:hover{background-color: blue; color: beige;}
        .yellow{border:3px solid yellow;}
        .yellow:hover{background-color: yellow; color: rgb(7, 7, 0);}
        .black{border:3px solid black;}
        .black:hover{background-color:black; color: beige;}
        .red{border:3px solid red;}
        .red:hover{background-color: red; color: beige;}
        /*3rd div end*/

        /*4th div start*/
        .btn4{ 
            padding:20px;
            background-color:rgb(255, 255, 255);}
        .btn4 .box{
            background-color: #2b28ec; /border: none;
            color: rgb(226, 190, 190);
            padding: 15px 32px;text-align: center;text-decoration: none;display: inline-block;font-size: 25px;
            margin: 1px 20px;
            cursor: pointer;
            border-radius: 8px;
            transition-duration: 0.6s;
        }
        .shadow1{box-shadow: 0 15px 25px 0 rgb(1, 1, 20);}
        .shadow2:hover{
            box-shadow: 0 20px 30px 0 rgb(36, 2, 2), 2px 16px 20px 10px rgb(219, 104, 104) ;
            background-color: rgb(241, 32, 32);
            color: white;
            
        }
        .Disabled{opacity: 0.4;
        }
        /*4th div end*/

        /*5th div start*/ 
        .btn5{
            background-color: rgb(226, 226, 169);}
        .btn5 .container{
            position: relative;
            max-width: 1000px;
            width: 100%;
        }
        img{height: auto; width: 100%;}
        .container .btn{
            position: absolute;
            top: 50%;
            left:25%;
            transform: translate(-50%, -50%);
            background-color: #292886a4;color: rgb(25, 219, 57);
            font-size: 25px;
            padding: 16px 40px;
            border: none;
            cursor: pointer;
            border-radius: 10px;
            transition: 0.6s; 
        }
        .container .btn:hover{
            background-color: rgba(52, 118, 240, 0.548);
            color:#ffffff;
            box-shadow: 0 15px 20px 0 #7775da;    
        }
        /*5th div end*/

        /*6th div start*/

        .btn6{
            background-color: rgb(120, 160, 196);
            padding: 50px;
        }
        .btnhover{
            display: inline-block;
            border-radius: 4px;
            background-color: #f4511e;
            border: none;
            color: #FFFFFF;
            text-align: center;
            font-size: 28px;
            padding: 20px;
            width: 200px;
            transition: all 0.5s;
            cursor: pointer;
            margin: 5px;
            
        }
        .span{
            position: relative;
            transition:0.5s;
        }
        .btnhover:hover span{
            padding-right: 25px;
        }
        /*6th div end*/

        /*7th div start*/

        .btn7{
            background-color: #FFFFFF;
            padding: 20px 25px;
        }
        .btn7 .refill{
            position: relative;
            overflow: hidden;
            width: 300px;
            padding: 25px 20px;
            margin: 4px 2px;
            background-color: #2b28ec;
            color: #FFFFFF;
            text-align: center;
            font-size: 30px;
            border: none;
            border-radius: 8px;
            cursor: pointer;
            transition-duration: 0.5s;
        }

        .refill:after{
            content:'';
            position: absolute;
            opacity: 0;
            background-color: aqua;
            padding: 300px;
            margin:-120px;
            transition:all 0.5s;
            display: block;
        }
        .refill:active:after{
            padding: 0;
            margin: 0;
            opacity: 1;
            transition: 0s;
        }
        /*7th div end*/

    </Style>
</head>
<body>
<!--btn1 start-->
<div class="btn1">
        <h1>1. CSS buttons</h1>
    <button>Default button</button>
    <a href="#" class="button" > link button</a>
    <button class="button"> button1</button>
    <input type="button" value="Input button" class="button">
</div><br><hr>
<!--btn1 end-->

<!--btn2 start-->
<div class="btn2">
    <h1>2. Button Colors varity</h1>
    <p style="font-size: larger;">Border radius red</p><br>
    
    <button class="btncolors none" style="color:black">None</button>
    <button class="btncolors green">Green</button>
    <button class="btncolors blue">Blue</button>
    <button class="btncolors red" style="border-radius: 50%;">Red</button>
    <button class="btncolors grey">Grey</button>
    <button class="btncolors black">Black</button>

</div><br><hr>
<!--btn2 end-->

<!--btn3 start-->
<div class="btn3">
    <h1>3. Botton Hover</h1>
    <p style="font-size: x-large;"> Use the transition-duration property to determine the speed of the "hover" effect:</p><hr>
    <button class="effect green"> Green</button>
    <button class="effect blue"> Blue </button>
    <button class="effect yellow"> yellow </button>
    <button class="effect black"> Black</button>
    <button class="effect red"> Red</button>

</div><br><hr>
<!--btn3 end-->

<!--btn4 start-->
<div class="btn4">
    <h1>4. Box Shadow Buttons and Disable Button</h1>
    <p style="font-size: x-large;"> You can shadow your box</p>
    <button class="box shadow1"> Box shadow 1 </button>
    <button class="box shadow2">Box shadow 2 </button>
    <button class="box Disabled" style="cursor: not-allowed;">Box disable</button>
    <p style="font-size: xx-large;"> Use the opacity property to add some transparency to a button make it look disabled</p>
</div><br><hr>
<!--btn4 end-->

<!--btn5 start-->
<div class="btn5">
    <h1>5. Button on Image</h1>
    <div class="container">
        <img src="/img/astronomy-1867616_1280.jpg" alt="" style="width: 50%;">
        <button class="btn">Touch me</button>
    </div>
</div><br><hr>
<!--btn5 end-->

<!--btn6 start-->
<div class="btn6">
    <h1>6. Animatted hover</h1>
    <button class="btnhover"><span>Hover</span></button>
</div><br><hr>
<!--btn6 end-->

<!--btn7 start-->
<div class="btn7">
    <h1>7. Animatter Refill </h1>
    <button class="refill"> Click me</button>
</div>
<!-- btn7 end-->


</body>
</html>
