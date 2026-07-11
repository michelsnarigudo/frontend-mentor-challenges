# Frontend Mentor - QR Code Component

<p align="center">
  <a href="#-sobre-o-desafio">Sobre o desafio</a> •
  <a href="#-tecnologias-e-conceitos-utilizados">Tecnologias</a> •
  <a href="#-o-que-aprendi">O que aprendi</a> •
  <a href="#-como-rodar">Como rodar</a>
</p>

<div align="center">

![Preview do projeto](./design/preview.jpg)

</div>

## 🎯 Sobre o desafio

O desafio é construir este componente de QR code e deixá-lo o mais próximo possível do design fornecido.

Os usuários devem ser capazes de:

- Visualizar o layout ideal do componente dependendo do tamanho da tela do dispositivo

Desafio original: [QR code component](https://www.frontendmentor.io/challenges/qr-code-component-iux_sIO_H) no Frontend Mentor.

## 💻 Tecnologias e conceitos utilizados

- HTML semântico
- CSS (Flexbox, box model)
- Layout responsivo (320px até desktop)

## 📚 O que aprendi

### width vs max-width

Aprendi que ao usar um valor fixo de largura o elemento não fica flexivel, o que é ruim, então é preciso usar uma combinação de width e max-width para o elemento ocupar o máximo de espaço possivel sem ultrapassar o valor de max-width.

```css
width: 100%;
max-width: 390px;
```

### height: auto em vez de altura fixa

Aprendi que ao não declarar height é assumido o valor padrão auto, o container cresce conforme o necessario, ou seja, é calculado sozinho baseado no conteudo de dentro (soma da imagem + texto + gaps).

## 🚀 Buscando evolução

- Estimar medida dos elementos de olho, sem precisar depender do figma, até porque nem todo projeto vai ter um figma.
- Escrever CSS com mais confiança e tranquilidade, quero dominar o CSS.

## ⚙️ Como rodar

```bash
# Clone o repositório
git clone https://github.com/michelsnarigudo/frontend-mentor-challenges.git

# Entre na pasta do projeto
cd frontend-mentor-challenges/newbie/qr-code-component
```

Depois é só abrir o `index.html` no navegador.

---

<p align="center">
  Feito por <a href="https://github.com/michelsnarigudo">michelsnarigudo</a>
</p>
