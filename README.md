# Vue + Vite + Tailwind CSS Boilerplate

Um projeto boilerplate moderno que combina Vue 3, Vite e Tailwind CSS para desenvolvimento rápido de interfaces.

## 🚀 Recursos

- ⚡️ [Vue 3](https://vuejs.org/) - Framework JavaScript progressivo
- ⚡️ [Vite](https://vitejs.dev/) - Ferramenta de build extremamente rápida
- 🎨 [Tailwind CSS 3](https://tailwindcss.com/) - Framework CSS utility-first
- 🦾 [TypeScript](https://www.typescriptlang.org/) - Suporte completo a tipagem
- 📱 Design responsivo pronto para uso
- 🧩 Componentes reutilizáveis (Header e Footer)

## 📦 Estrutura do Projeto

```
/
├── public/             # Arquivos estáticos
├── src/
│   ├── assets/         # Recursos (imagens, fontes etc.)
│   ├── components/     # Componentes Vue reutilizáveis
│   │   ├── Header.vue  # Componente Header
│   │   ├── Footer.vue  # Componente Footer
│   │   └── ...
│   ├── App.vue         # Componente principal
│   ├── main.ts         # Ponto de entrada da aplicação
│   └── style.css       # Estilos globais com Tailwind CSS
├── index.html
├── package.json
├── tailwind.config.js  # Configuração do Tailwind CSS
├── postcss.config.js   # Configuração do PostCSS
└── vite.config.ts      # Configuração do Vite
```

## 🛠️ Instalação

1. Clone este repositório:

```bash
git clone <seu-repositorio>
cd <seu-repositorio>
```

2. Instale as dependências:

```bash
npm install
# ou
yarn install
# ou
pnpm install
```

3. Inicie o servidor de desenvolvimento:

```bash
npm run dev
# ou
yarn dev
# ou
pnpm dev
```

4. Acesse a aplicação em: `http://localhost:5173`

## 🔧 Configuração do Tailwind CSS

Este projeto já possui o Tailwind CSS 3 configurado. A configuração pode ser encontrada nos seguintes arquivos:

- `tailwind.config.js` - Configurações principais do Tailwind
- `postcss.config.js` - Configuração do PostCSS para processar o Tailwind
- `src/style.css` - Importação das diretivas do Tailwind

## 🧩 Componentes Incluídos

### Header

Um componente de cabeçalho responsivo que inclui:

- Logo
- Menu de navegação
- Botão de ação (login)

### Footer

Um componente de rodapé responsivo que inclui:

- Informações sobre o site
- Links de navegação agrupados por categoria
- Ícones de redes sociais
- Copyright com ano atual

## 📝 Personalização

### Modificando o Tailwind

Para customizar o Tailwind, edite o arquivo `tailwind.config.js`:

```js
/** @type {import('tailwindcss').Config} */
export default {
  content: ['./index.html', './src/**/*.{vue,js,ts,jsx,tsx}'],
  theme: {
    extend: {
      // Adicione suas customizações aqui
      colors: {
        // Exemplo: 'primary': '#ff0000',
      },
      // ...outras customizações
    },
  },
  plugins: [
    // Adicione plugins aqui
  ],
};
```

### Adicionando Novos Componentes

Para adicionar novos componentes:

1. Crie um novo arquivo .vue na pasta `src/components/`
2. Importe e use o componente onde necessário

Exemplo:

```vue
<script setup lang="ts">
import NovoComponente from './components/NovoComponente.vue';
</script>

<template>
  <NovoComponente />
</template>
```

## 🏗️ Build para Produção

Para criar uma versão de produção:

```bash
npm run build
# ou
yarn build
# ou
pnpm build
```

Os arquivos para produção serão gerados na pasta `dist`.

## 👀 Prévia

Após iniciar o servidor de desenvolvimento, você verá:

- Um cabeçalho limpo e minimalista no topo
- Três logos: Vite, Vue e Tailwind CSS (com efeito de hover)
- Um rodapé completo na parte inferior

## 📚 Recursos Adicionais

- [Documentação do Vue 3](https://vuejs.org/guide/introduction.html)
- [Documentação do Vite](https://vitejs.dev/guide/)
- [Documentação do Tailwind CSS](https://tailwindcss.com/docs)

## 📄 Licença

[MIT](LICENSE)
