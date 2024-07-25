<h1>Projeto de Autenticação Laravel</h1>

<p>Este é um projeto básico de autenticação utilizando Laravel e JWT. Ele inclui funcionalidades para login, registro, logout e atualização de token.</p>

<h2>Requisitos</h2>
<ul>
  <li>PHP >= 7.4</li>
  <li>Composer</li>
  <li>Laravel 8.x</li>
  <li>MySQL ou qualquer outro banco de dados suportado pelo Laravel</li>
</ul>

<h2>Instalação</h2>
<ol>
  <li>Clone o repositório para o seu ambiente local:
    <pre class="command">git clone https://github.com/titocrf/api-rest-teste.git</pre>
  </li>
  <li>Instale as dependências do projeto usando o Composer:
    <pre class="command">composer install</pre>
  </li>
  <li>Copie o arquivo <code>.env.example</code> para <code>.env</code>:
    <pre class="command">cp .env.example .env</pre>
  </li>
  <li>Gere a chave da aplicação:
    <pre class="command">php artisan key:generate</pre>
  </li>
  <li>Configure as informações de conexão do banco de dados no arquivo <code>.env</code>:
    <pre class="command">DB_CONNECTION=mysql
DB_HOST=127.0.0.1
DB_PORT=3306
DB_DATABASE=nome_do_banco
DB_USERNAME=seu_usuario
DB_PASSWORD=sua_senha</pre>
  </li>
  <li>Execute as migrações para criar as tabelas no banco de dados:
    <pre class="command">php artisan migrate</pre>
  </li>
  <li>Instale o pacote JWT para Laravel:
    <pre class="command">composer require tymon/jwt-auth</pre>
  </li>
  <li>Publique a configuração do JWT:
    <pre class="command">php artisan vendor:publish --provider="Tymon\JWTAuth\Providers\LaravelServiceProvider"</pre>
  </li>
  <li>Gere a chave secreta do JWT:
    <pre class="command">php artisan jwt:secret</pre>
  </li>
</ol>

<h2>Uso</h2>

<h3>Servidor de Desenvolvimento</h3>
<p>Para iniciar o servidor de desenvolvimento, execute:</p>
<pre class="command">php artisan serve</pre>
<p>O servidor estará disponível em <code>http://localhost:8000</code>.</p>

<h3>Documentação Swagger</h3>

<div class="endpoint">
  <p><strong>Para acessar a documentação basta acessar:</strong></p>
  <pre class="command">http://localhost:8000/api/documentation"</pre>
</div>


<h2>Licença</h2>
<p>Este projeto é licenciado sob a licença MIT. Veja o arquivo <a href="LICENSE">LICENSE</a> para mais detalhes.</p>

</body>
</html>
