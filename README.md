# VNS-classes
VNS CLASSES
<html lang="hi">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>COACHING DASHBOARD | VNS CLASSES</title>
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

    /* टॉप हीरो व बैनर */
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

    /* डैशबोर्ड स्टेट्स ग्रिड */
    .stats-grid {
      display: grid;
      grid-template-columns: repeat(3, 1fr);
      gap: 10px;
      margin-bottom: 16px;
    }

    .stat-card {
      background: var(--card);
      padding: 12px 6px;
      border-radius: 10px;
      text-align: center;
      border: 1px solid #e2e8f0;
    }

    .stat-card .number {
      font-size: 1.2rem;
      font-weight: 800;
      color: var(--accent);
    }

    .stat-card .label {
      font-size: 0.75rem;
      color: #64748b;
      margin-top: 2px;
    }

    /* डैशबोर्ड कार्ड */
    .card {
      background: var(--card);
      border-radius: 12px;
      padding: 16px;
      margin-bottom: 16px;
      border: 1px solid #e2e8f0;
    }

    .card h2 {
      font-size: 1.1rem;
      color: var(--primary);
      margin-bottom: 12px;
      display: flex;
      align-items: center;
      gap: 8px;
    }

    /* कोर्स ग्रिड */
    .course-list {
      display: flex;
      flex-direction: column;
      gap: 10px;
    }

    .course-item {
      display: flex;
      justify-content: space-between;
      align-items: center;
      padding: 10px;
      background: #f8fafc;
      border-radius: 8px;
      border-left: 3px solid var(--accent);
    }

    .course-item span {
      font-weight: 600;
      font-size: 0.9rem;
    }

    .badge-status {
      background: #dcfce7;
      color: #166534;
      font-size: 0.75rem;
      padding: 3px 8px;
      border-radius: 12px;
      font-weight: bold;
    }

    /* फ़ोटो गैलरी */
    .gallery-grid {
      display: grid;
      grid-template-columns: repeat(2, 1fr);
      gap: 10px;
    }

    .gallery-grid img {
      width: 100%;
      height: 110px;
      object-fit: cover;
      border-radius: 8px;
      background: #e2e8f0;
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

  <!-- टॉप बैनर इमेज (GitHub पर banner.jpg अपलोड करें) -->
  <img src="banner.jpg" alt="Coaching Banner" class="hero-banner" onerror="this.src='https://images.unsplash.com/photo-1523240795612-9a054b0db644?w=800&q=80'">

  <div class="header-box">
    <h1>लक्ष्य करियर इंस्टीट्यूट</h1>
    <p>गुणवत्तापूर्ण शिक्षा, बेहतर परिणाम</p>
  </div>

  <div class="container">

    <!-- डैशबोर्ड आंकड़े (Stats) -->
    <div class="stats-grid">
      <div class="stat-card">
        <div class="number">10+</div>
        <div class="label">वर्षों का अनुभव</div>
      </div>
      <div class="stat-card">
        <div class="number">95%+</div>
        <div class="label">सर्वश्रेष्ठ रिज़ल्ट</div>
      </div>
      <div class="stat-card">
        <div class="number">20</div>
        <div class="label">छात्र प्रति बैच</div>
      </div>
    </div>

    <!-- उपलब्ध कोर्सेस -->
    <div class="card">
      <h2>📚 उपलब्ध बैच एवं सीटें</h2>
      <div class="course-list">
        <div class="course-item">
          <span>कक्षा 9 - 10 (Science & Maths)</span>
          <span class="badge-status">एडमिशन ओपन</span>
        </div>
        <div class="course-item">
          <span>कक्षा 11 - 12 (PCM / PCB)</span>
          <span class="badge-status">सीमित सीटें</span>
        </div>
        <div class="course-item">
          <span>JEE / NEET फाउंडेशन</span>
          <span class="badge-status">नया बैच</span>
        </div>
      </div>
    </div>

    <!-- क्लासरूम / फैकल्टी गैलरी -->
    <div class="card">
      <h2>📸 क्लासरूम व एक्टिविटीज</h2>
      <div class="gallery-grid">
        <!-- यहाँ अपनी फ़ोटो के नाम डालें जैसे classroom1.jpg, teacher.jpg -->
        <img src="classroom1.jpg" alt="Classroom" onerror="this.src='https://images.unsplash.com/photo-1580582932707-520aed937b7b?w=400&q=80'">
        <img src="classroom2.jpg" alt="Lab/Library" onerror="this.src='https://images.unsplash.com/photo-1497633762265-9d179a990aa6?w=400&q=80'">
      </div>
    </div>

    <!-- पता और समय -->
    <div class="card">
      <h2>📍 सेंटर का पता</h2>
      <p style="font-size: 0.9rem; line-height: 1.4;">
        प्लॉट नं. 24, मुख्य बाजार, बस स्टैंड के पास。<br>
        <strong>समय:</strong> सुबह 8:00 AM से शाम 7:30 PM
      </p>
    </div>

  </div>

  <!-- क्विक बटन -->
  <div class="action-bar">
    <a href="tel:+919876543210" class="btn btn-call">📞 कॉल करें</a>
    <a href="https://wa.me/919876543210?text=नमस्ते,%20मुझे%20एडमिशन%20की%20जानकारी%20चाहिए।" class="btn btn-wa">💬 व्हाट्सएप</a>
  </div>

</body>
</html>
