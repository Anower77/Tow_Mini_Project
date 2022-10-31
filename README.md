#### ADDITIONAL & SUBTRACTION & MULTIPLECATION & DIVISION
___
## HTML & JS(Project-01)

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Calculator</title>
    <style>
        input.border{border: none;}
    </style>
</head>
<body>
    <label>1st Number :</label>
    <input type="number", name="fnumber", id="fnumber"/>
    <br><br>
    <label>2nd Number :</label>
    <input type="number", name="lnumber", id="lnumber"/>
    <br><br>
    <button id="add" >Addition</button>
    <button id="sub">subtration</button>
    <!-- <button id="mul">Multiply</button>
    <button id="div">Divide</button> -->
    
    <br><br>
    Addition Result     : <input class="border" type="number" id="addResult1"><br><br>
    Subtaction Result   : <input class="border" type="number" id="addResult2"><br><br>
    <!-- Multipletion Result : <input class="border" type="number" id="addResult3"><br><br>
    Divition Result     : <input class="border" type="number" id="addResult4"> -->
    <!-- javascript -->
    <script>
        // var firstNumber, secondNumber, addition
        // function result(){
        //     firstNumber = parseInt(document.getElementById('fnumber').value)
        //     secondNumber = parseInt(document.getElementById('lnumber').value)
        // }

      const addButton1 = document.getElementById('add') 
      addButton1.addEventListener('click', function(){
        let firstNumber = parseInt(document.getElementById('fnumber').value)
        let secondNumber = parseInt(document.getElementById('lnumber').value)
      
         if(firstNumber && secondNumber){
            //Additon
           let addition = firstNumber + secondNumber
            document.getElementById('addResult1').value = addition  
        }

      })

      const addButton2 = document.getElementById('sub') 
      addButton2.addEventListener('click', function(){
         let firstNumber = parseInt(document.getElementById('fnumber').value)
         let secondNumber = parseInt(document.getElementById('lnumber').value)
      
         if(firstNumber && secondNumber){
            //Subtrction
            let subtrction = firstNumber - secondNumber
            document.getElementById('addResult2').value = subtrction
        }

      })
     
      
    //   const addButton3 = document.getElementById('mul') 
    //   addButton3.addEventListener('click', function(){
    //      let firstNumber = parseInt(document.getElementById('fnumber').value)
    //      let secondNumber = parseInt(document.getElementById('lnumber').value)
      
    //      if(firstNumber && secondNumber){
    //         //Subtrction
    //         let multiply = firstNumber * secondNumber
    //         document.getElementById('addResult3').value = multiply
    //     }

    //   })

      
    //   const addButton4 = document.getElementById('div') 
    //   addButton4.addEventListener('click', function(){
    //     let firstNumber = parseInt(document.getElementById('fnumber').value)
    //     let secondNumber = parseInt(document.getElementById('lnumber').value)
      
    //      if(firstNumber && secondNumber){
    //         //Subtrction
    //        let divition = firstNumber / secondNumber
    //         document.getElementById('addResult4').value = divition
    //     }

    //   })


    //   let addButton = document.getElementById('add')
    //   addButton.addEventListener('click', function(){
    //     document.getElementById('addResult').innerHTML = addition
    //   }) 
    </script>
</body>
</html>
```


<br/>


## HTML & JS(Project-02)

```html
<!doctype html>
<html>
<head></head>
<body>
<p id="input">
Enter First Number: <input id="one">
<br/><br/>
Enter Second Number: <input id="two">
</p>
<p><button onclick="fun()">Add</button></p>
<!-- <p id="res" style="display:none;"> -->

Addition Result = <input id="add"><br/><br/>

<script>
    var numOne, numTwo, res;
    function fun()
    {
      numOne = parseInt(document.getElementById("one").value);
      numTwo = parseInt(document.getElementById("two").value);
      if(numOne && numTwo)
      {
        // temp = document.getElementById("res");
        // temp.style.display = "block";
        res = numOne + numTwo;
        document.getElementById("add").value = res;
        
      }
    }
    </script>
</body>
</html>
```