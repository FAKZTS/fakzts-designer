<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Fakzts Designer</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      margin: 0;
      padding: 0;
      background: #f8f8f8;
      overflow-x: hidden;
    }
    header {
      background: #111;
      color: white;
      padding: 2rem;
      text-align: center;
      position: relative;
      overflow: hidden;
    }
    header h1 {
      margin: 0;
      font-size: 2.5rem;
      animation: slideInFromLeft 1s ease-out;
    }
    header p {
      margin: 0;
      font-size: 1.2rem;
      animation: slideInFromRight 1s ease-out;
    }
    section {
      padding: 2rem;
      opacity: 0;
      transform: translateY(20px);
      transition: opacity 0.6s ease-out, transform 0.6s ease-out;
    }
    .portfolio {
      display: flex;
      flex-wrap: wrap;
      justify-content: center;
    }
    .portfolio img {
      width: 100%;
      max-width: 300px;
      margin: 1rem;
      border-radius: 8px;
      transition: transform 0.3s ease;
    }
    .portfolio img:hover {
      transform: scale(1.05);
    }
    footer {
      background: #222;
      color: white;
      text-align: center;
      padding: 1rem;
    }
    @keyframes slideInFromLeft {
      from {
        transform: translateX(-100%);
      }
      to {
        transform: translateX(0);
      }
    }
    @keyframes slideInFromRight {
      from {
        transform: translateX(100%);
      }
      to {
        transform: translateX(0);
      }
    }
  </style>
</head>
<body>
  <header>
    <h1>Fakzts Designer</h1>
    <p>Criações visuais que impressionam</p>
  </header>

  <section id="sobre">
    <h2>Sobre</h2>
    <p>Sou um designer gráfico apaixonado por transformar ideias em arte visual impactante.</p>
  </section>

  <section id="portfolio" class="portfolio">
    <h2>Portfólio</h2>
    <p>Veja alguns dos meus trabalhos abaixo:</p>
    <img src="https://via.placeholder.com/300x200?text=Trabalho+1" alt="Trabalho 1" />
    <img src="https://via.placeholder.com/300x200?text=Trabalho+2" alt="Trabalho 2" />
    <img src="https://via.placeholder.com/300x200?text=Trabalho+3" alt="Trabalho 3" />
  </section>

  <section id="contato">
    <h2>Contato</h2>
    <p>WhatsApp: <a href="https://wa.me/5564992985478" target="_blank">(64) 99298-5478</a></p>
    <p>Instagram: <a href="https://www.instagram.com/fak_motion_designer" target="_blank">@fak_motion_designer</a></p>
  </section>

  <footer>
    <p>&copy; 2025 Fakzts Designer. Todos os direitos reservados.</p>
  </footer>

  <script>
    document.addEventListener("DOMContentLoaded", function() {
      const sections = document.querySelectorAll("section");
      sections.forEach(section => {
        section.style.opacity = 1;
        section.style.transform = "translateY(0)";
      });
    });
  </script>
</body>
</html>
