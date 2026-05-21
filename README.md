# Ex03 To-Do List using JavaScript
## Date:21-05-2026

## AIM
To create a To-do Application with all features using JavaScript.

## ALGORITHM
### STEP 1
Build the HTML structure (index.html).

### STEP 2
Style the App (style.css).

### STEP 3
Plan the features the To-Do App should have.

### STEP 4
Create a To-do application using Javascript.

### STEP 5
Add functionalities.

### STEP 6
Test the App.

### STEP 7
Open the HTML file in a browser to check layout and functionality.

### STEP 8
Fix styling issues and refine content placement.

### STEP 9
Deploy the website.

### STEP 10
Upload to GitHub Pages for free hosting.

## PROGRAM
```
<!doctype html>
<html>
<head>
    <title>To-do List</title>
    <style>
        body {
            font-family: Arial;
            background-color: #e6c18f;
            display: flex;
            justify-content: center;
            margin-top: 80px;
        }

        .container {
            background-color: white;
            width: 350px;
            padding: 20px;
            border-radius: 10px;
        }

        h2 {
            text-align: center;
        }

        .input-box {
            display: flex;
            gap: 10px;
        }

        input {
            flex: 1;
            padding: 10px;
            border: 1px solid gray;
            border-radius: 5px;
        }

        button {
            padding: 10px;
            border: none;
            border-radius: 5px;
            cursor: pointer;
        }

        .add-btn {
            background-color: orange;
            color: white;
        }

        li {
            background-color: #f2f2f2;
            margin-top: 10px;
            padding: 10px;
            border-radius: 5px;

            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .delete-btn {
            background-color: red;
            color: white;
        }

    </style>
</head>
<body>
    <div class="container">

        <h2>TO-DO LIST</h2>
        <dv class="input-box">

            <input type="text" id="taskInput" placeholder="Enter task">
            <button onclick="addtask()">Add</button>
        </dv>
        <ul id="tasklist"></ul>
        
    </div>
    <script>
        function addtask(){
            let input= document.getElementById("taskInput");
            let task = input.value;

            if(task == ""){
                alert("Enter a task!!!");
                return;
            }
            let li= document.createElement("li");
            li.textContent = task + " ";

            let delBtn = document.createElement("button");
            delBtn.textContent = "Delete";

            delBtn.onclick = function(){
                li.remove();
            }

            li.appendChild(delBtn);

            document.getElementById("tasklist").appendChild(li);
            input.value="";


            

        }
    </script>


</body>
</html>
```


## OUTPUT


## RESULT
The program for creating To-do list using JavaScript is executed successfully.
