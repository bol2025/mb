<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Wazzlitt Roadside and Machine Assistance</title>
  <link rel="stylesheet" href="styles.css" />
</head>
<body>
  <header>
    <h1>Wazzlitt Roadside and Machine Assistance</h1>
    <p>Quick and Reliable Help When You Need It!</p>
  </header>

  <main>
    <section id="order-form">
      <h2>Request Assistance</h2>
      <form id="assistanceForm">
        <label for="name">Full Name:</label>
        <input type="text" id="name" name="name" required />

        <label for="phone">Phone Number:</label>
        <input type="tel" id="phone" name="phone" required />

        <label for="location">Current Location:</label>
        <input type="text" id="location" name="location" required />

        <label for="problem">Describe Your Problem:</label>
        <textarea id="problem" name="problem" rows="4" required></textarea>

        <button type="submit">Submit Request</button>
      </form>
    </section>

    <section id="contact">
      <h2>Contact Us</h2>
      <p>Need more information? Call us at <strong>123-456-7890</strong></p>
    </section>
  </main>

  <footer>
    <p>&copy; 2025 Wazzlitt Roadside and Machine Assistance. All Rights Reserved.</p>
  </footer>

  <script>
    document.getElementById('assistanceForm').addEventListener('submit', function(event) {
      event.preventDefault();

      const name = document.getElementById('name').value;
      const phone = document.getElementById('phone').value;
      const location = document.getElementById('location').value;
      const problem = document.getElementById('problem').value;

      alert(`Request Received! \nName: ${name}\nPhone: ${phone}\nLocation: ${location}\nProblem: ${problem}`);

      // In a real application, send the data to a server here.
    });
  </script>
</body>
</html>
