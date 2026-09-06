Empowering line 
<html lang="hi">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>कोचिंग डैशबोर्ड | लक्ष्य इंस्टीट्यूट</title>
  <style>
    :root {
      --primary: #0f172a;
      --accent: #2563eb;
      --card: #ffffff;
      --bg: #f1f5f9;
      --text: #334155;
      --highlight: #10b981;
    }

    * {
      box-sizing: border-box;
      margin: 0;
      padding: 0;
      font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, sans-serif;
    }

    body {
      background: var(--bg);
      color: var(--text);
      padding-bottom: 80px;
    }

    .hero-banner {
      width: 100%;
      height: 180px;
      object-fit: cover;
      display: block;
      background-color: #cbd5e1;
    }

    .header-box {
      background: var(--card);
      padding: 16px;
      margin: -25px 16px 16px 16px;
      border-radius: 12px;
      box-shadow: 0 4px 12px rgba(0,0,0,0.06);
      position: relative;
      text-align: center;
    }

    .header-box h1 {
      font-size: 1.5rem;
      color: var(--primary);
    }

    .header-box p {
      font-size: 0.85rem;
      color: #64748b;
      margin-top: 4px;
    }

    .container {
      max-width: 520px;
      margin: 0 auto;
      padding: 0 16px;
    }

    .card {
      background: var(--card);
      border-radius: 12px;
      padding: 18px;
      margin-bottom: 16px;
      border: 1px solid #e2e8f0;
      box-shadow: 0 2px 5px rgba(0,0,0,0.03);
    }

    .card h2 {
      font-size: 1.1rem;
      color: var(--primary);
      margin-bottom: 14px;
      display: flex;
      align-items: center;
      gap: 8px;
    }

    /* फॉर्म स्टाइलिंग */
    .form-group {
      margin-bottom: 12px;
    }

    .form-group label {
      display: block;
      font-size: 0.85rem;
      font-weight: 600;
      margin-bottom: 5px;
      color: #475569;
    }

    .form-control {
      width: 100%;
      padding: 10px 12px;
      border: 1px solid #cbd5e1;
      border-radius: 8px;
      font-size: 0.95rem;
      outline: none;
      transition: border-color 0.2s;
    }

    .form-control:focus {
      border-color: var(--accent);
    }

    .btn-submit {
      width: 100%;
      background: var(--accent);
      color: white;
      border: none;
      padding: 12px;
      font-size: 1rem;
      font-weight: bold;
      border-radius: 8px;
      cursor: pointer;
      margin-top: 6px;
    }

    .btn-submit:hover {
      background: #1d4ed8;
    }

    /* क्विक एक्शन बार */
    .action-bar {
      position: fixed;
      bottom: 0;
      left: 0;
      width: 100%;
      background: var(--card);
      display: flex;
      gap: 10px;
      padding: 12px 16px;
      box-shadow: 0 -3px 12px rgba(0,0,0,0.08);
      z-index: 100;
    }

    .btn {
      flex: 1;
      text-align: center;
      padding: 12px;
      text-decoration: none;
      font-weight: 700;
      border-radius: 8px;
      font-size: 0.9rem;
    }

    .btn-call { background: var(--primary); color: white; }
    .btn-wa { background: var(--highlight); color: white; }
  </style>
</head>
<body>

  <img src="banner.jpg" alt="Coaching Banner" class="hero-banner" onerror="this.src='https://images.unsplash.com/photo-1523240795612-9a054b0db644?w=800&q=80'">

  <div class="header-box">
    <h1>V.N.S Coaching Classes</h1>
    <p>Enroll Today to claim your Free 3-day demo session!</p>
    <h2>Free Trial Classes</h2>
    <p>1-07-2026 to 3-07-2026</p>
  </div>

  <div class="container">

    <!-- डेटा कलेक्शन फॉर्म कार्ड -->
    <div class="card">
      <h2>📝 Admission / Free Demo Classes form</h2>
      
      <!-- Formspree Endpoint: अपनी फॉर्म आईडी यहाँ डालें -->
      <form action="https://formspree.io/f/maeydkyz" method="POST">
        <div class="form-group">
          <label for="student_name">Student Name</label>
          <input type="text" id="student_name" name="name" class="form-control" placeholder="Rahul Sharma" required>
        </div>

        <div class="form-group">
          <label for="phone">Mobile Number (WhatsApp)</label>
          <input type="tel" id="phone" name="phone" class="form-control" placeholder="10 Digit Number" pattern="[0-9]{10}" required>
        </div>

        <div class="form-group">
          <label for="course">Class / Select Course</label>
          <select id="course" name="course" class="form-control" required>
            <option value="">-- Select Course --</option>
            <option value="Class 9">Class 9 (Maths/Science)</option>
            <option value="Class 10">Class 10 (Maths/Science)</option>
            <option value="Class 11 PCM">Class 11 (Physics only)</option>
            <option value="Class 12 PCM">Class 12 (Physics only)</option>
          </select>
        </div>

        <div class="form-group">
          <label for="message">Any questions or suggessions (Optional)</label>
          <textarea id="message" name="message" class="form-control" rows="2" placeholder="Enter your suggessions..."></textarea>
        </div>

        <button type="submit" class="btn-submit">Submit</button>
      </form>
    </div>

    <!-- पता और समय -->
    <div class="card">
      <h2>📍 Contact & Address </h2>
      <p style="font-size: 0.9rem; line-height: 1.5;">
        <strong>Address:</strong> Akash Nagar,Near Tyagi hostel,Gali No 3<br>
        <strong>Time:</strong> 4:00 AM to 8:30 PM
      </p>
    </div>

  </div>
<!-- नेविगेशन बार या बटन के रूप में -->
<div style="text-align: center; margin: 15px 0;">
  <a href="about.html" style="margin: 0 10px; color: #2563eb; font-weight: bold; text-decoration: none;">हमारे बारे में</a> 
  <a href="courses.html" style="margin: 0 10px; color: #2563eb; font-weight: bold; text-decoration: none;">सभी कोर्सेज</a>
</div>

  <!-- क्विक एक्शन बार -->
  <div class="action-bar">
    <a href="tel:+918810220805" class="btn btn-call">📞 कॉल करें</a>
    <a href="https://wa.me/918810220805?text=नमस्ते,%20मुझे%20एडमिशन%20की%20जानकारी%20चाहिए।" class="btn btn-wa">💬 व्हाट्सएप</a>
  </div>

</body>
</html>
