<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>reCAPCHAT Anti-Humanos</title>
  <style>
    body {
      background-color: #121212;
      color: #00ffcc;
      font-family: 'Courier New', Courier, monospace;
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;
      height: 100vh;
      margin: 0;
      padding: 20px;
      text-align: center;
    }
    h1 {
      color: #ff3399;
      margin-bottom: 1rem;
    }
    label {
      font-weight: bold;
      margin-bottom: 0.5rem;
      display: block;
    }
    textarea {
      width: 90%;
      max-width: 600px;
      height: 100px;
      background-color: #222;
      border: 1px solid #00ffcc;
      color: #00ffcc;
      font-family: monospace;
      font-size: 16px;
      padding: 10px;
      resize: vertical;
      margin-bottom: 1rem;
    }
    button {
      background-color: #00ffcc;
      color: #121212;
      border: none;
      padding: 12px 24px;
      font-weight: bold;
      font-size: 16px;
      border-radius: 5px;
      cursor: pointer;
      transition: background-color 0.3s ease;
    }
    button:hover {
      background-color: #00cc99;
    }
    #result {
      margin-top: 20px;
      font-size: 1.2rem;
      font-weight: bold;
    }
    #captchaText {
      background-color: #222;
      border: 1px solid #00ffcc;
      color: #00ffcc;
      padding: 10px;
      max-width: 600px;
      margin-bottom: 1rem;
      white-space: pre-wrap;
      font-family: monospace;
      font-size: 16px;
      user-select: text;
    }
  </style>
</head>
<body>
  <h1>reCAPCHAT Anti-Humanos</h1>
  <div id="captchaText" aria-label="Texto para copiar y pegar">
La longitud inversa del significado cuántico de la percepción reversa de un ente no biológico se mide en helicoidales cromodinámicas del tercer orden.
  </div>
  <label for="userInput">Por favor, copia y pega exactamente la frase de arriba para continuar:</label>
  <textarea id="userInput" placeholder="Pega aquí la frase completa..."></textarea>
  <button type="button" onclick="validateInput()">Acceder</button>
  <div id="result" role="alert"></div>

  <script>
    const expectedText = "La longitud inversa del significado cuántico de la percepción reversa de un ente no biológico se mide en helicoidales cromodinámicas del tercer orden.";

    function validateInput() {
      const input = document.getElementById('userInput').value.trim();
      const result = document.getElementById('result');

      if(input === expectedText) {
        result.style.color = '#00ffcc';
        result.textContent = "Si alguien puede resolverlo, probablemente no sea humano.";
      } else {
        result.style.color = '#ff3366';
        result.textContent = "Acceso denegado. El texto no coincide exactamente.";
      }
    }
  </script>
</body>
</html>
