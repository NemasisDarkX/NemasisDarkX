<!DOCTYPE html>
<html>
<head>
  <title>Brainshop AI Chat</title>
</head>
<body>
  <p align="center">
    <h3 align="center">I AM GLITCH </h3>

    <a href="https://github.com/NemasisDarkX" style="display: block; text-align: center;"><img src="https://profile-48ks.onrender.com/image?" border="0"></a>
  </p>
  <br/>

  <p><b>I'm good at:</b></p>
  <img src="https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54">
  <img src="https://img.shields.io/badge/javascript-%23323330.svg?style=for-the-badge&logo=javascript&logoColor=%23F7DF1E">
  <img src="https://img.shields.io/badge/mysql-%2300f.svg?style=for-the-badge&logo=mysql&logoColor=white">

  <h2 align="center">🏆 Github Trophies</h2>
  <img align="center" src="https://github-profile-trophy.vercel.app/?username=NemasisDarkX&theme=juicyfresh&&title=Stars,Followers,Commit,PR,Repo,Issues&no-frame=true" width="100%" />

  <div id="chat-container">
    <div id="chat-log">
      <!-- Chat messages will be displayed here -->
    </div>
    <input type="text" id="user-input" placeholder="Type a message...">
    <button onclick="sendMessage()">Send</button>
  </div>

  <!-- JavaScript to interact with Brainshop AI -->
  <script>
    function sendMessage() {
      const userMessage = document.getElementById('user-input').value;
      
      // Display user message in the chat log
      displayMessage('You', userMessage);
      
      // Replace the API URL with the actual Brainshop AI API endpoint
      fetch('http://api.brainshop.ai/get?bid=178372&key=22YiicEpyQBVZnpm&uid=YOUR_USER_ID&msg=' + encodeURIComponent(userMessage), {
        method: 'GET', // You should use GET for Brainshop AI
        headers: {
          'Content-Type': 'application/json',
          // Add any required headers here
        }
      })
      .then(response => response.json())
      .then(data => {
        const aiResponse = data.cnt;
        // Display AI response in the chat log
        displayMessage('AI', aiResponse);
      })
      .catch(error => {
        console.error('Error sending message to Brainshop AI', error);
      });
    }

    function displayMessage(sender, message) {
      const chatLog = document.getElementById('chat-log');
      const messageElement = document.createElement('p');
      messageElement.textContent = `${sender}: ${message}`;
      chatLog.appendChild(messageElement);
    }
  </script>
</body>
</html>
