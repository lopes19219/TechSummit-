<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>TechFuture Summit</title>
  <style>
    :root {
      --primary: #004aad;
      --secondary: #00c6a9;
      --background: #f4f4f4;
      --text: #333;
      --white: #fff;
    }

    body {
      font-family: Arial, sans-serif;
      background-color: var(--background);
      margin: 0;
      padding: 0;
      color: var(--text);
    }

    header {
      background-color: var(--primary);
      color: var(--white);
      padding: 2rem;
      text-align: center;
    }

    section {
      padding: 2rem;
      max-width: 1000px;
      margin: auto;
    }

    .palestrantes {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
      gap: 1rem;
    }

    .palestrante {
      background: var(--white);
      padding: 1rem;
      border-radius: 8px;
      box-shadow: 0 2px 5px rgba(0,0,0,0.1);
      text-align: center;
    }

    .palestrante img {
      width: 100px;
      height: 100px;
      border-radius: 50%;
      object-fit: cover;
      margin-bottom: 0.5rem;
    }

    form {
      background: var(--white);
      padding: 2rem;
      border-radius: 8px;
      box-shadow: 0 2px 8px rgba(0,0,0,0.1);
    }

    label {
      display: block;
      margin-top: 1rem;
    }

    input[type="text"],
    input[type="email"] {
      width: 100%;
      padding: 0.5rem;
      border: 1px solid #ccc;
      border-radius: 4px;
    }

    .radio-group, .checkbox-group {
      margin-top: 1rem;
    }

    button {
      background: var(--secondary);
      color: var(--white);
      padding: 0.75rem 1.5rem;
      border: none;
      border-radius: 4px;
      margin-top: 1rem;
      cursor: pointer;
      transition: background 0.3s ease;
    }

    button:hover {
      background: #009b85;
    }

    @media (max-width: 600px) {
      header h1 {
        font-size: 1.5rem;
      }
    }
  </style>
</head>
<body>
  <header>
    <h1>TechFuture Summit 2025</h1>
  </header>

  <section>
    <h2>Sobre o Evento</h2>
    <p>Data: 10 de Setembro de 2025<br>
    Local: São Paulo Expo, SP<br>
    O TechFuture Summit é o encontro de referência para desenvolvedores e designers discutirem as próximas tendências em tecnologia e design.</p>
  </section>

  <section>
    <h2>Palestrantes</h2>
    <div class="palestrantes">
      <div class="palestrante">
        <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTeO3sEHOBwn39BRmW01zxv8x-K7ClmjDdnY3szsXNQPIejfuolhZ36npBc&s=100" alt="João Silva">
        <h3>João Silva</h3>
        <p>Especialista em UX e professor de design digital.</p>
      </div>
      <div class="palestrante">
        <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcT-xDjiuyTlquDi5urpCUfQ4WrlC_uwJ_AMorjIeHdOJLEz7Jl_20jbnMf2&s=100" alt="Maria Oliveira">
        <h3>Maria Oliveira</h3>
        <p>Engenheira de Software da TechGlobal com foco em IA.</p>
      </div>
    </div>
  </section>

  <section>
    <h2>Inscreva-se</h2>
    <form>
      <label for="nome">Nome completo:</label>
      <input type="text" id="nome" name="nome" required>

      <label for="email">E-mail:</label>
      <input type="email" id="email" name="email" required>

      <div class="radio-group">
        <p>Tipo de ingresso:</p>
        <label><input type="radio" name="tipo" value="presencial" required> Presencial</label>
        <label><input type="radio" name="tipo" value="online"> Online</label>
      </div>

      <div class="checkbox-group">
        <label><input type="checkbox" required> Aceito os termos e condições</label>
      </div>

      <button type="submit">Enviar inscrição</button>
    </form>
  </section>
</body>
</html>
