# 🌟 Project Name
     MUSIC PLAYER
     
## 📌 Description
This code creates a visually engaging music player sign-in page using HTML and CSS. The background features a smooth gradient transition with a subtle animated particle effect to enhance the design. The main content is a centered sign-in container with a welcoming message and a button labeled "Click ME." The container has a modern card-style design, featuring a semi-transparent white background, rounded corners, and a soft drop shadow to create a polished look. The button is designed with a vibrant gradient color, smooth hover effects, and a slight scaling animation for an interactive feel. Additionally, the page includes a fade-in animation to make elements appear smoothly upon loading. The layout is also responsive, adjusting for smaller screens to maintain usability.

## 🎨 Demo Preview (HTML & CSS)
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Music Player</title>
  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
      font-family: Arial, sans-serif;
    }

    body {
      display: flex;
      justify-content: center;
      align-items: center;
      min-height: 100vh;
      overflow: hidden;
      position: relative;
      background: linear-gradient(135deg, #7ee8fa, #80ff72); /* Brighter colors */
      color: white;
    }

    .particle-bg {
      position: absolute;
      top: 0;
      left: 0;
      width: 100%;
      height: 100%;
      background: radial-gradient(rgba(255, 255, 255, 0.15) 10%, transparent 70%);
      background-size: cover;
      animation: moveParticles 30s linear infinite;
      z-index: 0;
      opacity: 0.1; /* Very subtle effect */
    }

    @keyframes moveParticles {
      0% { transform: translate(0, 0); }
      100% { transform: translate(-50px, -50px); }
    }

    .sign-in-container {
      background: rgba(255, 255, 255, 0.9);
      padding: 40px;
      width: 90%;
      max-width: 400px;
      border-radius: 12px;
      box-shadow: 0 4px 20px rgba(0, 0, 0, 0.2);
      text-align: center;
      position: relative;
      z-index: 1;
      animation: fadeIn 1s ease-in-out;
      color: #333;
    }

    .sign-in-container h2 {
      margin-bottom: 20px;
      font-size: 26px;
      color: #222; /* Dark text for better contrast */
      text-shadow: 2px 2px 6px rgba(255, 255, 255, 0.8); /* Light glow */
    }

    .sign-in-container button {
      width: 100%;
      padding: 12px;
      background: #ff7e5f;
      border: none;
      border-radius: 6px;
      color: white;
      font-weight: bold;
      cursor: pointer;
      transition: background 0.3s ease, transform 0.2s ease, box-shadow 0.2s ease;
      margin-top: 10px;
    }

    .sign-in-container button:hover {
      background: #ff6a95;
      transform: scale(1.05);
      box-shadow: 0 4px 15px rgba(255, 106, 149, 0.5);
    }

    @keyframes fadeIn {
      from { opacity: 0; }
      to { opacity: 1; }
    }

    @media (max-width: 500px) {
      .sign-in-container {
        padding: 30px 20px;
      }
    }
  </style>
</head>
<body>
  <div class="particle-bg"></div>
  <div class="sign-in-container">
    <h2>Welcome to my Project 🎶🎶</h2>
    <button type="submit" class="button">Click ME</button>
  </div>
</body>
</html>

