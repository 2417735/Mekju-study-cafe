# Mekju-study-cafe
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Mekju Study Cafe</title>
    <style>
        body {
            font-family: 'Georgia', serif;
            background: linear-gradient(45deg, #ff9a9e, #fad0c4, #fad0c4, #ffdde1);
            height: 100vh;
            margin: 0;
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            text-align: center;
        }
        .bio {
            position: absolute;
            top: 20px;
            left: 20px;
            background: rgba(255, 255, 255, 0.7);
            padding: 10px;
            border-radius: 10px;
            box-shadow: 2px 2px 10px rgba(0, 0, 0, 0.2);
        }
        .bio p { margin: 5px 0; }
        .buttons {
            margin-top: 20px;
        }
        button {
            padding: 10px 20px;
            margin: 10px;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            font-size: 16px;
        }
        .chat-btn { background-color: #ff5733; color: white; }
        .assignment-btn { background-color: #33aaff; color: white; }
        .video-btn { background-color: #33cc33; color: white; }
        .book-btn { background-color: #ffcc00; color: white; }
        .chat-btn:hover, .assignment-btn:hover, .video-btn:hover, .book-btn:hover {
            opacity: 0.8;
        }
        .chat-images {
            display: none;
            position: absolute;
            bottom: 80px;
            right: 20px;
            background: white;
            padding: 10px;
            border-radius: 10px;
            box-shadow: 2px 2px 10px rgba(0, 0, 0, 0.2);
        }
    </style>
</head>
<body>
    <div class="bio">
        <p><strong>Name:</strong> ALAM AL KAHAF</p>
        <p><strong>Country:</strong> Bangladesh</p>
        <p><strong>Phone:</strong> 01096724615</p>
        <p><strong>Email:</strong> 2417735@donga.ac.kr</p>
    </div>
    <h1 style="font-family: 'Georgia', serif;">Mekju Study Cafe</h1>
    <div class="buttons">
        <button class="chat-btn" onclick="toggleChat()">Chat</button>
        <button class="assignment-btn" onclick="window.open('https://drive.google.com/drive/folders/1HEdPj6teJZ1kTmk-r2uzcGFjHI3ncf54', '_blank')">Assignment Submission</button>
        <button class="video-btn" onclick="window.open('https://drive.google.com/drive/folders/1In0_BGQVpAGaC2XHtIBeXNaIMkTAj5mN', '_blank')">Video Lecture</button>
        <button class="book-btn" onclick="window.open('https://forms.gle/sZsmRFRkNVZbYWn4A', '_blank')">Book A Date</button>
    </div>
    <div class="chat-images" id="chatImages">
        <img src="https://via.placeholder.com/150" alt="Chat Image 1">
        <img src="https://via.placeholder.com/150" alt="Chat Image 2">
    </div>
    <script>
        function toggleChat() {
            var chatDiv = document.getElementById('chatImages');
            chatDiv.style.display = (chatDiv.style.display === 'none' || chatDiv.style.display === '') ? 'block' : 'none';
        }
    </script>
</body>
</html>


