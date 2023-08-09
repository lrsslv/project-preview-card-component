## Sobre o projeto

Você deve ser capaz de:

- Ver um layout responsivo, que condiga com o tamanho da sua tela;
- Ver um efeito de _hover_ em elementos interativos.

### Sobre o processo

Apesar desse projeto ter sido um pouco parecido com outros que eu já havia feito, pude aprender algumas coisas durante o processo. Uma delas foi como alterar a imagem no modo respoonsivo utilizando apenas HTML e CSS, pois eu sabia de uma forma como fazer isso utilizando JS. 

Para o problema em questão, precisava esconder a imagem da versão _desktop_ na versão _mobile_ e vice-versa. Para isso, fiz o seguinte:

```html
 <picture class="preview">
            <img class="product-desktop" src="./src/images/image-product-desktop.jpg" alt="Gabrielle Essence Eau De Parfum">
        </picture>

        <picture class="preview">
            <img class="product-mobile" src="./src/images/image-product-mobile.jpg" alt="Gabrielle Essence Eau De Parfum">
        </picture>
```

```css
/*versão desktop*/
.container .preview .product-desktop {
    height: 450px;
    width: 300px;
}

.container .preview .product-mobile {
    display: none;
}

/*versão mobile*/
 .container .preview .product-mobile {
        display: block;
        width: 100%;
        height: 240px;
    }

    .container .preview .product-desktop {
        display: none;
    }
```