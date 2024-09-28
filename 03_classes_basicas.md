# Classes Utilitárias Básicas

No Tailwind CSS, as classes utilitárias são a espinha dorsal da estilização. Elas permitem que você aplique estilos diretamente aos elementos HTML, promovendo um desenvolvimento rápido e eficiente. Neste módulo, abordaremos algumas das classes utilitárias básicas mais usadas.

## Estrutura de Classes Utilitárias

As classes utilitárias no Tailwind seguem um padrão que descreve a propriedade CSS que está sendo aplicada, e muitas vezes incluem modificadores para especificar valores. Por exemplo:

- **Espaçamento**: `m-4` (margin), `p-4` (padding)
- **Cores**: `bg-blue-500` (background), `text-white` (texto)
- **Tipografia**: `font-bold` (negrito), `text-lg` (tamanho do texto)

## Cores, Espaçamentos e Tipografia

### 1. Cores

Tailwind CSS vem com uma paleta de cores predefinidas. Para aplicar uma cor de fundo ou de texto, você pode usar as classes correspondentes:

```html
<div class="bg-blue-500 text-white p-4">
  Este é um exemplo de um bloco com fundo azul e texto branco.
</div>
```

### 2. Espaçamentos

As classes de espaçamento são baseadas em uma escala de 0 a 96, que representa valores em `rem`. Você pode usar classes para margem (m) e padding (p):

```html
<div class="m-4 p-6">
  Este bloco tem margem de 4 e padding de 6.
</div>
```

### 3. Tipografia

Tailwind oferece várias classes para controlar a tipografia, como tamanho de fonte, peso e alinhamento. Aqui estão alguns exemplos:

```html
<h1 class="text-3xl font-bold text-center">
  Título com tamanho grande e negrito.
</h1>
```

## Exemplo de Layout Simples

Aqui está um exemplo de como combinar várias classes utilitárias para criar um layout simples:

```html
<div class="max-w-md mx-auto bg-white shadow-md rounded-lg overflow-hidden">
  <div class="p-6">
    <h2 class="text-lg font-semibold">Título do Cartão</h2>
    <p class="text-gray-700">Este é um exemplo de um cartão usando Tailwind CSS.</p>
  </div>
</div>
```

## Recursos Adicionais

Para mais informações sobre classes utilitárias, consulte a [documentação oficial](https://tailwindcss.com/docs/utility-first).

## Conclusão

Neste módulo, exploramos as classes utilitárias básicas do Tailwind CSS, incluindo cores, espaçamentos e tipografia. No próximo módulo, discutiremos como criar componentes reutilizáveis e personalizar estilos com SCSS.
