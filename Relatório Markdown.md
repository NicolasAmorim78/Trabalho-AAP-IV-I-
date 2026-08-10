# Relatório: Sistema de Gestão de Biblioteca

**Disciplina:** AAP IV – Programação para Internet
**Atividade:** GUI Semântica, Responsiva e Acessível para Front-End Web
**Aluno:** Nícolas Amorim Araújo
**Professor:** Vander Elme
**GitHub:** https://github.com/CodeWitch00/trabalho1.git

## 1. Introdução

O trabalho apresenta uma interface web para um **Sistema de Gestão de Biblioteca**, desenvolvida para permitir o cadastro, a pesquisa e a visualização de livros. A proposta é acadêmica e concentra-se na aplicação de conceitos de **HTML5 e CSS3**, especialmente semântica, acessibilidade, organização visual e responsividade, sem a necessidade de backend, banco de dados ou autenticação.

O HTML5 foi utilizado para estruturar o conteúdo, enquanto o CSS3 define a aparência, a adaptação a diferentes telas e os temas claro e escuro. O JavaScript possui função complementar, sendo utilizado para cadastro dinâmico, pesquisa, mudança de tema e controle das fichas. A estrutura principal permanece no HTML, reduzindo a dependência do JavaScript.

## 2. Estrutura semântica

A página foi organizada com elementos semânticos do HTML5, permitindo identificar a finalidade de cada área. O **`<header>`** contém a identificação da biblioteca e o título principal. O **`<nav>`** reúne os controles de navegação entre as fichas de Cadastro, Acervo, Resumo e a opção de exibição completa. O **`<main>`** delimita o conteúdo principal, enquanto **`<section>`** e **`<aside>`** organizam as diferentes áreas da interface.

O cadastro utiliza **`<form>`**, **`<fieldset>`** e **`<legend>`** para agrupar os dados da obra e sua disponibilidade. Os elementos **`<label>`** identificam os campos, enquanto `required` indica informações obrigatórias e `placeholder` apresenta exemplos de preenchimento.

Para o acervo foi utilizada uma tabela HTML composta por **`<table>`**, **`<caption>`**, **`<thead>`** e **`<tbody>`**, adequada para representar informações organizadas em linhas e colunas. O **`<footer>`** reúne as informações acadêmicas do projeto.

## 3. Acessibilidade e navegação

A interface utiliza o conceito visual de fichas de biblioteca, permitindo selecionar uma área específica ou visualizar todas simultaneamente. Para tornar essa navegação mais acessível, foram utilizados recursos ARIA, como **`role="tablist"`**, **`role="tab"`**, **`role="tabpanel"`**, `aria-selected` e `aria-controls`.

Também foi implementado um **skip link**, permitindo que usuários que navegam pelo teclado avancem diretamente para o conteúdo principal. Os elementos interativos possuem indicação de foco por meio de **`:focus-visible`**. Campos obrigatórios são identificados visualmente e mensagens de atualização utilizam `role="status"` e `aria-live="polite"`.

A escolha das cores considera a diferenciação visual entre os componentes, utilizando principalmente azul, bege e vermelho terracota.

## 4. Responsividade e CSS

A interface foi planejada para diferentes tamanhos de tela, evitando uma estrutura dependente de dimensões fixas. As fichas são organizadas verticalmente e podem ser exibidas individualmente ou em conjunto. Em dispositivos móveis, os controles de navegação são reorganizados para facilitar a interação por toque.

A tabela do acervo também recebe tratamento específico para telas pequenas, podendo assumir uma apresentação semelhante a cartões e utilizando `data-label` para preservar a identificação das informações.

HTML, CSS e JavaScript foram mantidos em arquivos separados. O CSS utiliza **custom properties** para centralizar as cores e facilitar a manutenção do projeto. A identidade visual utiliza **`#1f3a52`** como azul principal, **`#faf7f0`** como superfície clara e **`#c0392b`** para estados de destaque. O projeto também possui modo escuro por meio de `[data-theme="dark"]`.

## 5. JavaScript e conclusão

O JavaScript acrescenta interatividade à aplicação por meio do cadastro dinâmico, filtro de pesquisa, alternância de tema e controle das fichas. Entretanto, ele não substitui a estrutura HTML, que contém o conteúdo essencial da página. Recursos como banco de dados, API, autenticação e servidor não foram incluídos por não fazerem parte do escopo da atividade.

Conclui-se que o projeto atende à proposta de desenvolver uma **GUI semântica, responsiva e acessível**, utilizando os recursos fundamentais de HTML5 e CSS3. A estrutura semântica melhora a organização do conteúdo, enquanto os recursos de acessibilidade favorecem a navegação por diferentes usuários. A responsividade permite o uso em diferentes dispositivos, e o JavaScript complementa a experiência com funcionalidades interativas. Assim, o resultado apresenta uma solução simples, organizada e adequada aos objetivos acadêmicos da atividade.
