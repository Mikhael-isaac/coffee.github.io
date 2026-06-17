# coffee.github.io
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Important Coffee Business ☕</title>
  <style>
    :root {
      --bg1: #fff6ee;
      --bg2: #f6d7b8;
      --card: #ffffff;
      --text: #4b2e1f;
      --accent: #8b5e3c;
      --accent-dark: #6f472d;
      --soft: #f3e2d3;
      --yes: #7a4b2b;
      --maybe: #c98f59;
      --no: #d8c6b8;
      --shadow: 0 12px 30px rgba(75, 46, 31, 0.15);
    }

    * {
      box-sizing: border-box;
    }

    body {
      margin: 0;
      min-height: 100vh;
      font-family: Arial, Helvetica, sans-serif;
      background: linear-gradient(135deg, var(--bg1), var(--bg2));
      display: flex;
      justify-content: center;
      align-items: center;
      padding: 24px;
      color: var(--text);
      overflow-x: hidden;
    }

    .floating {
      position: fixed;
      font-size: 22px;
      opacity: 0.18;
      animation: float 12s linear infinite;
      pointer-events: none;
      user-select: none;
    }

    .f1 { left: 8%; top: 10%; animation-delay: 0s; }
    .f2 { left: 84%; top: 20%; animation-delay: 2s; }
    .f3 { left: 15%; top: 75%; animation-delay: 4s; }
    .f4 { left: 75%; top: 80%; animation-delay: 1s; }
    .f5 { left: 50%; top: 8%; animation-delay: 3s; }

    @keyframes float {
      0%   { transform: translateY(0px) rotate(0deg); }
      50%  { transform: translateY(-18px) rotate(8deg); }
      100% { transform: translateY(0px) rotate(0deg); }
    }

    .card {
      width: 100%;
      max-width: 560px;
      background: var(--card);
      border-radius: 24px;
      padding: 32px 28px;
      box-shadow: var(--shadow);
      text-align: center;
      position: relative;
    }

    .badge {
      display: inline-block;
      background: var(--soft);
      color: var(--accent-dark);
      padding: 8px 14px;
      border-radius: 999px;
      font-size: 13px;
      font-weight: bold;
      margin-bottom: 16px;
    }

    h1 {
      margin: 0 0 12px;
      font-size: 2rem;
      line-height: 1.2;
      color: var(--accent-dark);
    }

    .subtitle {
      font-size: 1.05rem;
      line-height: 1.6;
      margin: 0 auto 16px;
      max-width: 440px;
    }

    .tiny-joke {
      background: #fff8f1;
      border: 1px dashed #e7c7a8;
      padding: 12px 14px;
      border-radius: 16px;
      font-size: 0.95rem;
      margin: 16px 0 24px;
    }

    .buttons {
      display: flex;
      flex-wrap: wrap;
      justify-content: center;
      gap: 12px;
      margin-bottom: 16px;
    }

    button {
      border: none;
      border-radius: 999px;
      padding: 12px 18px;
      font-size: 15px;
      font-weight: bold;
      cursor: pointer;
      transition: transform 0.15s ease, opacity 0.15s ease, background 0.2s ease;
      min-width: 140px;
    }

    button:hover {
      transform: translateY(-2px);
    }

    .yes {
      background: var(--yes);
      color: white;
    }

    .maybe {
      background: var(--maybe);
      color: white;
    }

    .no {
      background: var(--no);
      color: var(--text);
    }

    .response-box {
      min-height: 28px;
      font-weight: bold;
      margin: 8px 0 20px;
      color: var(--accent-dark);
    }

    .planner {
      display: none;
      margin-top: 20px;
      text-align: left;
      background: #fffaf5;
      border: 1px solid #efd8c2;
      border-radius: 20px;
      padding: 18px;
    }

    .planner.show {
      display: block;
    }

    .planner h2 {
      font-size: 1.15rem;
      margin: 0 0 12px;
      text-align: center;
      color: var(--accent-dark);
    }

    .grid {
      display: grid;
      grid-template-columns: 1fr 1fr;
      gap: 12px;
    }

    .field {
      display: flex;
      flex-direction: column;
      gap: 6px;
    }

    .field.full {
      grid-column: 1 / -1;
    }

    label {
      font-size: 0.92rem;
      font-weight: bold;
    }

    input, select, textarea {
      width: 100%;
      padding: 11px 12px;
      border-radius: 12px;
      border: 1px solid #d9c2ae;
      font-size: 15px;
      outline: none;
      background: white;
      color: var(--text);
    }

    textarea {
      min-height: 90px;
      resize: vertical;
    }

    .send-actions {
      margin-top: 16px;
      display: flex;
      flex-wrap: wrap;
      gap: 12px;
      justify-content: center;
    }

    .wa {
      background: #25D366;
      color: white;
    }

    .mail {
      background: #5b7fff;
      color: white;
    }

    .note {
      font-size: 0.85rem;
      line-height: 1.5;
      margin-top: 14px;
      text-align: center;
      color: #6a5446;
    }

    .footer-line {
      margin-top: 18px;
      font-size: 0.85rem;
      opacity: 0.85;
    }

    .hidden {
      display: none;
    }

    @media (max-width: 600px) {
      .grid {
        grid-template-columns: 1fr;
      }

      h1 {
        font-size: 1.75rem;
      }

      .card {
        padding: 24px 18px;
      }

      button {
        width: 100%;
      }
    }
  </style>
</head>
<body>
  <div class="floating f1">☕</div>
  <div class="floating f2">✨</div>
  <div class="floating f3">☕</div>
  <div class="floating f4">🍪</div>
  <div class="floating f5">😌</div>

  <div class="card">
    <div class="badge">Officially Unofficial Invitation</div>

    <h1>Quick question...<br>Are you free for coffee? ☕</h1>

    <p class="subtitle">
      It could possibly turn out to be a vibe
    </p>

    <div class="tiny-joke">
      Side effects may include: laughing, caffeine, and suspiciously good conversation. - this was ai's idea "puke"
    </div>

    <div class="buttons">
      <button class="yes" onclick="handleChoice('yes')">Yes, obviously ☕</button>
      <button class="maybe" onclick="handleChoice('maybe')">Maybe... impress me 😏</button>
      <button class="no" onclick="handleChoice('no')">No (dramatic) 🎭</button>
    </div>

    <div id="response" class="response-box"></div>

    <div id="planner" class="planner">
      <h2>Pick a date and make this coffee thing official</h2>

      <div class="grid">
        <div class="field">
          <label for="date">Preferred date</label>
          <input type="date" id="date" />
        </div>

        <div class="field">
          <label for="time">Preferred time</label>
          <input type="time" id="time" />
        </div>

        <div class="field full">
          <label for="place">Coffee spot (optional)</label>
          <input type="text" id="place" placeholder="e.g. Seattle Coffee, Bootlegger, or 'surprise me'" />
        </div>

        <div class="field full">
          <label for="note">Optional message</label>
          <textarea id="note" placeholder="e.g. I accept this elite coffee opportunity."></textarea>
        </div>
      </div>

      <div class="send-actions">
        <button class="wa" onclick="sendWhatsApp()">Send via WhatsApp</button>
        <button class="mail" onclick="sendEmail()">Send via Email</button>
      </div>

      <div class="note">
        When they click one of these, it opens a pre-filled WhatsApp or email message to send back.
      </div>
    </div>

    <div class="footer-line">
      Built with caffeine, courage, and excellent taste.
    </div>
  </div>

  <script>
    // ============================
    // UPDATE THESE DETAILS
    // ============================
    const YOUR_NAME = "Mikhael";
    const YOUR_PHONE = "27658080572"; // WhatsApp number in international format, no + or spaces
    const YOUR_EMAIL = "mikhael.isaac@gmail.com";

    const responseEl = document.getElementById("response");
    const plannerEl = document.getElementById("planner");
    const dateEl = document.getElementById("date");

    // Set minimum date to today
    const today = new Date();
    const yyyy = today.getFullYear();
    const mm = String(today.getMonth() + 1).padStart(2, "0");
    const dd = String(today.getDate()).padStart(2, "0");
    dateEl.min = `${yyyy}-${mm}-${dd}`;

    function handleChoice(choice) {
      if (choice === "yes") {
        responseEl.textContent = "Excellent. A strong and intelligent decision. ☕";
        plannerEl.classList.add("show");
      } else if (choice === "maybe") {
        responseEl.textContent = "Understandable. Please review the coffee proposal below and be charmed responsibly 😌";
        plannerEl.classList.add("show");
      } else {
        responseEl.textContent = "That hurts a little... but I respect the theatrical honesty 🎭";
        plannerEl.classList.remove("show");
      }
    }

    function buildMessage() {
      const date = document.getElementById("date").value;
      const time = document.getElementById("time").value;
      const place = document.getElementById("place").value.trim();
      const note = document.getElementById("note").value.trim();

      let lines = [];
      lines.push(`Hey ${YOUR_NAME}! ☕`);

      if (date || time) {
        const whenText = `${date ? `on ${date}` : ""}${date && time ? " at " : ""}${time ? time : ""}`.trim();
        lines.push(`I’m in for coffee ${whenText}.`);
      } else {
        lines.push(`I’m in for coffee!`);
      }

      if (place) {
        lines.push(`Coffee spot suggestion: ${place}`);
      }

      if (note) {
        lines.push(`Message: ${note}`);
      }

      lines.push(`This was sent from your very persuasive coffee page 😄`);

      return lines.join("\n");
    }

    function sendWhatsApp() {
      const date = document.getElementById("date").value;
      if (!date) {
        alert("Pick a date first so your coffee reply looks properly organised ☕");
        return;
      }

      const message = buildMessage();
      const url = `https://wa.me/${YOUR_PHONE}?text=${encodeURIComponent(message)}`;
      window.open(url, "_blank");
    }

    function sendEmail() {
      const date = document.getElementById("date").value;
      if (!date) {
        alert("Pick a date first so the email doesn’t look like chaotic caffeine energy ☕");
        return;
      }

      const subject = "Re: Coffee Invite ☕";
      const body = buildMessage();
      const url = `mailto:${YOUR_EMAIL}?subject=${encodeURIComponent(subject)}&body=${encodeURIComponent(body)}`;
      window.location.href = url;
    }
  </script>
</body>
</html>
