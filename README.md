arcanum-silente/
├──index.html 
<DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Arcanum Silente</title>
  <style>
    body {
      background: black;
      color: #ccc;
      font-family: serif;
      margin: 0;
      padding: 0;
    }
    header {
      background: #1c1c1c;
      padding: 2rem;
      text-align: center;
    }
    header h1 {
      margin: 0;
      color: #e11d48;
    }
    main {
      padding: 2rem;
    }
    section {
      margin-bottom: 3rem;
    }
    h2 {
      color: #f43f5e;
    }
    .note, .latin, blockquote {
      background: #1f2937;
      padding: 1rem;
      border-left: 4px solid #e11d48;
      margin-top: 1rem;
      border-radius: 6px;
    }
    blockquote {
      color: #fca5a5;
      font-style: italic;
    }
    .button {
      display: inline-block;
      margin-top: 20px;
      padding: 10px 20px;
      background: #7f1d1d;
      color: white;
      text-decoration: none;
      border-radius: 8px;
    }
    .button:hover {
      background: #991b1b;
    }
    .alerta {
      text-align: center;
      margin-top: 3rem;
      font-size: 1.2rem;
      color: red;
    }
    footer {
      background: #111;
      text-align: center;
      padding: 1rem;
      font-size: 0.9rem;
      color: #666;
    }
  </style>
</head>
<body>
  <header>
    <h1>ARQUIVOS DE ORVAX</h1>
    <p><em>“Ex umbra in veritatem.”</em></p>
  </header>

  <main>
    <section>
      <p>As transcrições abaixo foram recuperadas das ruínas de <strong>Kaersalt</strong>, onde acredita-se que os primeiros registros da Ordem foram selados sob o nome-código <em>Orvax</em>.</p>
      <blockquote>
        "Ele não é apenas memória... é o eco de todos os gritos que se recusaram a morrer."
        <div style="text-align:right; font-size: small; color: gray;">— Manuscrito II, fragmento carbonizado</div>
      </blockquote>
      <p>Entre os registros, destaca-se um ser conhecido como <strong>Lamentos</strong>, cuja forma espectral carrega rastros de dois ancestrais: <span style="text-decoration: underline dotted;">um ancião chamado D.</span> e o que os textos chamam de <span style="text-decoration: underline dotted;">a fraqueza viva da B.</span></p>
      <p>Não se deve esquecer o primeiro espreitador, aquele que <em>vê mesmo quando não há olhos</em>.</p>
      <div class="note">
        ⚠ Acesso restrito: algumas partes contêm texto cifrado. Decifre as instruções com base em <code>Silenti Vox 3:17</code>.
      </div>
    </section>

    <section>
      <h2>Fragmento em Latim</h2>
      <p class="latin">“Sanguis unus, vita altera. Ubi umbra, ibi vestigium.”</p>
      <p style="font-size: small; color: gray;"><em>Apenas uma gota resta, e ela não está onde dizem que está.</em></p>
      <div style="text-align:center;">
        <a href="orvax/blood.html" class="button">Acessar a gota de sangue</a>
        <p style="font-size: small; color: gray;">Senha necessária. Pista oculta na página principal, linha 13 do códice.</p>
      </div>
    </section>

    <section>
      <h2>Registros de Membros</h2>
      <ul>
        <li>Pedro</li><li>Arthur</li><li>Douglas</li><li>Samantha</li><li>Leon</li><li>Fernanda</li><li>Rayka</li><li>Guilherme</li><li>Caterina</li><li>Lyri</li><li>Eric</li><li>Edward</li><li>Hana</li>
      </ul>
      <p style="font-size: small; color: gray;">Alguns nomes foram omitidos por questões de segurança. O primeiro espreitador observa em silêncio.</p>
    </section>

    <section>
      <h2>Textos Apócrifos</h2>
      <div class="note">"Quando o sangue sussurra, nem mesmo as cinzas podem dormir."</div>
      <div class="note">"O eco de D. ainda vive sob as garras de L., que caminha entre a carne e a lembrança."</div>
      <div class="note">"Ela se debruça sobre os nomes riscados, e por entre eles, o que nunca foi dito permanece ativo."</div>
    </section>

    <div class="alerta" id="bloqueio"></div>
  </main>

  <footer>
    &copy; Arcanum Silente. Criado por 01.
  </footer>

  <script>
    document.addEventListener("DOMContentLoaded", () => {
      const senha = prompt("Tem certeza da escolha? Digite a senha:");
      if (senha !== "silente") {
        document.getElementById("bloqueio").innerText = "🔒 Acesso negado.";
        document.querySelector("main").style.display = "none";
      }
    });
  </script>
</body>
</html>
└── orvax/
    └── blood.html      ← subpágina protegida


