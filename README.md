# Lista de Tarefas

> Aplicação web introdutória para adicionar tarefas a uma lista e armazenar os dados no navegador usando JavaScript e `localStorage`.

![Status](https://img.shields.io/badge/status-em%20desenvolvimento-yellow)
![Versão](https://img.shields.io/badge/vers%C3%A3o-0.1.0-blue)
![Tecnologias](https://img.shields.io/badge/tecnologias-HTML%20%7C%20JavaScript-orange)

---

## 📋 Sobre o projeto

O **Lista de Tarefas** é um projeto de estudo que demonstra a integração entre HTML e JavaScript para criar uma lista simples de tarefas. Os itens são mantidos em um array durante a execução e persistidos no navegador por meio da API `localStorage`, permitindo que a lista seja recuperada após atualizar ou reabrir a página no mesmo navegador. O projeto foi desenvolvido em acompanhamento ao curso Full Stack Pro - Sujeito Programador.

### Objetivos de aprendizagem

- Estruturar uma página com HTML5.
- Selecionar elementos do DOM com `document.querySelector()`.
- Criar elementos HTML dinamicamente com `document.createElement()`.
- Tratar eventos de clique.
- Trabalhar com arrays e funções JavaScript.
- Converter dados entre objetos JavaScript e JSON com `JSON.stringify()` e `JSON.parse()`.
- Persistir informações no navegador com `localStorage`.

## ✨ Funcionalidades implementadas

- Campo de texto para digitar uma tarefa.
- Botão **Registrar** para adicionar uma tarefa à lista.
- Exibição dinâmica dos itens cadastrados.
- Aviso quando o campo está vazio.
- Persistência das tarefas com a chave `@listaTarefas` no `localStorage`.
- Recuperação e renderização das tarefas armazenadas ao carregar a página.

### Limitações atuais

- A função `deletarTarefa(posicao)` existe no JavaScript, mas não está conectada a um botão ou controle na interface; portanto, a exclusão de tarefas ainda não está disponível para o usuário pela página.
- O campo de texto não tem um `id` ou `name` definido, embora seja localizado atualmente pelo seletor `#app input`.
- A validação verifica apenas se o valor é uma string vazia. Entradas contendo somente espaços podem ser registradas.
- Não há estilos CSS próprios; a aparência depende dos estilos padrão do navegador.
- Os dados ficam apenas no armazenamento local daquele navegador e dispositivo. Não há servidor, conta de usuário ou sincronização entre dispositivos.

## 🧰 Tecnologias utilizadas

- **HTML5** — estrutura da página.
- **JavaScript** — manipulação do DOM, eventos, lógica da lista e persistência.
- **DOM API** — criação e atualização dos elementos da lista.
- **Web Storage API (`localStorage`)** — armazenamento local no navegador.

O projeto não utiliza framework, biblioteca externa, processo de build ou dependências que precisem ser instaladas.

## 📁 Estrutura do projeto

```text
fe_lista_tarefas/
├── index.html       # Estrutura da interface
├── script.js        # Lógica da lista e armazenamento local
└── README.md        # Documentação do projeto
```

## ▶️ Como executar

### Opção 1 — Abrir no navegador

1. Baixe ou extraia os arquivos do projeto.
2. Abra o arquivo `index.html` em um navegador moderno.
3. Digite uma tarefa no campo de texto e clique em **Registrar**.
4. Atualize a página para verificar se a tarefa continua na lista.

### Opção 2 — Usar o Visual Studio Code

1. Abra a pasta `fe_lista_tarefas/` no VS Code.
2. Abra o arquivo `index.html` no navegador. Se utilizar a extensão Live Server, clique com o botão direito no arquivo e selecione **Open with Live Server**.

> Não é necessário executar `npm install` nem iniciar um servidor de aplicação. Para testar a persistência, mantenha o mesmo navegador e a mesma origem; abrir o arquivo diretamente e usar um servidor local pode resultar em armazenamentos separados.

## 🧪 Checklist de validação manual

- [ ] A página abre sem erros visíveis.
- [ ] Uma tarefa preenchida é adicionada à lista ao clicar em **Registrar**.
- [ ] O campo é limpo após o cadastro.
- [ ] Tentar registrar o campo vazio exibe o aviso esperado.
- [ ] As tarefas continuam visíveis depois de atualizar a página.
- [ ] O console do navegador não apresenta erros durante o fluxo básico.

## 🔧 Melhorias futuras

1. Conectar a função de exclusão à interface e adicionar um botão de remover em cada tarefa.
2. Aplicar `trim()` para impedir cadastro de entradas vazias ou compostas apenas por espaços.
3. Definir atributos `id`, `name` e um `<label>` acessível para o campo de entrada.
4. Permitir adicionar tarefas pressionando **Enter**.
5. Adicionar CSS responsivo e estados visuais para foco e interação.
6. Exibir mensagens acessíveis de sucesso e validação, em vez de depender exclusivamente de `alert()`.
7. Avaliar tratamento de dados inválidos no `localStorage` para que um conteúdo corrompido não interrompa a inicialização.
8. Adicionar testes manuais ou automatizados para cadastro, persistência e exclusão.

## 👤 Autor

**Diego Prates**

- GitHub: [@pratesddev](https://github.com/pratesddev)
- LinkedIn: [Diego Prates](https://linkedin.com/in/prates-diego)
- E-mail: [dmoprates1@gmail.com](mailto:dmoprates1@gmail.com)

---

Desenvolvido por **Diego Prates** como projeto de estudo de desenvolvimento web.

## 📄 Licença

O arquivo de origem mencionava a licença MIT, mas não incluía um arquivo `LICENSE`. Antes de distribuir o projeto sob essa licença, adicione o arquivo correspondente e confirme a intenção de licenciamento.
