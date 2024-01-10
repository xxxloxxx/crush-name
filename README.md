<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Crush Name Page</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            text-align: center;
            margin: 50px;
        }

        h1 {
            color: #333;
        }

        form {
            margin-top: 20px;
        }

        input[type="text"] {
            padding: 10px;
            font-size: 16px;
        }

        input[type="submit"] {
            padding: 10px 20px;
            font-size: 18px;
            background-color: #4CAF50;
            color: #fff;
            border: none;
            cursor: pointer;
        }

        input[type="submit"]:hover {
            background-color: #45a049;
        }

        #result {
            margin-top: 20px;
            font-size: 18px;
            color: #333;
        }
    </style>
</head>
<body>
    <h1>Write Your Crush's Name</h1>

    <form id="crushForm">
        <label for="crushName">Crush's Name:</label>
        <input type="text" id="crushName" name="crushName" required>
        <br>
        <input type="submit" value="Submit">
    </form>

    <div id="result"></div>

    <script>
        document.getElementById("crushForm").addEventListener("submit", function(event) {
            event.preventDefault();
            var crushName = document.getElementById("crushName").value;
            
            if (crushName.toLowerCase() === "louay") {
                document.getElementById("result").innerText = "Louay too loves you!";
            } else {
                document.getElementById("result").innerText = "Sorry, no love from Louay.";
            }
        });
    </script>
</body>
</html>
