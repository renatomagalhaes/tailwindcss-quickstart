# Configuração do Ambiente

## Instalando o Tailwind CSS

Para começar a usar o Tailwind CSS em seu projeto, siga os passos abaixo. Você pode usar o Tailwind CSS em um projeto existente ou criar um novo projeto do zero.

### 1. Criando um Novo Projeto

Caso você não tenha um projeto existente, inicie um novo projeto com o seguinte comando:

```bash
mkdir meu-projeto-tailwind
cd meu-projeto-tailwind
npm init -y
```

### 2. Instalando Tailwind via npm

Execute o seguinte comando para instalar o Tailwind CSS e suas dependências:

```bash
npm install -D tailwindcss postcss autoprefixer
```

### 3. Inicializando o Tailwind

Após a instalação, inicialize o Tailwind e o PostCSS com o comando:

```bash
npx tailwindcss init -p
```

Isso criará dois arquivos: `tailwind.config.js` e `postcss.config.js`.

## Configurando o arquivo tailwind.config.js

O arquivo `tailwind.config.js` é onde você pode personalizar seu projeto Tailwind. Aqui está um exemplo básico:

```javascript
/** @type {import('tailwindcss').Config} */
module.exports = {
  content: ['./src/**/*.{html,js}'],
  theme: {
    extend: {},
  },
  plugins: [],
}
```

### 1. Configurando o Path de Conteúdo

A propriedade `content` permite que o Tailwind saiba onde procurar suas classes. Altere os caminhos para incluir todos os arquivos onde você usará as classes Tailwind.

### 2. Personalizando o Tema

Você pode estender o tema padrão do Tailwind adicionando novas cores, fontes ou espaçamentos dentro da propriedade `theme`.

## Integrando com SCSS

Se você estiver usando SCSS em seu projeto, é possível integrar o Tailwind com SCSS. Aqui estão os passos:

### 1. Instalando SASS

Se ainda não tiver o SASS instalado, você pode instalá-lo com o comando:

```bash
npm install -D sass
```

### 2. Criando um Arquivo SCSS

Crie um arquivo `styles.scss` e adicione as diretrizes do Tailwind:

```scss
@tailwind base;
@tailwind components;
@tailwind utilities;
```

### 3. Compilando o SCSS

Adicione um script no seu `package.json` para compilar o SCSS:

```json
"scripts": {
  "build-css": "sass styles.scss styles.css --no-source-map"
}
```

Agora você pode executar:

```bash
npm run build-css
```

## Recursos Adicionais

Para mais informações sobre a instalação e configuração do Tailwind CSS, consulte a [documentação oficial](https://tailwindcss.com/docs/installation).

## Conclusão

Neste módulo, cobrimos a instalação e configuração do Tailwind CSS em um novo projeto, além de como integrá-lo com SCSS. No próximo módulo, exploraremos as classes utilitárias básicas que o Tailwind oferece.
