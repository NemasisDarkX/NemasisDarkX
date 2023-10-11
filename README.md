<p align="center">
<h3 align="center">I AM GLITCH </h3>

  

<a href="https://github.com/NemasisDarkX" style="display: block; text-align: center;"><img src="https://profile-48ks.onrender.com/image?" border="0"></a>





</p>
<br/>
<p><b>I'm good at: </p></b>

![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)
![JavaScript](https://img.shields.io/badge/javascript-%23323330.svg?style=for-the-badge&logo=javascript&logoColor=%23F7DF1E)
![MySQL](https://img.shields.io/badge/mysql-%2300f.svg?style=for-the-badge&logo=mysql&logoColor=white)
<h2 align="center">🏆 Github Trophies</h2>
<img align="center"
  src="https://github-profile-trophy.vercel.app/?username=NemasisDarkX&theme=juicyfresh&&title=Stars,Followers,Commit,PR,Repo,Issues&no-frame=true"
  width="100%" />
<br />

## 📊 Github Stats <img align="right" src="https://img.shields.io/github/stars/NemasisDarkX?label=Stars&style=social" alt="GitHub Badge"> <a href="https://github.com/NemasisDarkX?tab=followers"><img align="right" src="https://img.shields.io/github/followers/NemasisDarkX?label=Followers&style=social" alt="GitHub Badge"></a> 



<a href="https://github.com/NemasisDarkX"><img alt="NemasisDarkX's Github Stats"
    src="https://github-readme-stats.vercel.app/api?username=NemasisDarkX&show_icons=true&count_private=true&theme=react&bg_color=151515" /></a>
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

<br />

## 📊 Stack Overflow stats ![](https://img.shields.io/stackexchange/stackoverflow/r/19911293?color=orange&label=reputation&logo=stackoverflow&style=for-the-badge&cacheSeconds=86400)


<a href="https://stackoverflow.com/users/19911293/abhay"><img src="https://stackoverflow.com/users/flair/19911293.png" width="208" height="58" alt="profile for Abhay at Stack Overflow, Q&amp;A for professional and enthusiast programmers" title="profile for Abhay at Stack Overflow, Q&amp;A for professional and enthusiast programmers"></a>
<br/>

