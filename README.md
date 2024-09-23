<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Registration Form</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #f4f4f4;
            margin: 0;
            padding: 0;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
        }

        form {
            background: white;
            padding: 20px;
            border-radius: 8px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
        }

        h1 {
            text-align: center;
            color: #333;
        }

        label {
            font-weight: bold;
            display: block;
            margin-top: 20px;
            color: #555;
        }

        input[type="text"],
        input[type="email"],
        input[type="tel"] {
            width: calc(100% - 22px);
            padding: 10px;
            margin-top: 5px;
            margin-bottom: 10px;
            border: 1px solid #ddd;
            border-radius: 4px;
            box-sizing: border-box;
        }

        input[type="submit"] {
            width: 100%;
            padding: 10px;
            background-color: #5c67f2;
            border: none;
            border-radius: 4px;
            color: white;
            font-size: 16px;
            cursor: pointer;
            margin-top: 20px;
        }

        input[type="submit"]:hover {
            background-color: #4a54e1;
        }
    </style>
</head>
<body>
    <form id="registrationForm">
        <h1>User Registration</h1>
        <label for="email">Email:</label>
        <input type="email" id="email" name="email">

        <label for="firstname">First Name:</label>
        <input type="text" id="firstname" name="firstname">

        <label for="lastname">Last Name:</label>
        <input type="text" id="lastname" name="lastname">

        <label for="role">Role in Company:</label>
        <input type="text" id="role" name="role">

        <label for="company">Company Name:</label>
        <input type="text" id="company" name="company">

        <label for="address">Address:</label>
        <input type="text" id="address" name="address">

        <label for="phone">Phone Number:</label>
        <input type="tel" id="phone" name="phone">

        <input type="submit" value="Submit">
    </form>

    <script>
        document.getElementById('registrationForm').addEventListener('submit', function(event) {
            event.preventDefault(); // Prevent the default form submission
            alert('Form submitted successfully! Ready for new input.');
            this.reset(); // Reset the form fields for new input
        });
    </script>
</body>
</html>
