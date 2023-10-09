# To_Do_List_WebApp
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Simple To-Do List</title>
    <style>
        /* Add your CSS styles here */
    </style>
</head>
<body>
    <h1>My To-Do List</h1>
    <div>
        <input type="text" id="taskInput" placeholder="Add a task">
        <button onclick="addTask()">Add</button>
    </div>
    <ul id="taskList">
        <!-- Tasks will be displayed here -->
    </ul>
    <script>
        function addTask() {
            // Get the task input value
            var taskText = document.getElementById("taskInput").value;

            // Create a new list item
            var li = document.createElement("li");
            li.appendChild(document.createTextNode(taskText));

            // Add the task to the task list
            document.getElementById("taskList").appendChild(li);

            // Clear the input field
            document.getElementById("taskInput").value = "";
        }
    </script>
</body>
</html>

