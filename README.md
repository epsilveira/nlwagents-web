# NLW Agents - Frontend

Este é o repositório do frontend da aplicação "NLW Agents", desenvolvida durante a Next Level Week da Rocketseat. A aplicação é uma plataforma de perguntas e respostas em tempo real, onde os usuários podem fazer perguntas, inclusive gravando áudio, e receber respostas geradas por uma Inteligência Artificial.

## ✨ Tecnologias

Este projeto foi construído com um conjunto de tecnologias modernas para desenvolvimento web, focando em performance e experiência do desenvolvedor.

| Tecnologia | Descrição |
| :--- | :--- |
| **Vite** | Um ferramental de frontend de última geração que oferece uma experiência de desenvolvimento extremamente rápida através do seu servidor de desenvolvimento nativo (ESM) e build otimizado com Rollup. |
| **React** | Uma biblioteca JavaScript para construir interfaces de usuário (UI) declarativas e baseadas em componentes. É a base da nossa aplicação. |
| **TypeScript** | Um superset do JavaScript que adiciona tipagem estática opcional. Ajuda a prevenir bugs em tempo de desenvolvimento e melhora a legibilidade e manutenção do código. |
| **Tailwind CSS** | Um framework CSS *utility-first* para criar designs customizados rapidamente sem sair do HTML. Ele permite estilizar componentes de forma eficiente e consistente. |
| **shadcn/ui** | Não é uma biblioteca de componentes tradicional, mas sim uma coleção de componentes reutilizáveis, acessíveis e customizáveis construídos com Radix UI e Tailwind CSS que podem ser facilmente integrados ao projeto. |
| **Lucide React** | Uma biblioteca de ícones SVG leve, customizável e de fácil utilização, que fornece os ícones usados na interface. |
| **Day.js** | Uma biblioteca minimalista para manipulação, validação e exibição de datas e horas. Usada para formatar os timestamps das perguntas. |
| **Axios** | Um cliente HTTP baseado em *Promises* para o navegador e Node.js. É utilizado para realizar as requisições para a API do backend de forma simples e eficiente. |

---

## 🚀 Começando

Siga os passos abaixo para configurar e executar o projeto em seu ambiente local.

### Pré-requisitos

- **Node.js**: Versão 18.x ou superior.
- **npm**, **yarn** ou **pnpm** como gerenciador de pacotes.
- **Backend em execução**: O [servidor da API](https://github.com/epsilveira/nlwagents-server) precisa estar rodando localmente, pois o frontend depende dele para funcionar.

### Instalação

1. **Clone o repositório:**
   ```bash
   git clone https://github.com/epsilveira/nlwagents-web.git
   ```

2. **Navegue até o diretório do projeto:**
   ```bash
   cd nlwagents-web
   ```

3. **Instale as dependências:**
   ```bash
   npm install
   ```

4. **Configure as variáveis de ambiente:**
   - Crie uma cópia do arquivo de exemplo `.env.example`:
     ```bash
     cp .env.example .env
     ```
   - Abra o arquivo `.env` e configure a variável `VITE_API_URL`. Ela deve apontar para a URL onde o seu backend está rodando. Por padrão, o valor é `http://localhost:3333`.
     ```env
     VITE_API_URL=http://localhost:3333
     ```

---

## 📜 Scripts Disponíveis

No diretório do projeto, você pode executar os seguintes scripts:

### `npm run dev`

Inicia o servidor de desenvolvimento do Vite em modo de desenvolvimento.

- **O que faz?** Compila a aplicação e a serve em um endereço local (geralmente `http://localhost:5173`). Ele utiliza Hot-Module Replacement (HMR) para atualizar a aplicação no navegador instantaneamente sempre que você salva um arquivo.
- **Quando usar?** Durante o desenvolvimento ativo da aplicação.

---

### `npm run build`

Compila e otimiza a aplicação para produção.

- **O que faz?** Executa o `tsc` para verificar os tipos do TypeScript e, em seguida, o `vite build` para criar uma versão otimizada, minificada e pronta para deploy da sua aplicação. Os arquivos resultantes são salvos no diretório `dist/`.
- **Quando usar?** Quando você estiver pronto para fazer o deploy da sua aplicação em um ambiente de produção.

---

### `npm run lint`

Executa o linter (ESLint) para analisar o código em busca de problemas.

- **O que faz?** Verifica todos os arquivos `.ts` e `.tsx` em busca de erros de código, inconsistências de estilo e potenciais bugs, de acordo com as regras configuradas.
- **Quando usar?** Antes de commitar seu código, para garantir a qualidade e a consistência do mesmo.

---

### `npm run preview`

Inicia um servidor local para visualizar o build de produção.

- **O que faz?** Serve os arquivos estáticos do diretório `dist/` em um servidor local. É uma maneira fácil de verificar se a versão de produção da sua aplicação está funcionando como esperado antes de publicá-la.
- **Quando usar?** Após executar `npm run build` para testar o resultado final localmente.