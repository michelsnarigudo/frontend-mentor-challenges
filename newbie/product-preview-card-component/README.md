# Frontend Mentor - Product Preview Card Component

<p align="center">
  <a href="#-sobre-o-desafio">Sobre o desafio</a> •
  <a href="#-tecnologias-e-conceitos-utilizados">Tecnologias</a> •
  <a href="#-o-que-aprendi">O que aprendi</a> •
  <a href="#-como-rodar">Como rodar</a>
</p>

<div align="center">

![Preview do projeto](./design/desktop-preview.jpg)

</div>

## 🎯 Sobre o desafio

O desafio é construir este card de produto e deixá-lo o mais próximo possível do design fornecido.

Os usuários devem ser capazes de:

- Visualizar o layout ideal do componente dependendo do tamanho da tela (duas colunas no desktop, empilhado no mobile)
- Ver os estados de hover e focus nos elementos interativos

Desafio original: [Product preview card component](https://www.frontendmentor.io/challenges/product-preview-card-component-GO7UmttRfa) no Frontend Mentor.

## 💻 Tecnologias e conceitos utilizados

- HTML semântico (`article`, `picture`, `s`)
- CSS Grid e Flexbox
- Imagem responsiva com `<picture>` e `<source>`
- Acessibilidade com a técnica visually-hidden
- Layout responsivo com media query (320px até desktop)

## 📚 O que aprendi

### Imagens diferentes por tamanho de tela com `<picture>`

O elemento `source` troca a imagem conforme a media query, sem precisar de CSS ou JS. A `img` serve de fallback e carrega o `alt`:

```html
<picture>
  <source media="(max-width: 600px)" srcset="./images/image-product-mobile.jpg">
  <img src="./images/image-product-desktop.jpg" alt="..." />
</picture>
```

### Acessibilidade nos preços com visually-hidden

O leitor de tela lia os dois preços sem contexto. A solução é um texto extra escondido visualmente, mas audível — encolhido a 1px em vez de `display: none` (que o leitor de tela ignoraria):

```html
<p class="product-original-price">
  <span class="visually-hidden">Original price: </span><s>$169.99</s>
</p>
```

### `<s>` para preço antigo

A tag `s` marca conteúdo que não é mais relevante/preciso (diferente de `del`, que indica remoção editorial). Semântica em vez de só risco visual.

### Grid empilha por padrão

`display: grid` sem `grid-template-columns` já empilha os filhos (uma coluna, cada filho vira uma linha) — por isso `display: grid; gap: 1rem` resolve o espaçamento vertical em duas linhas, sem declarar direção como no flex.

## 🚀 Buscando evolução

- Fiz este desafio desktop-first de propósito e comparei com a abordagem mobile-first para entender na prática por que ela gera menos código de "desfazer". Próximo desafio será mobile-first.
- Quero praticar mais a aplicação de acessibilidade até virar algo natural, e melhorar a decisão de **em qual elemento** aplicar cada propriedade (espaçamentos principalmente).
- Adotar variáveis CSS (`:root` + `var()`) nos próximos projetos.

## ⚙️ Como rodar

```bash
# Clone o repositório
git clone https://github.com/michelsnarigudo/frontend-mentor-challenges.git

# Entre na pasta do projeto
cd frontend-mentor-challenges/newbie/product-preview-card-component
```

Depois é só abrir o `index.html` no navegador.

---

<p align="center">
  Feito por <a href="https://github.com/michelsnarigudo">michelsnarigudo</a>
</p>
