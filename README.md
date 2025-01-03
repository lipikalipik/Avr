7.	Design and develop HTML program to display Chess Board.  

<!DOCTYPE html>
<html>
    <head>
        <title>chess </title>
                <style>
            .chess-board { border-spacing: 0; border-collapse: collapse; }
                     td { border: 1px solid; width: 2em; height: 2em; }
           .light { background:white; }
             .dark { background: black; }
        </style>
    </head>
    <body>
        <table class="chess-board">
            
                <tr>
                    <th></th>
                    <th>a</th>
                    <th>b</th>
                    <th>c</th>
                    <th>d</th>
                    <th>e</th>
                    <th>f</th>
                    <th>g</th>
                    <th>h</th>
                </tr>
                <tr>
                    <th>8</th>
                    <td class="light"></td>
                    <td class="dark"></td>
                    <td class="light"></td>
                    <td class="dark"></td>
                    <td class="light"></td>
                    <td class="dark"></td>
                    <td class="light"></td>
                    <td class="dark"></td>
                </tr>
                <tr>
                    <th>7</th>
                    <td class="dark"></td>
                    <td class="light"></td>
                    <td class="dark"></td>
                    <td class="light"></td>
                    <td class="dark"></td>
                    <td class="light"></td>
                    <td class="dark"></td>
                    <td class="light"></td>
                </tr>
                <tr>
                    <th>6</th>
                    <td class="light"></td>
                    <td class="dark"></td>
                    <td class="light"></td>
                    <td class="dark"></td>
                    <td class="light"></td>
                    <td class="dark"></td>
                    <td class="light"></td>
                    <td class="dark"></td>
                </tr>
                <tr>
                    <th>5</th>
                    <td class="dark"></td>
                    <td class="light"></td>
                    <td class="dark"></td>
                    <td class="light"></td>
                    <td class="dark"></td>
                    <td class="light"></td>
                    <td class="dark"></td>
                    <td class="light"></td>
                </tr>
                <tr>
                    <th>4</th>
                    <td class="light"></td>
                    <td class="dark"></td>
                    <td class="light"></td>
                    <td class="dark"></td>
                    <td class="light"></td>
                    <td class="dark"></td>
                    <td class="light"></td>
                    <td class="dark"></td>
                </tr>
                <tr>
                    <th>3</th>
                    <td class="dark"></td>
                    <td class="light"></td>
                    <td class="dark"></td>
                    <td class="light"></td>
                    <td class="dark"></td>
                    <td class="light"></td>
                    <td class="dark"></td>
                    <td class="light"></td>
                </tr>
                <tr>
                    <th>2</th>
                    <td class="light"></td>
                    <td class="dark"></td>
                    <td class="light"></td>
                    <td class="dark"></td>
                    <td class="light"></td>
                    <td class="dark"></td>
                    <td class="light"></td>
                    <td class="dark"></td>
                </tr>
                <tr>
                    <th>1</th>
                    <td class="dark"></td>
                    <td class="light"></td>
                    <td class="dark"></td>
                    <td class="light"></td>
                    <td class="dark"></td>
                    <td class="light"></td>
                    <td class="dark"></td>
                    <td class="light"></td>
                </tr>
            
        </table>
    </body>
</html>

OUTPUT
 

8.	Write a JavaScript function to count the number of vowels in each string. (Demonstrate)
<html>
	<head>
		<title>
			get a number of vowels in a string in JavaScript
		</title>
	</head>
<body>
	<h1>
		vowel in a string
	</h1>
<script>
function getVowels(string) {
	var Vowels = 'aAeEiIoOuU';
	var vowelsCount = 0;
	for(var i = 0; i < string.length ; i++) {
		if (Vowels.indexOf(string[i]) !== -1) {
			vowelsCount += 1;
		}
	}
return vowelsCount;
}
document.write("The Number of vowels in -"+" Computer Science "+ getVowels("Computer Science "));
</script>
</body>
</html>

OUTPUT:
 
9.	Write a JavaScript to design a simple calculator to perform the following operations: sum, product, difference, and quotient. (Exercise)
<html>
	<head>
<title> Simple Calculator </title>
<style>
	input {
	    background-color:darkmagenta; 
	    border: none;
        	    color: white;
                   width: 100%;
	    padding: 15px 32px;
        	    text-align: center;
        	    text-decoration: none;
	    display: inline-block;
                     font-size: 16px;
	}
	
</style>	
</head>
<body>
	<center>
        	      <form name="calculator">
         <table>
            <tr>
               <td colspan="4">
                  <input type="text" name="display">
               </td>
            </tr>
            <tr>
               <td><input type="button" value="1" onclick="calculator.display.value += '1'"></td>
               <td><input type="button"  value="2" onclick="calculator.display.value += '2'"></td>
               <td><input type="button"  value="3" onclick="calculator.display.value += '3'"></td>
               <td><input type="button"  value="+" onclick="calculator.display.value += '+'"></td>
            </tr>
            <tr>
               <td><input type="button" value="4" onclick="calculator.display.value += '4'"></td>
               <td><input type="button" value="5" onclick="calculator.display.value += '5'"></td>
	               <td><input type="button" value="6" onclick="calculator.display.value += '6'"></td>
	               <td><input type="button" value="-" onclick="calculator.display.value += '-'"></td>
	            </tr>
	            <tr>
               <td><input type="button" value="7" onclick="calculator.display.value += '7'"></td>
               <td><input type="button" value="8" onclick="calculator.display.value += '8'"></td>
               <td><input type="button" value="9" onclick="calculator.display.value += '9'"></td>
               <td><input type="button" value="x" onclick="calculator.display.value += '*'"></td>
            </tr>
	            <tr>
	               <td><input type="button" value="c" onclick="calculator.display.value = ''"></td>
	               <td><input type="button" value="0" onclick="calculator.display.value += '0'"></td>
	               <td><input type="button"value="="onclick="calculator.display.value = eval(calculator.display.value)"></td>
	               <td><input type="button" value="/" onclick="calculator.display.value += '/'"></td>
	            </tr>
	         </table>
	      </form>
	</center>
	   </body>
   </html>

OUTPUT
 
10.	Design and develop a program to create a countdown timer with JavaScript. (Exercise)
<!DOCTYPE HTML>
<html>
<head>
<style>
p { text-align: center; font-size: 60px; }
</style>
</head>
<body>
<p id="demo"></p>

<script>
var deadline = new Date("march 7, 2025 10:00:25").getTime();
var x = setInterval(function() {
  var t = deadline - new Date().getTime();
  if (t < 0) {
    clearInterval(x);
    document.getElementById("demo").innerHTML = "EXPIRED";
  } else {
    document.getElementById("demo").innerHTML = Math.floor(t / (1000 * 60 * 60 * 24)) + "d " +
    Math.floor((t % (1000 * 60 * 60 * 24)) / (1000 * 60 * 60)) + "h " +
    Math.floor((t % (1000 * 60 * 60)) / (1000 * 60)) + "m " +
    Math.floor((t % (1000 * 60)) / 1000) + "s ";
  }
}, 1000);
</script>
</body>
</html>
OUTPUT
 

 

