<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Cybersecurity Career Roadmap Seminar</title>
  <style>
    /* General Styles */
    body {
      font-family: Arial, sans-serif;
      line-height: 1.6;
      margin: 0;
      padding: 0;
      background-color: #f5f5f5;
    }

    h1, h2, h3 {
      color: #333;
    }

    /* Responsive Banner */
    .banner {
      max-width: 100%;
      height: auto;
      display: block;
      margin: 20px auto;
      box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
      border-radius: 8px;
    }

    /* Countdown Timer */
    #countdown {
      text-align: center;
      font-size: 2em;
      font-weight: bold;
      color: #e63946;
      margin: 20px 0;
    }

    /* Responsive Speaker Section */
    .speaker-section {
      display: flex;
      flex-wrap: wrap;
      gap: 20px;
      align-items: center;
      justify-content: center;
      padding: 20px;
      background-color: #fff;
      border-radius: 8px;
      box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
    }

    .speaker-image {
      flex: 0 1 150px;
      border-radius: 50%;
      box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
    }

    .speaker-details {
      flex: 1;
      text-align: left;
      padding: 10px;
    }

    /* Buttons */
    .btn {
      display: inline-block;
      background-color: #007bff;
      color: white;
      padding: 10px 20px;
      margin: 10px 0;
      text-decoration: none;
      border-radius: 5px;
      text-align: center;
    }

    .btn:hover {
      background-color: #0056b3;
    }

    /* Responsive Media Queries */
    @media (max-width: 768px) {
      .speaker-section {
        flex-direction: column;
        text-align: center;
      }

      .speaker-image {
        margin-bottom: 15px;
      }
    }
  </style>
</head>
<body>

  <!-- Seminar Banner -->
  <div>
    <img src="https://raw.githubusercontent.com/SecureByteOfficial/live-seminars/main/sbdec6.png" 
         alt="Seminar Banner" class="banner">
  </div>

  <!-- Countdown Section -->
  <div id="countdown"></div>
  <p style="text-align: center;">Days Left to Join</p>

  <!-- Guest Speaker Section -->
  <div class="speaker-section">
    <img src="https://pbs.twimg.com/profile_images/1844791721571602432/M4jiVjeE_400x400.jpg" 
         alt="Naem Azam Chowdhury" class="speaker-image">
    <div class="speaker-details">
      <h3>Naem Azam Chowdhury</h3>
      <p><strong>Position:</strong> Security Researcher, China</p>
      <p><strong>Expertise:</strong> Cybersecurity, Ethical Hacking, AI, Web Development</p>
      <p>Naem Azam Chowdhury is a renowned cybersecurity expert leading innovative research and development in cybersecurity and AI. With a gold medal in Computer Science and an MS in Cybersecurity, Naem is dedicated to educating the next generation of cybersecurity professionals.</p>
      <a href="https://www.youtube.com/@NaemAzamChowdhury" class="btn">YouTube Channel</a>
      <a href="https://x.com/naemazamchow" class="btn" style="background-color: #1DA1F2;">Twitter</a>
    </div>
  </div>

  <!-- Countdown Timer Script -->
  <script>
    const countDownDate = new Date("December 6, 2024 20:00:00").getTime();

    // Update countdown every second
    const x = setInterval(function() {
      const now = new Date().getTime();
      const distance = countDownDate - now;

      // Calculate time left
      const days = Math.floor(distance / (1000 * 60 * 60 * 24));
      const hours = Math.floor((distance % (1000 * 60 * 60 * 24)) / (1000 * 60 * 60));
      const minutes = Math.floor((distance % (1000 * 60)) / (1000 * 60));
      const seconds = Math.floor((distance % 1000) / 1000);

      // Display result
      document.getElementById("countdown").innerHTML = `${days}d ${hours}h ${minutes}m ${seconds}s`;

      // If the countdown is finished
      if (distance < 0) {
        clearInterval(x);
        document.getElementById("countdown").innerHTML = "The Cybersecurity Career Roadmap Seminar is Live Now!";
      }
    }, 1000);
  </script>

</body>
</html>
