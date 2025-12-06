
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>Python Basics</title>
  <style>
    :root{
      --bg:#f6fbff;
      --card:#ffffff;
      --accent:#0b63d9;
      --text:#0f1723;
      --muted:#556074;
      --radius:12px;
      --shadow: 0 6px 18px rgba(12, 40, 80, 0.08);
      font-family: Inter, system-ui, -apple-system, "Segoe UI", Roboto, "Helvetica Neue", Arial;
    }
    body{
      margin:0;
      min-height:100vh;
      display:flex;
      align-items:center;
      justify-content:center;
      background:linear-gradient(180deg,var(--bg),#eef6ff);
      color:var(--text);
      padding:32px;
    }
    .card{
      max-width:720px;
      background:var(--card);
      border-radius:var(--radius);
      box-shadow:var(--shadow);
      padding:28px;
      border:1px solid rgba(11,99,217,0.06);
    }
    .kicker{
      display:inline-block;
      background:rgba(11,99,217,0.08);
      color:var(--accent);
      font-weight:600;
      padding:6px 10px;
      border-radius:8px;
      font-size:13px;
      margin-bottom:12px;
    }
    h1{
      margin:4px 0 12px;
      font-size:20px;
      letter-spacing:-0.2px;
    }
    p{
      margin:0;
      line-height:1.65;
      color:var(--muted);
      font-size:15px;
    }
    @media (prefers-color-scheme: dark) {
      :root{
        --bg:#071025;
        --card:#071428;
        --accent:#58a6ff;
        --text:#e6eef8;
        --muted:#a9bbd6;
        --shadow: 0 8px 24px rgba(2,6,23,0.6);
      }
    }
  </style>
</head>
<body>
  <article class="card" role="article" aria-labelledby="title">
    <div class="kicker">Programming</div>
    <h1 id="title">Python basics</h1>
    <p>
      Python is a high-level, interpreted programming language known for clear, readable syntax and a large standard library that speeds development. It supports multiple programming paradigms — procedural, object-oriented, and functional — making it suitable for beginners and experienced developers alike. Common uses include web development, data analysis, scripting, automation, and scientific computing. Python's package ecosystem (installed via pip) provides libraries for almost any task, and its interactive REPL and simple file-based scripts make it easy to experiment and iterate quickly.
    </p>
  </article>





<article class="card" role="article" aria-labelledby="debug-title" style="margin-top:32px;">
  <div class="kicker">Programming</div>
  <h1 id="debug-title">Debugging in Python</h1>
  <p>
    Debugging in Python is the process of identifying and fixing errors so your program runs 
    correctly. It often involves examining error messages, adding temporary print statements 
    to trace values, or using tools like Python's built-in <code>pdb</code> debugger to step 
    through code line by line. Debugging helps you understand why something isn’t working as 
    expected, isolate the issue, and apply a clear fix.
  </p>
</article>






<article class="card" role="article" aria-labelledby="broken-code-title" style="margin-top:32px;">
  <div class="kicker">#1</div>
  <h1 id="broken-code-title">Broken Code Example</h1>
  
  



 ```
temperature = 75

if temperature > 80:
    print("It's hot")

elif temperature > 50:
    print("It's temperate")
    
elif temperature < 0:
    print("It's cold")
```



  
  
  <p>
    So here with python,you would wanna start by reading line by line.The first line starts off with the variable called "temperature",given the value of 75.The second line states a conditional statement whereas when a number higher than 80 is inputted,a print statement will run saying that it's hot.The next line is an elif statement,.In Python, "elif" is a keyword that stands for "else if." It is used in conditional statements to check for multiple conditions sequentially after an initial if statement has evaluated to False.That elif statement explains how if the number inputted is higher than 50,then a print statement will run saying how "it's temperate".The last line has yet another elif statement.This time it checks for a number less than 0.The entire python code snippet simply exists for the purpose of checking the temperature.The error here is that nothing is being accounted for anything greater then 0 but less than 50.To fix this issue Change the final elif to an else statement, this will make sure any temperature less than 50 is determined to be cold
  </p>
</article>

<article class="card" role="article" aria-labelledby="broken-code-title" style="margin-top:32px;">
  <div class="kicker">#2</div>
  <h1 id="broken-code-title">Broken Code Example</h1>
  
  



 ```
text = "Hello, world, my name is"
count = 0

for char in text:
    if char == "":
       count += 1

print(count)
```



  
  
  <p>
    The purpose of this code snippet is to count how many spaces there are in the sentence "Hello world,my name is"
    Right now the count is zero.The code states that for every character within text, if there is "" then count will increase by 1.However when printing the count,there is an error.This is due to the iff statement.The quotation marks have nothing within them.Therefore we need to get them to accept spaces.Simply fixing "" to " " would suffice since there is a space found between the quotation marks.
  </p>
</article>

<article class="card" role="article" aria-labelledby="broken-code-title" style="margin-top:32px;">
  <div class="kicker">#3</div>
  <h1 id="broken-code-title">Broken Code Example</h1>
  
  



 ```
print("give me a number")
n = input()

for num in range(1, n):
    if num % 2 < 0:
        print(num, "is even.")
    else:
        print(num, "is odd.")
```



  
  
  <p>
    This next snippet actually stumped me for like 10 minutes if I'm being honest.Going step by step we start out with the code asking the user for a number.The user then inputs a number.Then getting to the loop,If the numbers within the loop are dived by 2 and their remainder is greater than 0 they are odd,if they have no remainder,then that number will be even.The main issue here is that second line.The input is just excepting strings as inputs,they need to be changed so it accepts numbers as well.Changing "n = input()" to n = int((input)),we allow the input to accept whole numbers.
  </p>
</article>

<article class="card" role="article" aria-labelledby="broken-code-title" style="margin-top:32px;">
  <div class="kicker">#4</div>
  <h1 id="broken-code-title">Broken Code Example</h1>
  
  



 ```
num = int(input("Enter an integer: "))

if num < -1:
  print("No negative numbers.")
else:
  result = 1
  for i in range(1, num):
    result *= i   

  print("Factorial of " + num + "is" + result)
```



  
  
  <p>
    The main issue here is that the for loop cant loop as intended,the for loop is supposed to to loop the number of times between 1 and whatever value num is given.However,num is being excluded.To fix that the for loop must be fixed to for i in range(1,num + 1).That isn't the only issue however.The Problem: You cannot use the addition operator (+) to directly join strings (like "Factorial of ") and integers (num and result).The Fix: You must convert the integers to strings using str() or use an f-string (the recommended modern method) to embed the variables inside the string.
  </p>
</article>

<article class="card" role="article" aria-labelledby="broken-code-title" style="margin-top:32px;">
  <div class="kicker">#5</div>
  <h1 id="broken-code-title">Broken Code Example</h1>
  
  



 ```
attempts = 0
correct_password = "secret"

while True:
    password = input("Enter your password: ")
    attempts += 1

    if password == "incorrect_password":
        print("Correct password!")
    else:
        print("Incorrect password")

    if attempts > 3:
        print("Too many attempts")
        break
```



  
  
  <p>
     The code checks if the user's input equals the text "incorrect_password", not the correct stored secret ("secret"). This means the password can never be accepted.
The Fix: Change the comparison to if password == correct_password:.

Missing Exit on Success: Even if the password were correctly checked, the loop doesn't stop when the right password is entered. It prints "Correct password!" but immediately asks for the password again.
The Fix: Add a break command right after printing "Correct password!"
  </p>
</article>


<article class="card" role="article" aria-labelledby="conclusion-title" style="margin-top:32px;">
  <div class="kicker">Summary</div>
  <h1 id="conclusion-title">Conclusion: Core Debugging Patterns</h1>
  
  <p>
    This experience highlights that effective debugging relies on strict attention to data types (like converting strings to integers) and a thorough understanding of conditional logic and the exact behavior of built-in functions like range and the modulo operator.Nonetheless debugging is a fun practice.
  </p>
</article>




</body>
</html>