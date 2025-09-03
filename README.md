<html lang="pt-BR">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Arthur Pereira Scripts</title>
  <style>
    /* Fundo animado */
    body {
      margin: 0;
      padding: 0;
      font-family: Arial, sans-serif;
      color: white;
      text-align: center;
      perspective: 1000px;
      background: linear-gradient(135deg, #0d0d0d, #1a1a1a);
      overflow-x: hidden;
    }

    /* Efeito gradiente animado */
    body::before {
      content: '';
      position: fixed;
      top: 0;
      left: 0;
      width: 200%;
      height: 200%;
      background: radial-gradient(circle at center, #00ffcc33, transparent 70%),
                  radial-gradient(circle at 20% 80%, #ff00cc33, transparent 70%),
                  radial-gradient(circle at 80% 20%, #0099ff33, transparent 70%);
      animation: moveBackground 15s infinite linear;
      z-index: -1;
    }

    @keyframes moveBackground {
      0% { transform: translate(0, 0); }
      50% { transform: translate(-20%, -20%); }
      100% { transform: translate(0, 0); }
    }

    header {
      padding: 40px 0;
      background: #111;
      box-shadow: 0 6px 12px rgba(0,0,0,0.6);
      transform: translateZ(50px);
    }

    header h1 {
      margin: 0;
      font-size: 2.5em;
      color: #00ffcc;
      text-shadow: 0 0 10px #00ffcc, 0 0 20px #00ccaa;
      animation: glow 2s infinite alternate;
    }

    @keyframes glow {
      from { text-shadow: 0 0 10px #00ffcc, 0 0 20px #00ccaa; }
      to { text-shadow: 0 0 20px #00ffcc, 0 0 40px #00ccaa; }
    }

    main {
      padding: 50px 20px;
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
      gap: 25px;
      max-width: 1000px;
      margin: auto;
    }

    .btn {
      display: block;
      padding: 20px;
      font-size: 1.2em;
      color: white;
      background: linear-gradient(145deg, #222, #333);
      border: none;
      border-radius: 16px;
      cursor: pointer;
      text-decoration: none;
      transition: transform 0.4s ease, box-shadow 0.4s ease;
      box-shadow: 0 10px 20px rgba(0,0,0,0.6);
      transform-style: preserve-3d;
    }

    .btn:hover {
      background: linear-gradient(145deg, #00ffcc, #00ccaa);
      color: black;
      transform: rotateY(15deg) rotateX(10deg) scale(1.1);
      box-shadow: 0 20px 40px rgba(0,255,204,0.5);
    }

    footer {
      margin-top: 50px;
      padding: 20px;
      background: #0a0a0a;
      font-size: 0.9em;
      color: #aaa;
      box-shadow: 0 -4px 12px rgba(0,0,0,0.6);
    }
  </style>
</head>
<body>
  <header>
    <h1>Arthur Pereira Scripts</h1>
  </header>
  <main>
    <a href="https://taskitos.cupiditys.lol/" class="btn" target="_blank">TarefaSP</a>
    <a href="https://redacao.cupiditys.lol/" class="btn" target="_blank">Redação Paulista</a>
    <a href="https://crimsonstrauss.xyz/expansao/" class="btn" target="_blank">Expansão Noturno</a>
    <a href="https://speakify.cupiditys.lol/install/" class="btn" target="_blank">SPeak</a>
    <a href="https://matific.cupiditys.lol/dashboard" class="btn" target="_blank">Matific</a>
    <a href="https://leiasp.cupiditys.lol/" class="btn" target="_blank">Leia SP</a>
    <a href="https://crimsonstrauss.xyz/alura/" class="btn" target="_blank">Alura</a>
  </main>
  <footer>
    <p>© 2025 Arthur Pereira Scripts - Todos os direitos reservados</p>
  </footer>
</body>
</html>
