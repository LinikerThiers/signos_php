# 🔮 Site de Signos em PHP

Este é um projeto prático desenvolvido como parte da disciplina de **Programação Web** do curso de **Engenharia de Software** na **UNOPAR**.  
O objetivo do projeto é apresentar informações sobre os signos do zodíaco utilizando **PHP** e **XML**, de forma simples e funcional.

---

## 🧩 Sobre o Projeto

O site permite que o usuário selecione um signo de acordo com a data de aniversário.
Os dados são armazenados em um arquivo `.xml` e carregados dinamicamente com PHP, utilizando a função `simplexml_load_file`.

---

## 📁 Estrutura dos Arquivos

```
signos-php/
│
├── index.php                  # Página principal com a seleção da data de aniversário
├── show_zodiac_sign.php      # Página que exibe as informações do signo escolhido
├── signos.xml                 # Arquivo XML contendo os dados dos signos
│
├── layout/
│   ├── header.php             # Cabeçalho comum às páginas
│   └── footer.php             # Rodapé comum às páginas
│
├── assets/
│   └── css/
│       └── style.css          # Estilos da página
│
└── README.md                  # Documentação do projeto
```

---

## 📄 Explicação dos Arquivos

### `index.php`
Página inicial do site. Apresenta um imput para o usuário escolher a sua data de aniversário, e estará dentro de um form com o metodo post para realização da consulta.

### `show_zodiac_sign.php`
Recebe a data de aniversário por parâmetro e carrega o arquivo XML para buscar e exibir as informações correspondentes. A leitura dos dados é feita com `simplexml_load_file`.

### `signos.xml`
Arquivo que contém as informações de todos os signos, estruturado em XML com elementos como `<signo>`, `<dataInicio>`, `<dataFim>`, `<signoNome>`, `<descricao>`.

Exemplo de estrutura:
```xml
<signos>
    <signo>
        <dataInicio>21/01</dataInicio>
        <dataFim>18/02</dataFim>
        <signoNome>Aquário</signoNome>
        <descricao>Original, visionário e independente. Gosta de inovar, pensar fora da caixa e lutar por causas coletivas.</descricao>
    </signo>
  <!-- Outros signos... -->
</signos>
```

### `layout/header.php` e `layout/footer.php`
Arquivos reutilizáveis que representam o cabeçalho e o rodapé da página, respectivamente. Facilitam a manutenção e organização do código.

### `assets/css/style.css`
Folha de estilos com o design e formatação visual do site.

---

## 🎓 Instituição

> Projeto desenvolvido na disciplina de **Programação Web**  
> Curso de **Engenharia de Software** – UNOPAR  
> Aluno: *Liniker Thiers Simões Silva*  
> Semestre: *5º Semestre*

---

## 🚀 Como Executar

1. Clone ou baixe o repositório.
2. Coloque a pasta do projeto em um servidor local (ex: XAMPP, WAMP).
3. Acesse no navegador:  
   `http://localhost/signos-php/index.php`
4. Escolha uma data e veja o signo correspondente a ela.

---

## 📌 Tecnologias Utilizadas

- PHP
- XML
- HTML/CSS (opcional)
- Bootstrap

---

## 💡 Possíveis Melhorias

- Adicionar imagens dos signos
- Tornar o layout responsivo
- Migrar os dados para um banco de dados (MySQL)
- Versão com API REST em PHP

---
