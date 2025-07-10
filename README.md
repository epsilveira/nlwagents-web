# NLW Agents - Web

Este é o frontend do projeto **NLW Agents**, desenvolvido durante a trilha de React no evento Next Level Week da [Rocketseat](https://rocketseat.com.br).

## 🚀 Tecnologias Utilizadas

O projeto foi construído com um conjunto de tecnologias modernas para o desenvolvimento web:

- **React**: Biblioteca para construção de interfaces de usuário.
- **Vite**: Ferramenta de build para um desenvolvimento frontend mais rápido.
- **TypeScript**: Superset do JavaScript que adiciona tipagem estática.
- **Tailwind CSS**: Framework CSS utility-first para estilização rápida e customizável.
- **shadcn/ui**: Coleção de componentes de UI reutilizáveis.
- **Biome**: Ferramenta para formatação e linting do código, garantindo consistência e qualidade.
- **React Router Dom** - Biblioteca de roteamento
- **TanStack React Query** - Gerenciamento de estado servidor e cache
- **Radix UI** - Componentes primitivos acessíveis
- **Lucide React** - Biblioteca de ícones

## 🏛️ Padrões e Arquitetura

O projeto utiliza **path aliases** (ex: `@/components`) para facilitar a importação de módulos e manter o código mais limpo e organizado. Essa configuração pode ser encontrada nos arquivos `tsconfig.json` e `vite.config.ts`.

## ⚙️ Setup e Configuração

Siga os passos abaixo para configurar e executar o projeto em seu ambiente local.

### 1. Clonar o Repositório

```bash
git clone https://github.com/epsilveira/nlwagents-web.git
cd nlwagents-web
```

### 2. Instalar as Dependências

Recomenda-se o uso do `npm` para gerenciamento de pacotes.

```bash
npm install
```

### 3. Executar o Projeto

Com tudo configurado, inicie o servidor de desenvolvimento:

```bash
npm run dev
```

O projeto estará disponível em `http://localhost:5173`

### Scripts Disponíveis

- `npm run dev` - Inicia o servidor de desenvolvimento
- `npm run build` - Gera build de produção
- `npm run preview` - Preview do build de produção

### Backend

O projeto consome uma API que deve estar rodando na porta 3333. Certifique-se de que o backend esteja configurado e executando antes de iniciar o frontend.

## 🛠️ Estrutura do Projeto

```
src/
├── components/ui/    # Componentes de interface
├── pages/           # Páginas da aplicação
├── lib/             # Utilitários e configurações
└── app.tsx          # Componente raiz
``` 



