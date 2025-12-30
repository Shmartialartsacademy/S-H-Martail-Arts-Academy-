<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>S H Martial Arts & Self Defense Academy</title>
  <style>
    body {
      margin: 0;
      font-family: Arial, sans-serif;
      background: #f5f5f5;
      color: #222;
    }
    section {
      padding: 30px 20px;
      max-width: 1100px;
      margin: auto;
    }
    h2 {
      margin-bottom: 10px;
    }
    p {
      color: #555;
    }
    .grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(160px, 1fr));
      gap: 15px;
      margin-top: 20px;
    }
    .card {
      background: #fff;
      border-radius: 12px;
      padding: 20px;
      text-align: center;
      box-shadow: 0 4px 10px rgba(0,0,0,0.08);
    }
    .btn {
      display: inline-block;
      margin-top: 20px;
      padding: 14px 25px;
      background: #d4af37;
      color: #000;
      font-weight: bold;
      text-decoration: none;
      border-radius: 10px;
    }
    .gallery img {
      width: 100%;
      border-radius: 12px;
    }
    .coach img {
      width: 100%;
      max-width: 320px;
      border-radius: 15px;
      display: block;
      margin: 0 auto 20px;
    }
    .contact-box {
      display: grid;
      grid-template-columns: 1fr 1fr;
      gap: 20px;
    }
    input, button {
      width: 100%;
      padding: 12px;
      margin-top: 10px;
      border-radius: 8px;
      border: 1px solid #ccc;
    }
    button {
      background: #000;
      color: #fff;
      border: none;
      font-weight: bold;
    }
    @media(max-width: 700px){
      .contact-box {
        grid-template-columns: 1fr;
      }
    }
  </style>
</head>
<body>

<!-- CLASS TIMINGS -->
<section>
  <h2>Class Timings</h2>
  <p>We offer structured classes suitable for children and adults.</p>

  <div class="grid">
    <div class="card">
      <h3>Batch 1</h3>
      <p>5:00 PM – 6:30 PM<br>(Evening)</p>
    </div>
    <div class="card">
      <h3>Batch 2</h3>
      <p>6:00 PM – 7:30 PM<br>(Evening)</p>
    </div>
    <div class="card">
      <h3>Batch 3</h3>
      <p>7:30 PM – 8:30 PM<br>(Evening)</p>
    </div>
    <div class="card">
      <h3>Batch 4</h3>
      <p>8:30 PM – 9:30 PM<br>(Evening)</p>
    </div>
  </div>

  <a class="btn" href="https://wa.me/919782342112">Book Trial – WhatsApp</a>
</section>

<!-- GALLERY -->
<section>
  <h2>Gallery</h2>
  <p>Photos from classes, training sessions and events.</p>

  <div class="grid gallery">
    <img src="img1.jpg">
    <img src="img2.jpg">
    <img src="img3.jpg">
    <img src="img4.jpg">
  </div>
</section>

<!-- COACH -->
<section class="coach">
  <img src="coach.jpg" alt="Coach Abdul Wajid">
  <h2>About Coach Abdul Wajid</h2>
  <p>
    Coach Abdul Wajid is a Self-Defense Diploma Holder and a
    <strong>3rd Dan Kukkiwon Black Belt</strong> in Taekwondo.
    He also holds a <strong>1st Dan Black Belt</strong> in Self-Defense
    and serves as a certified referee and coach.
  </p>
</section>

<!-- CONTACT -->
<section>
  <h2>Contact</h2>

  <div class="contact-box">
    <div>
      <p>
        <strong>S H Martial Arts & Self Defense Academy</strong><br>
        Jodhpur, India<br><br>
        WhatsApp: <strong>+91 97823 42112</strong>
      </p>
    </div>

    <div>
  <h3>Register</h3>

  <input type="text" id="name" placeholder="Student Name" required>
  <input type="number" id="age" placeholder="Age" required>

  <select id="occupation" required>
    <option value="">Father / Mother Occupation</option>
    <option>Business</option>
    <option>Private Job</option>
    <option>Government Job</option>
    <option>Self Employed</option>
    <option>Farmer</option>
    <option>Other</option>
  </select>

  <textarea id="reason" rows="4"
    placeholder="Why do you want to learn Martial Arts?" required></textarea>

  <button onclick="sendWhatsApp()">Submit on WhatsApp</button>
</div>

<script>
function sendWhatsApp() {
  var name = document.getElementById("name").value;
  var age = document.getElementById("age").value;
  var occupation = document.getElementById("occupation").value;
  var reason = document.getElementById("reason").value;

  if (!name || !age || !occupation || !reason) {
    alert("Please fill all details");
    return;
  }

  var phoneNumber = "919782342112"; // academy WhatsApp number

  var message =
    "New Registration%0A%0A" +
    "Name: " + name + "%0A" +
    "Age: " + age + "%0A" +
    "Parent Occupation: " + occupation + "%0A" +
    "Reason: " + reason;

  window.open(
    "https://wa.me/" + phoneNumber + "?text=" + message,
    "_blank"
  );
}
</script>
