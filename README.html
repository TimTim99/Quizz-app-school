<!DOCTYPE html>
<html lang="de">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Kontraste Quiz App</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      background: url('https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Fimg.fotocommunity.com%2Fkontraste-c878b2c8-ba85-40e9-8333-fbcc8fd74d94.jpg%3Fheight%3D1080&f=1&nofb=1&ipt=6db44f370ef040eecdae135936dfa6095e5357ee4778b73a9855f3466e7e787c') no-repeat center center fixed;
      background-size: cover;
      margin: 0;
      padding: 0;
      color: #111;
    }
    .menu {
      position: fixed;
      top: 1rem;
      left: 1rem;
      z-index: 10;
    }
    .menu button {
      padding: 0.5rem 1rem;
      font-size: 1rem;
      background-color: #111827;
      color: white;
      border: none;
      border-radius: 0.5rem;
      cursor: pointer;
    }
    .question-list {
      display: none;
      position: fixed;
      top: 4rem;
      left: 1rem;
      background: white;
      padding: 1rem;
      border-radius: 0.5rem;
      box-shadow: 0 2px 8px rgba(0,0,0,0.2);
      max-height: 80vh;
      overflow-y: auto;
      z-index: 10;
      width: 320px;
    }
    .question-list ul {
      list-style: none;
      padding: 0;
      margin: 0;
    }
    .question-list li {
      padding: 0.5rem;
      cursor: pointer;
      border-bottom: 1px solid #eee;
    }
    .question-list li:hover {
      background: #f3f4f6;
    }
    .quiz-container {
      background: rgba(255, 255, 255, 0.95);
      padding: 2rem;
      border-radius: 1rem;
      box-shadow: 0 4px 12px rgba(0, 0, 0, 0.2);
      max-width: 700px;
      margin: 10vh auto;
    }
    h1 {
      font-size: 1.5rem;
      margin-bottom: 1rem;
    }
    input[type="text"] {
      width: 100%;
      padding: 0.5rem;
      font-size: 1rem;
      margin-top: 1rem;
      border: 1px solid #ccc;
      border-radius: 0.5rem;
    }
    button {
      margin-top: 1rem;
      padding: 0.5rem 1rem;
      font-size: 1rem;
      background-color: #2563eb;
      color: white;
      border: none;
      border-radius: 0.5rem;
      cursor: pointer;
    }
    .feedback {
      margin-top: 1rem;
      font-weight: bold;
      min-height: 1.5em;
    }
  </style>
</head>
<body>
  <div class="menu">
    <button onclick="toggleMenu()">📋 Menü</button>
    <div class="question-list" id="questionList"></div>
  </div>

  <div class="quiz-container">
    <button onclick="speakQuestion()">🔊 Frage vorlesen</button>
    <h1 id="question">Frage wird geladen...</h1>
    <input type="text" id="answer" placeholder="Deine Antwort hier..." autocomplete="off" />
    <button onclick="checkAnswer()">Antwort prüfen</button>
    <div class="feedback" id="feedback"></div>
    <button onclick="nextQuestion()">Nächste Frage</button>
  </div>

  <script>
    const questions = [
      { question: "Wie nennt man den Kontrast, bei dem Farben in verschiedenen Größenverhältnissen zueinander auftreten und ihre Wirkung sich dadurch verändert?", answer: "Quantitätskontrast" },
      { question: "Wie heißt der Kontrast, bei dem eine reine Farbe mit einer getrübten Farbe verglichen wird?", answer: "Qualitätskontrast" },
      { question: "Welcher Kontrast nutzt reine, kräftige Farben wie Rot, Gelb und Blau nebeneinander?", answer: "Farbe-an-sich-Kontrast" },
      { question: "Welcher Kontrast entsteht durch den Unterschied zwischen hellen und dunklen Farben?", answer: "Hell-Dunkel-Kontrast" },
      { question: "Wie heißt der Kontrast, bei dem warme und kalte Farben gegenübergestellt werden?", answer: "Kalt-Warm-Kontrast" },
      { question: "Wie nennt man den Kontrast, bei dem sich Farbpaare im Farbkreis genau gegenüberliegen, wie zum Beispiel Grün und Rot?", answer: "Komplementärkontrast" },
      { question: "Wieviel Karat muss Gold für Beschriftungen im Außenbereich mindestens aufweisen?", answer: "23 1/2 Karat" },
      { question: "Welche Funktion hat das Vorschaltgerät bei Leuchtstofflampen, auch \"Trafo\" oder \"Konverter\" genannt?", answer: "Es heizt die Elektroden vor, Liefert die Zündspannung und begrenzt den darauf folgenden Entladestorm" },
      { question: "Die Leistungsaufnahme eines elektrischen Verbrauchers errechnet man aus", answer: "P=U•I" },
      { question: "Welche Maßnahme erhöht die Sicherheit von elektrischen Beleuchtungsanlagen?", answer: "Fehlerschutzschalter anbringen für Schutz von Personen, Verwendung von geprüften und zugelassenen Komponenten, Installation und Wartung durch Fachpersonal, Bohren von Wasserlöchern, Regelmäßige Wartung/Inspektion" },
      { question: "Welche Profilnummer für die Bezeichnung von der Lichtwerbung ist gebräuchlich?", answer: "01, 1, 2, 3, 4, 5, 6, 7, 8, 9a, 9b, 10, 11LED, 12LED" },
      { question: "Kann weißes Licht durch Farbmischung roter, grüner und blauer LEDs erzeugt werden?", answer: "Ja kann dadurch erstellt werden" },
      { question: "Haben LEDs ein äußerst kurze Lebensdauer?", answer: "Nein" },
      { question: "Lassen sich mit LEDs keine Lichtwerbeanlagen mit geringen Bautiefen herstellen?", answer: "Nein" },
      { question: "Sind LEDs im Aufbau den Leuchstoffröhren sehr ähnlich?", answer: "Nein" },
      { question: "Ist ein Vorteil von LEDs in der Lichtwerbung ihr hoher Stromverbrauch?", answer: "Nein" },
      { question: "Ist ein Vorteil von LEDs in der Lichtwerbung der äußerst geringe Anschaffungspreis?", answer: "Nein" },
      { question: "Ist ein Vorteil von LEDs in der Lichtwerbung ihr Stromversorgung über Wireless LAN?", answer: "Nein" },
      { question: "Ist ein Vorteil von LEDs in der Lichtwerbung ihr kompakte Bauform?", answer: "Ja" },
      { question: "Wie kann ein Holzuntergrund richtig zur Beschichtung vorbereitet werden?", answer: "Alte Beschichtung entfernen, Holz anfeuchten, Holz schleifen, Staub/Verunreinigungen entfernen, Beschichtung auftragen" },
      { question: "Ein mit Schrauben auf die Wand montiertes Acrylschild wölbt sich nach vorne. Nennen Sie zwei mögliche Montagefehler!", answer: "Keine Langlöcher gemacht, Schrauben zu fest, Temperaturbedingungen nicht beachtet" },
      { question: "Worüber hätte der Werbetechniker sich für eine fachgerechte Montage informieren müssen?", answer: "Wärmeausdehnungskoeffizienten, Temperatur vor Ort" },
      { question: "Nennen Sie den Wärmeausdehnungs-Koeffizienten α für PMMA mit Einheiten!", answer: "70 x 10 Hoch-6 m/mxK" },
      { question: "Was gibt der »MAK-Wert« an!", answer: "Maximale Arbeitsplatz Konzentration" },
      { question: "Nennen Sie drei Trocknungsarten von Anstrichmitteln!", answer: "-Chemische\n-Physikalische\n-Kalter FLuss" },
      { question: "Nennen Sie drei zeichnerische Vergrößerungsverfahren!", answer: "-Rastervergrößerung\n-Maßstabvergrößerung\n-Fluchtpunktvergrößerung" },
      { question: "Erklären Sie die Bedeutung des Begriffs »Kompositionsgold«!", answer: "Ist eine Preiswerte Alternative zu Gold, meist 85% Messing & 15% Zink, nicht für den außenbereich geeignet" },
      { question: "Nennen Sie die vier Hauptbestandteile eines Anstrichstoffs!", answer: "-Bindemittel\n-Additive\n-Pigmente\n-Lösungsmittel" },
      { question: "Nenne 3 geometrische Perspektiven!", answer: "-Froschperspektive\n-Vogelperspektive\n-Axonomischeperspektive\n-Kavalierperspektive" },
      { question: "Nenne vier Klebstoffsysteme und deren Anwendungsbereiche bei der Acrylverarbeitung", answer: "-Methylmethacrylat (MMA) Klebstoff\n-Cyancrylat (CA) Klebstoff\n-Epoxidharz Klebstoff\n-Polyurethan (PUR) Klebstoff" },
      { question: "Beschreiben Sie den Poliervorgang klarer Acrylglaskanten!", answer: "Die Acrylglaskante wird nacheinander mit verschieden starken Schleifpapieren geschliffen, dann wird die kannte einmal mit einem Tuch gesäubert und mit Wachs beschichtet, der Wachs dient als poliermittel die kannte setzt man gleichmäßig an einen befestigten polierkopf an einem Bohrer etc. an" },
      { 
        question: "Ein Großformatdrucker ist in einem Jahr an 258 Arbeitstagen durchschnittlich 8 Stunden eingeschaltet. In der Standby-Phase hat der Drucker eine Leistungsaufnahme von 200 W, während des Druckens eine Leistungsaufnahme von 850 Watt. 60 % der Einschaltzeit werden für Ausdrucke genutzt. Der Strom-Arbeitspreis beträgt 0,15 Euro/kWh, der Strom-Grundpreis 58,40 Euro/Monat. Berechnen Sie die jährlichen Stromkosten in Euro! Geben Sie dazu Formel, Rechenweg und Einheiten an und runden Sie das Endergebnis kaufmännisch auf 2 Stellen hinter dem Komma!", 
        answer: `Berechnung der jährlichen Stromkosten:
- Betriebsstunden pro Jahr = 258 Tage * 8 Std = 2064 Std
- Druckbetrieb: 60 % von 2064 Std = 1238,4 Std
- Standby-Betrieb: 40 % von 2064 Std = 825,6 Std
- Energieverbrauch Druckbetrieb = 1238,4 Std * 0,85 kW = 1052,64 kWh
- Energieverbrauch Standby = 825,6 Std * 0,2 kW = 165,12 kWh
- Gesamter Energieverbrauch = 1052,64 + 165,12 = 1217,76 kWh
- Stromkosten Arbeit = 1217,76 kWh * 0,15 €/kWh = 182,66 €
- Stromkosten Grundpreis = 58,40 € * 12 Monate = 700,80 €
- Gesamtkosten = 182,66 € + 700,80 € = 883,46 €
Endergebnis: 883,46 €`
      },
      { question: "Nenne drei Vorteile von LED-Beleuchtung gegenüber herkömmlichen Glühlampen.", answer: "Längere Lebensdauer, geringer Stromverbrauch, weniger Wärmeentwicklung" },
      { question: "Wie lautet die physikalische Einheit der elektrischen Leistung?", answer: "Watt (W)" },
      { question: "Was versteht man unter dem Begriff ‚Komplementärfarben‘?", answer: "Farben, die sich im Farbkreis gegenüberliegen und zusammen Weiß ergeben" },
      { question: "Nenne zwei Maßnahmen zur Erhöhung der Sicherheit bei elektrischen Anlagen.", answer: "Fehlerschutzschalter installieren, Verwendung geprüfter Komponenten" },
      { question: "Welche Hauptbestandteile enthält ein Lack?", answer: "Bindemittel, Pigmente, Lösungsmittel, Additive" }
    ];

    let currentIndex = 0;

    function toggleMenu() {
      const list = document.getElementById('questionList');
      if (list.style.display === 'block') {
        list.style.display = 'none';
      } else {
        populateQuestionList();
        list.style.display = 'block';
      }
    }

    function populateQuestionList() {
      const list = document.getElementById('questionList');
      list.innerHTML = '';
      const ul = document.createElement('ul');
      questions.forEach((q, i) => {
        const li = document.createElement('li');
        li.textContent = `Frage ${i + 1}`;
        li.onclick = () => {
          currentIndex = i;
          showQuestion();
          document.getElementById('questionList').style.display = 'none';
          document.getElementById('feedback').textContent = '';
          document.getElementById('answer').value = '';
        };
        ul.appendChild(li);
      });
      list.appendChild(ul);
    }

    function showQuestion() {
      const q = questions[currentIndex];
      document.getElementById('question').textContent = q.question;
      document.getElementById('answer').value = '';
      document.getElementById('feedback').textContent = '';
    }

    function checkAnswer() {
      const userAnswer = document.getElementById('answer').value.trim().toLowerCase();
      const correctAnswer = questions[currentIndex].answer.trim().toLowerCase();

      // Für längere Antworten (z.B. Rechenweg) prüfen wir nur, ob die Antwort Teilstring ist
      if (correctAnswer.length > 50) {
        if (correctAnswer.includes(userAnswer) || userAnswer.includes(correctAnswer)) {
          document.getElementById('feedback').textContent = 'Richtig!';
        } else {
          document.getElementById('feedback').textContent = 'Leider falsch. Richtige Antwort:\n' + questions[currentIndex].answer;
        }
      } else {
        if (userAnswer === correctAnswer) {
          document.getElementById('feedback').textContent = 'Richtig!';
        } else {
          document.getElementById('feedback').textContent = 'Leider falsch. Richtige Antwort: ' + questions[currentIndex].answer;
        }
      }
    }

    function nextQuestion() {
      currentIndex = (currentIndex + 1) % questions.length;
      showQuestion();
    }

    function speakQuestion() {
      const msg = new SpeechSynthesisUtterance();
      msg.text = questions[currentIndex].question;
      msg.lang = 'de-DE';
      window.speechSynthesis.speak(msg);
    }

    // Seite lädt erste Frage automatisch
    nextQuestion();
  </script>
</body>
</html>
