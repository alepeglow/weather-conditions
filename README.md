# weather-conditions

Este projeto é uma aplicação web que permite aos usuários pesquisar por cidades e visualizar informações sobre as condições climáticas atuais, como temperatura e um ícone representando o estado do tempo (ex: ensolarado, chuvoso, nublado, etc.). Os dados são obtidos em tempo real utilizando a API do [OpenWeatherMap](https://openweathermap.org/).

## Funcionalidades

- **Busca por cidades:** Insira o nome de uma cidade para obter informações sobre o clima.
- **Exibição de temperatura:** Mostra a temperatura atual na cidade pesquisada.
- **Ícone do clima:** Exibe um ícone visual que representa o estado atual do tempo.

## Tecnologias Utilizadas

- **HTML5:** Estrutura da aplicação.
- **CSS3:** Estilização e responsividade.
- **JavaScript:** Manipulação da DOM e integração com a API.
- **TypeScript:** Garantia de tipagem e maior segurança no código.

## Pré-requisitos

- Navegador atualizado (Google Chrome, Firefox, Edge, etc.).
- Conta no OpenWeatherMap para gerar uma API Key (gratuita).

## Como executar o projeto

1. **Clone o repositório:**
   ```bash
   git clone https://github.com/alepeglow/weather-conditions.git
   ```

2. **Acesse o diretório do projeto:**
   ```bash
   cd weather-conditions
   ```

3. **Configure a API Key:**
   - Crie um arquivo `config.js` na raiz do projeto e adicione a sua chave da API:
     ```javascript
     const API_KEY = 'SUA_API_KEY_AQUI';
     export default API_KEY;
     ```

4. **Abra o arquivo HTML em seu navegador:**
   - Simplesmente clique duas vezes no arquivo `index.html` ou use uma extensão como "Live Server" para executá-lo.

## Estrutura de Pastas

```
weather-conditions
<p>├── index.html        # Página principal</p>
<p>├── styles/style.css        # Arquivo de estilos</p>
<p>├── js/index.js            # Lógica em JavaScript</p>
<p>├── ts/index.ts            # Lógica em TypeScript</p>
<p>└── README.md         # Documentação do projeto</p>
```

## Integração com a API OpenWeatherMap

- A aplicação utiliza o endpoint `/weather` da API do OpenWeatherMap para buscar as condições climáticas.
- Documentação da API: [https://openweathermap.org/current](https://openweathermap.org/current)

Exemplo de requisição:
```javascript
fetch(`https://api.openweathermap.org/data/2.5/weather?q={CITY_NAME}&appid={API_KEY}&units=metric`)
  .then(response => response.json())
  .then(data => {
    console.log(data);
  });
```

## Melhorias Futuras

- **Previsão do tempo:** Exibir a previsão para os próximos dias.
- **Localização automática:** Detectar a localização do usuário e mostrar o clima atual automaticamente.
- **Suporte a múltiplos idiomas:** Permitir que a interface e os dados da API sejam apresentados em diferentes idiomas.
- **Interface Responsiva:** Permitir que seja responsivo em dispositivos móveis e desktops

## Contribuição

Contribuições são bem-vindas! Sinta-se à vontade para abrir issues ou enviar pull requests para melhorias e novas funcionalidades.


## Contato

Se tiver dúvidas ou sugestões, entre em contato:
- **Email:** peglowalessandra@gmail.com
- **LinkedIn:** [Alessandra Peglow](https://www.linkedin.com/in/alessandra-peglow/)

---

**Divirta-se explorando as condições do tempo!**
