# Ex.08 Design of a Standard Calculator
## Date:22/04/2024

## AIM:
To design a web application for a standard calculator with minimum five operations.

## DESIGN STEPS:

### Step 1:
Clone the github repository and create Django admin interface.

### Step 2:
Change settings.py file to allow request from all hosts.

### Step 3:
Use CSS for creating attractive colors.

### Step 4:
Write JavaScript program for implementing five different operations.

### Step 5:
Validate the HTML and CSS code.

### Step 6:
Publish the a website in the given URL.

## PROGRAM :
```
calc.html 

<!DOCTYPE html>
<html lang="en">
    <head>
        <title>Calculator</title>
        
        <script>
        function calculate(args)
        {
            res = document.getElementById("result");
            expression = res.innerText;
            cmd = args.srcElement.innerText;
            if(cmd == "=")
            {
                expression = "" + eval(expression)
            }
            else if(cmd == "C")
            {
                expression=""
            }
            else if(cmd == "DEL")
            {
                expression = expression.slice(0, -1);

            }
            else if(cmd == "√")
            {
                expression = "" + Math.sqrt(eval(expression));
            }
            else if(cmd == "%")
            {
                expression = expression % 1;
            }
            else if(cmd == "log")
             {
        expression = Math.log10(expression);
           }
       
            else{
                expression = expression + cmd;
            }
            res.innerText = expression;
            

        }
         
        </script>

        <style>
          
            .calculator-container {
                width: 400px;
                background-color:rgb(187, 69, 14);
                margin: 0 auto; 
                margin-top: 100px;
                text-align: center;
                
            }

           
            button {
                width: 50px;
                height: 50px;
                margin: 10px; 
                font-size: 25px; 
                
                background-color: blue; 
                color: black (255, 255, 255); 
                border: none;
            }

          
            #result {
                
       background-color:rgb(211, 218, 8);
    text-align: right;
    padding-right: 50px;
    font-size: 25px;
    margin-bottom: 20px; 
    border: solid black 0.5px;
    color: black;
    width: 348px;
    height: 50px;
    display: flex;
    align-items: center;
    justify-content: flex-end;

            }
            h1 {
                padding-top: 10px;
                color:rgb(7, 7, 7);
                font-size: 50px;
            }
            .redd {
                background-color:black(244, 240, 240);
                color: rgb(12, 11, 11)
            }
            .bluee {
                
                background-color:rgb(20, 183, 79);
                color: rgb(49, 25, 165) (218, 188, 188);
                font-size: 17px;
            }
            body {
                background-color: palevioletred
            }
        </style>

    </head>
<body bgcolor="skyblue">
    <h1 align="center">PAVITHRA S</h1>
    <h2 align="center">212223220073</h2>
    <div class="calculator-container">
        
        <div id="result">0</div>
        <button onclick="calculate(event);">7</button>
        <button onclick="calculate(event);">8</button>
        <button onclick="calculate(event);">9</button>
        <button class="bluee"  onclick="calculate(event);">/</button>
        <button class="bluee"  onclick="calculate(event);"> DEL </button><br>
        <button onclick="calculate(event);">4</button>
        <button onclick="calculate(event);">5</button>
        <button onclick="calculate(event);">6</button>
        <button class="bluee"  onclick="calculate(event);">*</button>
        <button class="bluee"  onclick="calculate(event);">&radic; </button><br>
        <button onclick="calculate(event);">1</button>
        <button onclick="calculate(event);">2</button>
        <button onclick="calculate(event);">3</button>
        <button class="bluee"  onclick="calculate(event);">-</button>
        <button class="bluee"  onclick="calculate(event);">log</button><br>
        <button onclick="calculate(event);">0</button>
        <button onclick="calculate(event);">.</button>
        <button class="redd" onclick="calculate(event);">C</button>
        <button class="bluee"  onclick="calculate(event);">+</button>
        <button class="bluee" onclick="calculate(event);">=</button><br>
    </div>
    </body>
</html>
```
## OUTPUT:
![Screenshot 2024-04-26 212733](https://github.com/Pavithrasaravanakumar/Calc/assets/150664013/5c03a670-7ec3-4801-889c-5f07f10592bf)
![Screenshot 2024-04-26 212746](https://github.com/Pavithrasaravanakumar/Calc/assets/150664013/2b3836fd-f54d-469d-b051-d05beab08db5)



## RESULT:
The program for designing a standard calculator using HTML and CSS is executed successfully.
