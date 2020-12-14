

# Jogo da memória Dev!

Jogo da memória com 12 posições para Dev's.

#### Disposição das cartas nas divs
```html
        <div class="card" data-card="angular">
            <img class="card-front" src="./img/Angular.png" alt="Face da carta">
            <img class="card-back" src="./img/box2.png" alt="Verso da carta">
        </div>
        <div class="card" data-card="node">
            <img class="card-front" src="./img/Node.png" alt="Face da carta">
            <img class="card-back" src="./img/box2.png" alt="Verso da carta">
        </div>
```

#### Função para embaralhar as cartas
```js
(function shuffle() {
    cards.forEach((card) => {
        let ramdomPosition = Math.floor(Math.random() * 12);
        card.style.order = ramdomPosition;
    })
})();
```

#### Função para desvirar as cartas
```js
function unflipCards() {
    lockBoard = true;

    setTimeout(() => {
        firstCard.classList.remove('flip');
        secondCard.classList.remove('flip');

        resetBoard();
    }, 1500);
}
```

#### Imagem Ilustrativa do jogo

![fig1](/.tmp/fig1.png)

![](/.tmp/fig2.png)

