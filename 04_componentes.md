# Componentes e Personalização

Um dos grandes benefícios do Tailwind CSS é a capacidade de criar componentes reutilizáveis que podem ser personalizados facilmente. Neste módulo, discutiremos como criar componentes e como integrar o Tailwind com SCSS para personalização.

## Criando Componentes Reutilizáveis

Componentes reutilizáveis são blocos de código que podem ser utilizados em diferentes partes da sua aplicação, facilitando a manutenção e a consistência visual. Aqui está um exemplo de um botão reutilizável:

```html
<button class="bg-blue-500 text-white font-semibold py-2 px-4 rounded hover:bg-blue-600">
  Clique aqui
</button>
```

### Exemplo de Componente de Cartão

Vamos criar um componente de cartão reutilizável:

```html
<div class="bg-white shadow-lg rounded-lg overflow-hidden">
  <img src="imagem.jpg" alt="Descrição da imagem" class="w-full h-48 object-cover">
  <div class="p-4">
    <h2 class="text-xl font-bold">Título do Cartão</h2>
    <p class="text-gray-700">Descrição do conteúdo do cartão.</p>
    <button class="mt-2 bg-green-500 text-white py-1 px-3 rounded hover:bg-green-600">
      Ação
    </button>
  </div>
</div>
```

## Personalizando Classes com SCSS

Embora o Tailwind forneça uma vasta gama de classes utilitárias, você pode personalizar ainda mais os estilos utilizando SCSS. O SCSS permite que você agrupe classes e adicione estilos personalizados.

### Usando o @apply

O Tailwind CSS oferece a diretiva `@apply` para aplicar um conjunto de classes utilitárias a uma classe CSS personalizada. Aqui está como você pode usá-la:

```scss
.btn {
  @apply bg-blue-500 text-white font-semibold py-2 px-4 rounded hover:bg-blue-600;
}
```

Você pode então usar essa classe personalizada em seus elementos HTML:

```html
<button class="btn">
  Clique aqui
</button>
```

## Exemplo de Componente de Navegação

Aqui está um exemplo de um componente de navegação utilizando SCSS e Tailwind:

```html
<nav class="bg-gray-800 p-4">
  <ul class="flex space-x-4">
    <li><a href="#" class="text-white hover:text-gray-400">Home</a></li>
    <li><a href="#" class="text-white hover:text-gray-400">Sobre</a></li>
    <li><a href="#" class="text-white hover:text-gray-400">Serviços</a></li>
    <li><a href="#" class="text-white hover:text-gray-400">Contato</a></li>
  </ul>
</nav>
```

## Recursos Adicionais

Para mais informações sobre como criar componentes e personalizar estilos, consulte a [documentação oficial](https://tailwindcss.com/docs/components).

## Conclusão

Neste módulo, discutimos como criar componentes reutilizáveis e personalizar estilos utilizando SCSS e Tailwind CSS. No próximo módulo, abordaremos a responsividade e o uso de pseudo-classes no Tailwind.
