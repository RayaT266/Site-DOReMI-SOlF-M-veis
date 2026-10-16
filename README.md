# 🛋️ Site DOReMI SOlFÁ Móveis — AD1

Este repositório contém a AD1 (Avaliação a Distância 1) da disciplina Construção de Páginas WEB, do curso de Tecnologia em Sistemas de Computação oferecido pela Fundação CECIERJ em parceria com a UFF, referente ao 2º semestre de 2026.

A proposta da atividade é desenvolver, do zero, o site de uma loja fictícia de móveis especializada em sofás e camas — a DOReMI SOlFÁ. Mais do que "fazer o layout bater com a imagem do enunciado", o exercício serve como um percurso guiado por boa parte dos fundamentos de HTML e CSS: da estruturação de página com tabelas até a versão final usando as tags semânticas do HTML5, passando por listas, tabelas de dados e formulários mais elaborados.

> 🇬🇧 *English summary at the end.*

---

## 🧱 Como o projeto foi evoluindo

O trabalho não nasceu pronto — ele foi construído em camadas, seguindo a ordem proposta no próprio enunciado da AD1:

1. **Página inicial com tabela de bordas invisíveis.** A primeira versão da home usava tabela para posicionar logo, menu e texto de apresentação — a forma "clássica" de montar layout antes do CSS moderno se popularizar.
2. **Migração para HTML5 + CSS externo.** A mesma página foi refeita usando header, nav e section, com toda a aparência movida para um arquivo .css separado, sem atributos ou tags descontinuadas. Essa é a base reaproveitada em todas as páginas seguintes.
3. **Página de Camas.** Introduz listas aninhadas (ul dentro de li, ol com numeração romana) para organizar os modelos por categoria e preço.
4. **Página de Sofás.** Usa uma tabela de verdade — com rowspan para unir "Sofá 2 lugares" e "Sofá 3 lugares" às suas variações — para exibir produto, descrição, foto e preço.
5. **Página de Encomendas.** O primeiro formulário do site: login, seleção de produtos com optgroup, campo de valor readonly e dados de cartão organizados em fieldsets aninhados.
6. **Página de Cadastro.** Formulário de cadastro de cliente, reaproveitando as mesmas classes de posicionamento (ColEsq, ColDir, LabBox, InpBoxGnd...) criadas para a página de Encomendas, provando que o conjunto de classes definido ali é genérico o suficiente para servir a outros formulários.

> 💡 Uma decisão importante tomada ao longo do processo foi resistir à tentação de usar `<table>` para posicionar os campos dos formulários (prática comum há alguns anos) e resolver tudo com `float`, `display: block` e classes CSS reutilizáveis. É mais trabalhoso de acertar no início, mas deixa a estrutura HTML mais limpa e mais fácil de estilizar depois.

---

## 🗂️ Estrutura de arquivos

```
├── DoremisolfaMoveis.html   # página inicial
├── Doremi.html              # catálogo de camas
├── Solfa.html               # catálogo de sofás
├── Encomendas.html          # formulário de pedido
├── Cadastro.html            # formulário de cadastro de cliente
├── style.css                # todo o estilo do site, em um único arquivo
└── Imagens/                 # logos e fotos dos produtos
```

Todas as páginas compartilham o mesmo header e nav, e apontam para o mesmo style.css — só o conteúdo de dentro da section muda de uma para outra.

---

## 🛠️ Tecnologias

- HTML5 semântico (sem tags nem atributos descontinuados)
- CSS3, com fontes do Google Fonts (Stoke e Karla) e fallback para fontes locais
- Nenhuma dependência de JavaScript, framework ou build tool — é HTML e CSS puros, como pede o enunciado da disciplina

![HTML5](https://img.shields.io/badge/HTML5-E34F26?logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?logo=css3&logoColor=white)

---

## 🎓 Sobre a disciplina

Construção de Páginas WEB é uma disciplina introdutória de desenvolvimento front-end do curso de Tecnologia em Sistemas de Computação. As avaliações a distância (ADs) têm um peso que vai além da nota: o conteúdo cobrado nelas costuma reaparecer nas provas presenciais, então a ideia é aproveitar cada questão como treino mesmo — e não só como tarefa a ser entregue.

---

## 🚀 Como visualizar

Basta abrir o arquivo DoremisolfaMoveis.html em qualquer navegador (sem necessidade de servidor local) e navegar pelo menu. Os links do menu abrem cada página em uma nova aba, como pedido no enunciado.

---

## 👩‍💻 Autora

**Rayara Escala** — Estudante de Tecnologia em Sistemas de Computação (UFF/CEDERJ)
🔗 [LinkedIn](www.linkedin.com/in/rayaraescala-r-torres)

---

## 🇬🇧 English summary

This repository holds **Assignment 1 (AD1)** of the Web Page Construction course (UFF/CEDERJ, 2026): a fictional sofa-and-bed store website, **DOReMI SOlFÁ**, built with plain **HTML5 and CSS3**. It goes from a table-based layout to semantic HTML5 with external CSS, covering nested lists, merged-cell tables and CSS-positioned forms.

**View it:** open `DoremisolfaMoveis.html` in any browser.

---

> Projeto educacional. A loja, os produtos e os preços são fictícios.
