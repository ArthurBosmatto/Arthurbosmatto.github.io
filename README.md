<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Loja MONSTER FISH</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      margin: 0;
      background-image: url('https://www.clarin.com/2019/10/17/EDAxYXgZ_1200x0__1.jpg');
      background-size: cover;
      background-attachment: fixed;
      background-position: center;
      color: #000000;
    }
    header {
      background-color: rgba(0, 0, 0, 0.85);
      color: white;
      padding: 20px;
      text-align: center;
      position: relative;
    }
    nav {
      background-color: rgba(0, 0, 0, 0.85);
      padding: 10px;
      text-align: center;
    }
    nav a {
      color: white;
      margin: 0 15px;
      text-decoration: none;
      font-weight: bold;
    }
    section {
      padding: 20px;
      background-color: rgba(200, 200, 200, 0.85);
      margin: 10px;
      border-radius: 8px;
    }
    h2 {
      color: #000000;
    }
    .promo, .produtos {
      display: flex;
      gap: 20px;
      flex-wrap: wrap;
    }
    .card {
      background-color: #dddddd;
      padding: 15px;
      border-radius: 10px;
      box-shadow: 0 2px 5px rgba(0,0,0,0.1);
      width: 200px;
      text-align: center;
      color: black;
      cursor: pointer;
    }
    .card img {
      width: 100%;
      border-radius: 8px;
      margin-bottom: 10px;
    }
    footer {
      background-color: rgba(0, 0, 0, 0.85);
      color: white;
      text-align: center;
      padding: 20px;
      margin-top: 20px;
    }
    .footer-links {
      margin-top: 10px;
    }
    .footer-links a {
      color: #e0f2f1;
      margin: 0 10px;
      text-decoration: none;
      font-size: 0.9em;
    }
    #cart {
      background-color: #fff;
      border: 1px solid #ccc;
      border-radius: 10px;
      padding: 10px;
      width: 300px;
      box-shadow: 0 2px 5px rgba(0,0,0,0.3);
      margin-top: 10px;
    }
    #cart h3 {
      margin-top: 0;
    }
    #cart-items {
      list-style: none;
      padding: 0;
      max-height: 200px;
      overflow-y: auto;
    }
    #cart-items li {
      margin-bottom: 5px;
      display: flex;
      justify-content: space-between;
      align-items: center;
      color: black;
    }
    #cart-items li span {
      color: black;
    }
    #total {
      font-weight: bold;
      margin-top: 10px;
    }
    .remove-btn {
      margin-left: 10px;
      color: red;
      cursor: pointer;
      font-weight: bold;
    }
    .auth-buttons {
      position: absolute;
      top: 20px;
      right: 20px;
      display: flex;
      flex-direction: column;
      gap: 10px;
    }
    .auth-and-cart {
      position: absolute;
      top: 20px;
      right: 20px;
      display: flex;
      flex-direction: column;
      align-items: flex-start;
    }
  </style>
</head>
<body>

  <header>
    <h1>MONSTER FISH</h1>
    <p>Sua loja de aquarismo JUMBO</p>
  </header>

  <div class="auth-and-cart">
    <div class="auth-buttons">
      <button onclick="window.location.href='#login'" style="margin-right: 10px;">Login</button>
      <button onclick="window.location.href='#cadastro'">Cadastro</button>
    </div>

    <div id="cart">
      <h3>🛒 Carrinho</h3>
      <ul id="cart-items"></ul>
      <div id="total">Total: R$ 0,00</div>
    </div>
  </div>

  <nav>
    <a href="#promocoes">Promoções</a>
    <a href="#historia">Nossa História</a>
    <a href="#produtos">Produtos</a>
  </nav>

  <section id="promocoes">
  <div id="user-greeting" style="font-weight: bold; font-size: 18px; margin-bottom: 10px; color: #004d40;"></div>
    <h2>RIVER MONSTERS</h2>
    <div class="promo">
      <div class="card" data-price="79.90">
        <div class="selo">RIVER MONSTERS</div>
        <img src="https://t4.ftcdn.net/jpg/03/55/75/85/360_F_355758577_jaUhim6zMHrty6vpFsG9Wj7v8Y40IUVs.jpg" alt="Aimara">
        <h3>AIMARA</h3>
        <p>De R$ 99,90 por R$ 79,90!</p>
      </div>
      <div class="card" data-price="2999.00">
        <img src="https://www.fishi-pedia.com/wp-content/uploads/2013/10/Potamotrygon_leopoldi_2.jpg" alt="Arraia Leopoldi">
        <h3>ARRAIA</h3>
        <p>Majestosa e venenosa!</p>
      </div>
      <div class="card" data-price="499.90">
        <img src="https://http2.mlstatic.com/D_NQ_NP_791690-MLB41722615749_052020-O-aruana-prata-peixe-importado-jumbo-aquario-lago-ornamental.webp" alt="Aruanã">
        <h3>ARUANÃ</h3>
        <p>Peixe saltador com escamas metálicas.</p>
      </div>
      <div class="card" data-price="499.90">
        <img src="https://s2.glbimg.com/9q14WeiMDMQ8IfJGaX6N6HmLBvA=/1200x630/s.glbimg.com/jo/g1/f/original/2015/01/15/255.jpg" alt="Peixe Cachorra">
        <h3>PEIXE CACHORRA</h3>
        <p>Mordida poderosa e visual único.</p>
      </div>
      <div class="card" data-price="39.90">
        <img src="https://pisciculturabrumado.com.br/wp-content/uploads/2020/12/Jundia-rosa.jpg" alt="Jundiá">
        <h3>JUNDIÁ</h3>
        <p>Comportamento calmo e aparência elegante.</p>
      </div>
      <div class="card" data-price="59.90">
        <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcR-vNXXaQnQaCm7cuAJPrHL4imfzUMCNkcAWA&s" alt="Oscar">
        <h3>OSCAR</h3>
        <p>Peixe amazônico e companheiro!</p>
      </div>
      <div class="card" data-price="29.90">
        <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTFnVwr4rrmyPH4__V_nt5EpRSPZlTEzpjapw&s" alt="Pacu">
        <h3>PACU</h3>
        <p>Onívoro e pacífico, ótimo para comunitários.</p>
      </div>
      <div class="card destaque" data-price="199.90">
        <div class="selo">RIVER MONSTERS</div>
        <img src="https://st2.depositphotos.com/1011158/8802/i/450/depositphotos_88023162-stock-photo-arapaima-one-of-the-biggest.jpg" alt="Pirarucu">
        <h3>PIRARUCU</h3>
        <p>De R$ 399,90 por R$ 199,90!</p>
      </div>
      <div class="card destaque" data-price="99.90">
        <div class="selo">RIVER MONSTERS</div>
        <img src="https://cdn.interago.com.br/img/png/w_0_q_8/5/mc/Novo%20cat%C3%A1logo/Pirarara/pirararafundo2" alt="Pirarara">
        <h3>PIRARARA</h3>
        <p>De R$ 199,90 por R$ 99,90!</p>
      </div>
      <div class="card" data-price="129.90">
        <img src="https://aquaponia-urbana.com/wp-content/uploads/2023/09/Peixe-Pintado-tem-Espinho.jpg" alt="Surubim">
        <h3>SURUBIM</h3>
        <p>Forte e resistente, ideal para tanques grandes.</p>
      </div>
      <div class="card" data-price="119.50">
        <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRd_mvOfUcN5ANHdM544lkdJ441XnUhvHaPpg&s" alt="Tucunaré Amarelo">
        <h3>TUCUNARÉ AMARELO</h3>
        <p>Predador voraz e muito elegante.</p>
      </div>
      <div class="card" data-price="89.90">
        <img src="https://cptstatic.s3.amazonaws.com/imagens/enviadas/materias/materia6196/pacu-e-tambaqui-tipos-de-racao-cpt.jpg" alt="Tambaqui">
        <h3>TAMBAQUI</h3>
        <p>Espécie amazônica robusta e bonita.</p>
      </div>
    </div>
</section>

  <section id="historia">
    <h2>📜 Nossa História</h2>
    <p>
      Fundada em 2010, a <strong>MONSTER FISH</strong> nasceu da paixão por peixes jumbos e tank busters.
      Com anos de experiência, oferecemos produtos de qualidade e peixes de altíssimo padrão para todo Brasil.
    </p>
  </section>

  <section id="produtos">
    <h2>🐠 Produtos</h2>
    <div class="produtos">
      <div class="card" data-price="49.90">
        <img src="https://http2.mlstatic.com/D_NQ_NP_776857-MLB48466712884_122021-O.webp" alt="Rede de Captura">
        <h3>Rede de Captura</h3>
        <p>Ideal para manuseio seguro de peixes grandes.</p>
      </div>
      <div class="card" data-price="120.00">
        <img src="https://images.tcdn.com.br/img/img_prod/749804/filtro_externo_hf_800_ocean_tech_220v_917_1_20201211001328.png" alt="Filtros">
        <h3>Filtros</h3>
        <p>Modelos internos, externos e canisters.</p>
      </div>
      <div class="card" data-price="85.00">
        <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcS05QIyiWJ_3EN3heoAcoboFhmkQ5lK9g6uMQ&s" alt="Iluminação LED">
        <h3>Iluminação LED</h3>
        <p>Ideal para aquários plantados.</p>
      </div>
      <div class="card" data-price="69.90">
        <img src="https://images.petz.com.br/fotos/1466108687847.jpg" alt="Termostatos">
        <h3>Termostatos</h3>
        <p>Controle preciso da temperatura.</p>
      </div>
      <div class="card" data-price="79.90">
        <img src="https://poytara.com/adm-produtos/uploads/resized_11604e487057a62_1615743088_360x.webp" alt="Ração Premium">
        <h3>Ração Premium</h3>
        <p>Nutrição ideal para peixes de grande porte.</p>
      </div>
      <div class="card" data-price="19.90">
        <img src="https://down-br.img.susercontent.com/file/aefa9f026733ae5ab3a0b9b4d2ffbc44" alt="Redutor de Amônia">
        <h3>Redutor de Amônia</h3>
        <p>Melhore a qualidade da água.</p>
      </div>
      <div class="card" data-price="99.90">
        <img src="https://cobasi.vteximg.com.br/arquivos/ids/833655/6955974905636_edt.jpg?v=637683446331430000" alt="Bomba de Circulação">
        <h3>Bomba de Circulação</h3>
        <p>Oxigenação eficiente para grandes aquários.</p>
      </div>
      <div class="card" data-price="29.90">
        <img src="https://http2.mlstatic.com/D_NQ_NP_790178-MLB47976473123_102021-O-alcon-labcon-protect-plus-30ml-anticloro-para-aquario.webp" alt="Condicionador de Água">
        <h3>Condicionador de Água</h3>
        <p>Remove cloro e metais pesados.</p>
      </div>
      <div class="card" data-price="29.90">
        <img src="https://cdn.awsli.com.br/800x800/1751/1751460/produto/1315446035c663c68f0.jpg" alt="Teste de Parâmetros">
        <h3>Teste de Parâmetros</h3>
        <p>Verifique pH, amônia, nitrito e nitrato.</p>
      </div>
      <div class="card" data-price="39.90">
        <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcR2XT8yOeC46HbkH460V_fcgakRuZlBvKws7w&s" alt="Substrato Areia">
        <h3>Substrato Areia</h3>
        <p>Ideal para peixes de fundo e estética natural.</p>
      </div>
      <div class="card" data-price="89.90">
        <img src="https://www.tropizoo.com/loja/img/p/4/4/3/4/4434-tm_thickbox_default.jpg" alt="Tampa de Aquário">
        <h3>Tampa de Aquário</h3>
        <p>Evite saltos e evaporação da água.</p>
      </div>
      <div class="card" data-price="119.90">
        <img src="https://http2.mlstatic.com/D_NQ_NP_753519-MLB78303809520_082024-O-controlador-de-temperatura-z31e-p-aquario-marinho-bivolt.webp" alt="Aquecedor Digital">
        <h3>Aquecedor Digital</h3>
        <p>Alta precisão e segurança térmica.</p>
      </div>
    </div>
  </section>

  <footer>
    <p>&copy; 2025 MONSTER FISH - Todos os direitos reservados.</p>
    <div class="footer-links">
      <a href="#">Termos de Uso</a>
      <a href="#">Política de Privacidade</a>
      <a href="#">Contato</a>
    </div>
  </footer>

  <section id="login" style="padding: 20px; background-color: #ffffffcc; border-radius: 10px; max-width: 400px; margin: 40px auto;">
    <h2>Login</h2>
    <form onsubmit="loginUser(event)">
      <label>Email:</label><br>
      <input type="email" id="loginEmail" required style="width: 100%; margin-bottom: 10px;"><br>
      <label>Senha:</label><br>
      <input type="password" id="loginSenha" required style="width: 100%; margin-bottom: 10px;"><br>
      <button type="submit">Entrar</button>
    </form>
  </section>

  <section id="cadastro" style="padding: 20px; background-color: #ffffffcc; border-radius: 10px; max-width: 400px; margin: 40px auto;">
    <h2>Cadastro</h2>
    <form onsubmit="registerUser(event)">
      <label>Nome:</label><br>
      <input type="text" id="cadastroNome" required style="width: 100%; margin-bottom: 10px;"><br>
      <label>Email:</label><br>
      <input type="email" id="cadastroEmail" required style="width: 100%; margin-bottom: 10px;"><br>
      <label>Senha:</label><br>
      <input type="password" id="cadastroSenha" required style="width: 100%; margin-bottom: 10px;"><br>
      <button type="submit">Cadastrar</button>
    </form>
  </section>

  <script>
    const cartItems = document.getElementById('cart-items');
    const totalElement = document.getElementById('total');
    let total = 0;

    function updateTotal() {
      totalElement.textContent = `Total: R$ ${total.toFixed(2)}`;
    }

    function addToCart(productName, price) {
      const li = document.createElement('li');
      const itemText = document.createElement('span');
      itemText.textContent = `${productName} - R$ ${price.toFixed(2)}`;
      
      const removeBtn = document.createElement('span');
      removeBtn.className = 'remove-btn';
      removeBtn.textContent = '×';
      removeBtn.onclick = () => removeItem(removeBtn, price);

      li.appendChild(itemText);
      li.appendChild(removeBtn);
      cartItems.appendChild(li);

      total += price;
      updateTotal();
    }

    function removeItem(element, price) {
      element.parentElement.remove();
      total -= price;
      updateTotal();
    }

    document.querySelectorAll('.card').forEach(card => {
      card.addEventListener('click', () => {
        const name = card.querySelector('h3').textContent;
        const price = parseFloat(card.getAttribute('data-price')) || 0;
        addToCart(name, price);
      });
    });
  
    function loginUser(event) {
      event.preventDefault();
      const email = document.getElementById('loginEmail').value;
      const senha = document.getElementById('loginSenha').value;
      const stored = localStorage.getItem(email);
      if (stored && JSON.parse(stored).senha === senha) {
        alert('Login bem-sucedido!');
      } else {
        alert('Email ou senha incorretos.');
      }
    }

    function registerUser(event) {
      event.preventDefault();
      const nome = document.getElementById('cadastroNome').value;
      const email = document.getElementById('cadastroEmail').value;
      const senha = document.getElementById('cadastroSenha').value;
      localStorage.setItem(email, JSON.stringify({ nome, senha }));
      alert('Cadastro realizado com sucesso!');
    }
  
    let currentUser = null;

    function loginUser(event) {
      event.preventDefault();
      const email = document.getElementById('loginEmail').value;
      const senha = document.getElementById('loginSenha').value;
      const stored = localStorage.getItem(email);
      if (stored && JSON.parse(stored).senha === senha) {
        currentUser = JSON.parse(stored).nome;
        alert(`Bem-vindo, ${currentUser}!`);
        document.querySelector('#login').style.display = 'none';
        document.querySelector('#cadastro').style.display = 'none';
        document.querySelector('.auth-buttons').innerHTML = `<span style='color: white;'>Olá, ${currentUser}</span>`;
      } else {
        alert('Email ou senha incorretos.');
      }
    }

    function registerUser(event) {
      event.preventDefault();
      const nome = document.getElementById('cadastroNome').value;
      const email = document.getElementById('cadastroEmail').value;
      const senha = document.getElementById('cadastroSenha').value;
      localStorage.setItem(email, JSON.stringify({ nome, senha }));
      alert('Cadastro realizado com sucesso!');
      document.querySelector('#cadastro').style.display = 'none';
    }
  
    // Verifica usuário logado ao carregar
    window.onload = function () {
      const userGreeting = document.getElementById('user-greeting');
      const usuarioAtual = localStorage.getItem('usuarioAtual');
      if (usuarioAtual) {
        if (userGreeting) userGreeting.textContent = `Você está logado como ${JSON.parse(usuarioAtual).nome}`;
        const nome = JSON.parse(usuarioAtual).nome;
        document.querySelector('#login').style.display = 'none';
        document.querySelector('#cadastro').style.display = 'none';
        document.querySelector('.auth-buttons').innerHTML = `
          <span style='color: white;'>Olá, ${nome}</span>
          <button onclick="logoutUser()">Sair</button>
        `;
      }
    };

    function logoutUser() {
      localStorage.removeItem('usuarioAtual');
      location.reload();
    }

    function loginUser(event) {
      event.preventDefault();
      const email = document.getElementById('loginEmail').value;
      const senha = document.getElementById('loginSenha').value;
      const stored = localStorage.getItem(email);
      if (stored && JSON.parse(stored).senha === senha) {
        const usuario = JSON.parse(stored);
        localStorage.setItem('usuarioAtual', JSON.stringify(usuario));
        alert(`Bem-vindo, ${usuario.nome}!`);
        window.location.hash = '#promocoes';
        document.querySelector('#login').style.display = 'none';
        document.querySelector('#cadastro').style.display = 'none';
        document.querySelector('.auth-buttons').innerHTML = `
          <span style='color: white;'>Olá, ${usuario.nome}</span>
          <button onclick="logoutUser()">Sair</button>
        `;
      } else {
        alert('Email ou senha incorretos.');
      }
    }

    function registerUser(event) {
      event.preventDefault();
      const nome = document.getElementById('cadastroNome').value;
      const email = document.getElementById('cadastroEmail').value;
      const senha = document.getElementById('cadastroSenha').value;
      const usuario = { nome, senha };
      localStorage.setItem(email, JSON.stringify(usuario));
      localStorage.setItem('usuarioAtual', JSON.stringify(usuario));
      alert('Cadastro realizado com sucesso!');
      document.querySelector('#cadastro').style.display = 'none';
      document.querySelector('#login').style.display = 'none';
      document.querySelector('.auth-buttons').innerHTML = `
        <span style='color: white;'>Olá, ${nome}</span>
        <button onclick="logoutUser()">Sair</button>
      `;
    }
  </script>

</body>
</html>
