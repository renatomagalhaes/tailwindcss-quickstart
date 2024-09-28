# Responsividade e Pseudo-classes

Uma das principais características do Tailwind CSS é sua abordagem fácil para design responsivo. Neste módulo, abordaremos como utilizar breakpoints para responsividade e como aplicar pseudo-classes.

## Utilizando Breakpoints

Tailwind CSS oferece uma série de breakpoints pré-definidos que facilitam a aplicação de estilos diferentes em diferentes tamanhos de tela. Os breakpoints padrão são:

- `sm` - 640px
- `md` - 768px
- `lg` - 1024px
- `xl` - 1280px
- `2xl` - 1536px

### Exemplo de Uso de Breakpoints

Você pode aplicar classes utilitárias específicas para cada breakpoint, adicionando o prefixo correspondente. Por exemplo:

```html
<div class="bg-blue-500 p-4 sm:bg-green-500 md:bg-red-500 lg:bg-yellow-500">
  Este bloco muda de cor dependendo do tamanho da tela.
</div>
```

Neste exemplo, o bloco terá fundo azul em telas pequenas, verde em telas médias, vermelho em telas grandes e amarelo em telas extra grandes.

## Pseudo-classes e Estados

O Tailwind CSS também suporta pseudo-classes, permitindo que você aplique estilos em diferentes estados de um elemento, como `hover`, `focus`, e `active`.

### Exemplo de Pseudo-classe Hover

Você pode usar as pseudo-classes para adicionar estilos quando um elemento é passado o mouse ou está em foco:

```html
<button class="bg-blue-500 text-white py-2 px-4 rounded hover:bg-blue-600 focus:outline-none focus:ring-2 focus:ring-blue-400">
  Botão com Estilos de Hover e Focus
</button>
```

Neste exemplo, o botão mudará de cor quando o mouse estiver sobre ele e também exibirá um anel ao ser focado.

## Exemplo Completo de Layout Responsivo

Aqui está um exemplo de um layout simples que utiliza breakpoints e pseudo-classes:

```html
<div class="flex flex-col md:flex-row">
  <div class="md:w-1/2 bg-blue-500 p-4 hover:bg-blue-600">
    Coluna 1
  </div>
  <div class="md:w-1/2 bg-green-500 p-4 hover:bg-green-600">
    Coluna 2
  </div>
</div>
```

Neste layout, as colunas serão exibidas em uma única coluna em telas pequenas e em duas colunas em telas médias ou maiores.

## Recursos Adicionais

Para mais informações sobre responsividade e pseudo-classes, consulte a [documentação oficial](https://tailwindcss.com/docs/responsive-design) e [pseudo-classes](https://tailwindcss.com/docs/pseudo-class-variants).

## Conclusão

Neste módulo, exploramos como utilizar breakpoints para responsividade e aplicamos pseudo-classes para estados de elementos. No próximo módulo, discutiremos boas práticas em Tailwind CSS para manter seu código organizado e eficiente.
