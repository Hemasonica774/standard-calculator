# Design of a Standard Calculator

## AIM:

To design a web application for a standard calculator.

## DESIGN STEPS:

### Step 1:
Clone the github repository and create Django admin interface.

### Step 2:
Change setting.py file to allow request from all hosts.

### Step 3:
Use CSS for creating attractive colors.

### Step 4:
Write Javascript program for implementing five different operations.

### Step 5:
Validate the HTML and CSS code.

### Step 6:

Publish the website in the given URL.

## PROGRAM :
```
<!DOCTYPE html>
<html>
    <head>
        <title> My standard Calculator</title>
        <style type="text/css">
        .calci{
            width:500px;
            height: 400px;
            background-color: green;
            margin-left: auto;
            margin-right: auto;
        }
        #result{
            background-color: grey;
        }
        .button{
            width:40px;
            height: 20px;
            background-color: hotpink;
        }
        </style>
        <script type="text/javascript">
        function calculate(args)
        {
            res = document.getElementById("result");
            expression=res.innerText;
            cmd=args.srcElement.innerText;
            if (cmd=="=")
            {
                expression =""+ eval(expression);
            }else if(cmd=="C"){
                expression=""
            }else{
            expression=expression + cmd
            }
            res.innerText=expression;
            //alert("Clicked"+ cmd);
        }
        </script>
    </head>
    <body>
        <div class="calci">
            <div class="calci_title">
            <h1>Calculator</h1>
            </div>
        <div id="result"></div>
        <div class="button">
            <button onclick="calculate(event);">0</button>
            <button onclick="calculate(event);">1</button>
            <button onclick="calculate(event);">2</button>
            <button onclick="calculate(event);">+</button>
            <button onclick="calculate(event);">=</button>
            <button onclick="calculate(event);">C</button>
        </div>
        </div>
    </body>
</html>
```

## OUTPUT:
![image](https://user-images.githubusercontent.com/118361409/213870581-8ef40c22-2d2d-47ad-a71f-dbddfa35017d.png)


## HTML VALIDATOR:
![image](https://user-images.githubusercontent.com/118361409/213870618-d60cd696-07eb-405d-aa3a-aab837016704.png)


## Result:
The program for designing a simple calculator using Javascript is executed successfully.

