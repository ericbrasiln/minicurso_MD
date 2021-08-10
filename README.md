III Semana de História do campus dos Malês, IHLM/UNILAB

# Uma introdução ao Markdown e suas possibilidades no ensino e divulgação científica

Prof. [Eric Brasil](ericbrasiln.github.io)

---

Markdown é uma sintaxe baseada em texto simples para formatação de documentos. Possui muitas opções interessantes para produção de materiais didáticos, apresentações entre outros.

---

## Ementa

O que é a sintaxe Markdown. Estrutura básica: cabeçalhos, parágrafos, tabelas, imagens, gifs, links, códigos, listas, html. Editores de markdown. "Sabores" e temas. Exportando e colocando online.

---

***Esse minicurso é inspirado e utiliza como base a lição [Introdução ao Markdown](https://programminghistorian.org/pt/licoes/introducao-ao-markdown), de Sarah Simpkin, publicada no [ProgrammingHistorian](https://programminghistorian.org/pt) e traduzida para o português por [João Gilberto Saraiva](https://0jonjo.github.io/)***

---

Vamos começar!

![gato](https://media.giphy.com/media/LmNwrBhejkK9EFP504/source.gif)

---

## A Sintaxe

A sintaxe Markdown foi criada em 2004 e é um modo de formatar arquivos de textos simples, utilizando algumas marcações com símbolos como `#`, `*`, `[]()` etc.

Esses arquivos são salvos com a extensão `.md` e podem ser abertos com editores de texto simples, como Gedit, Notepad, etc. Assim, podem ser abertos em diferentes sistemas operacionais.

Além disso, muitas plataformas de publicação e sites aceitam arquivos arquivos `.md`, muitas vezes renderizando o arquivo automaticamente para HTML.

Atualmente, existem inúmeros programas gratuitos e de código aberto para edição de Markdown, possibiltando a configuração de muitos recursos, temas (ou "flavours") e opções de exportação (seja em html, pdf, doc, etc). 

---

### Pq usar Markdown para suas aulas e apresentações?

- A pandemia e o ensino remoto; 
- Como transpor a aula presencial para o virtual? Oi? 😰
- A maldição dos pdfs e ppts. 👻

<img src="https://media.giphy.com/media/xXbwgiIjYaZJC86YCk/source.gif" alt="ppt" style="zoom:50%;" />

- Versatilidade, adaptabilidade, leveza, compartilhável 📡

---

## Estrutura báscia

Vamos agora entender a estrutura básica de um arquivo em `.md`. 

---

### Cabeçalhos

```
# Primeiro nível de cabeçalho
## Segundo nível de cabeçalho
### Terceiro nível de cabeçalho
#### Quarto nível de cabeçalho
```

---

Renderiza como:

# Primeiro nível de cabeçalho

## Segundo nível de cabeçalho

### Terceiro nível de cabeçalho

#### Quarto nível de cabeçalho

---

### Parágrafos e Quebras de linha

Os parágrafos devem ser separados por uma linha vazia.

Por exemplo:

```
Vamos aprender markdown?

Para separar parágrafos precisamos inserir um linha em branco para criar um parágrafo.
```

Isso renderiza assim:

Vamos aprender markdown?

Para separar parágrafos precisamos inserir um linha em branco para criar um parágrafo.

---

### Ênfases

Para colocar um texto em itálico é só colocá-lo entre `*` ou `_` e em negrito entre `**` ou `__`.

```
A _III Semana de História_ do campus dos Malês será um **sucesso**.
```

A _III Semana de História_ do campus dos Malês será um **sucesso**.

---

### Blocos de citação

Para inserir um bloco de destaque para uma citação é só incluir `>` no início do parágrafo:

```
>Eu sou uma citação bonita de um texto qualquer.
```

>Eu sou uma citação bonita de um texto qualquer.

---

### Tabelas

É possível inserir tabelas separando as colunas com `|` e hífens para demarcar a linha de títulos.

Por exemplo:

```
| Coluna 1 | Coluna 2 | Coluna 3 |
| -------- | --------- | -------- |
| Linha 1, coluna 1 | Linha 1, coluna 2 | Linha 1, coluna 3|
| Linha 2, coluna 1 | Linha 2, coluna 2 | Linha 2, coluna 3|
| Linha 3, coluna 1 | Linha 3, coluna 2 | Linha 3, coluna 3|
```

---

Isso é renderizado como:

| Coluna 1 | Coluna 2 | Coluna 3 |
| -------- | --------- | -------- |
| Linha 1, coluna 1 | Linha 1, coluna 2 | Linha 1, coluna 3|
| Linha 2, coluna 1 | Linha 2, coluna 2 | Linha 2, coluna 3|
| Linha 3, coluna 1 | Linha 3, coluna 2 | Linha 3, coluna 3|

---

É possível definir o alinhamento da coluna incluíndo `:` na linha do cabeçalho:

```
| Alinhado à esquerda | Centralizado | Alinhado à direita |
| :-------- | :-------: | --------: |
| Maçãs | Vermelho | 5000 |
| Bananas | Amarelo| 75 |
```

---

| Alinhado à esquerda | Centralizado | Alinhado à direita |
| :-------- | :-------: | --------: |
| Maçãs | Vermelho | 5000 |
| Bananas | Amarelo| 75 |

---

### Linhas horizontais

Para separar seu documento e criar quebra de sessões, é possível inserir linhas horizontais utilizando `---` ou `***`

---

### Imagens e gifs

Para inserir imagen basta escrever o seguinte: `![título da imagem](caminho para a imagem em seu computador ou link para a imagem online)`

---

Imagem com caminho em meu computador:

![unilab](imgs/unilab.png)

---

Imagem com url:

![logo hist](https://cclhm0057.netlify.app/favicon/logohist.png)

OBS: Se vc pretende configurar mais elementos de sua imagem, como tamanho, alinhamento, legenda, será preciso utilizar `html`. Veremos algumas dicas assim abaixo.

---

### Links

Acrescentar links no documento é bem simples e segue padrão similar à inserção de imagens. Basta colocar o texto entre colchetes e o link entre parênteses na sequência `[]()`:

`[Introdução ao Markdown](https://programminghistorian.org/pt/licoes/introducao-ao-markdown)`

Isso renderiza assim:

[Introdução ao Markdown](https://programminghistorian.org/pt/licoes/introducao-ao-markdown)

---

### Códigos

É possível escrever blocos de código utilizando três acentos graves para abrir e fechar  bloco:

```
python
print('Olá, mundo!')
```

---

Ou ainda, escrever o código em linha usando um acento grave abrindo e fechando

`sudo apt install pandoc`

---

### Listas

É possível incluir listas ordenadas e não ordenadas

A lista ordenada é criada inserindo `-` ou `*` no início de cada linha. 

 ```
 Lista não ordenada
 
- ul
	- ul
- ul
- ul
 ```

---

Renderiza como:

- ul
	- ul
- ul
- ul

---

Listas ordenadas são criadas numerando cada linha e colocando um `.` após cada número:

```
Lista ordenada

1. od
2. od
	1. od
3. od
4. od
```

---

Renderiza como:

Lista ordenada

1. od
2. od
	1. od
3. od
4. od

---

### HTML

O Markdown possui limitações  e ainda não é um formato amplamente aceito no meio acadêmico. Muitos recursos de editores de texto como Word, LibreOffice não estão disponíveis em Markdown.

Entretanto, é possível inserir mais opções utilizando um pouco de html em seu documento.

---

Ex 1: Tamanho de uma imagem

```
<img src="https://media.giphy.com/media/nVTa8D8zJUc2A/source.gif" alt="seriously" style="zoom:100%;" />
```

<img src="https://media.giphy.com/media/nVTa8D8zJUc2A/source.gif" alt="seriously" style="zoom:100%;" />

---

<img src="https://media.giphy.com/media/nVTa8D8zJUc2A/source.gif" alt="seriously" style="zoom:70%;" />

---

Ex 2: Alinhamento da imagem

<img src="https://media.giphy.com/media/nVTa8D8zJUc2A/source.gif" alt="seriously" style="zoom:50%;"  align="left" />

---

<img src="https://media.giphy.com/media/nVTa8D8zJUc2A/source.gif" alt="seriously" style="zoom:50%;"  align="right" />

---

### Editores de markdown

Escrever o texto direto num editor de texto simples, sem visualizar o resultado final instantaneamente, pode ser um desafio no início. 

Entretanto, exixtem vários editores de markdown que facilitam muito sua vida e ainda possuem vários "sabores" [*flavours*] ou temas para trabalhar.

---

#### Apps 

- [Typora](https://typora.io/)
- [Mark Text](https://marktext.app/)
- [Apostrophe](https://gitlab.gnome.org/World/apostrophe)

#### On-line

- [Notion](https://www.notion.so)
- [HackMd](https://hackmd.io)

---

## Avançado

### Exportando e colocando online.

- HTML e suas vantagens para aulas online

### Slides, blogs e livros

- RMarkdow e variações:
  - [RMarkdown](https://beatrizmilz.com/talk/2020-rmarkdown-geocast/)
  - [Xaringan](https://beatrizmilz.github.io/IME-27-08-2019/#1)
  - Bookdown e Blogdown
- Reveal.js

### PDF e artigos científicos

- [Pandoc](https://osf.io/ceb4a/)

### Deploy

- [Netlify](https://app.netlify.com/drop): Exportar como HTML para uma pasta e renomear como index.html. A pasta deve conter tb os demais elementos.
- [Github](https://github.com/): criar uma conta, criar repositório com o arquivo `.md` e outros elmentos (imagens, gifs, etc). Publicar com [GitHub Pages](https://pages.github.com/)

---

## Contatos

1. E-mails

  	- profericbrasil@unilab.edu.br
  	- ericbrasiln@protonmail.com
2. Twitter: <a href="https://twitter.com/ericbrasiln" target="_blank">@ericbrasiln</a>
3. Instagram: <a href="https://www.instagram.com/ericbrasiln/" target="_blank">ericbrasiln</a>
4. Site pessoal: <a href="https://ericbrasiln.github.io/" target="_blank"> ericbrasiln.github.io</a>
5. Github: <a href= "https://github.com/ericbrasiln/" target="_blank">ericbrasiln</a>
6. [Lattes](http://lattes.cnpq.br/6853705640900524)
7. [Orcid](https://orcid.org/0000-0001-5067-8475)
8. [ResearchGate](https://www.researchgate.net/profile/Eric_Brasil)
9. [Academia.edu](https://unilab.academia.edu/EricBrasil)
10. [YouTube](https://www.youtube.com/channel/UC-tuyLIm7Ww_TDjKdHdnaAg)
---

## Agradecimentos

Obrigado pela paciência e participação.

<img src="https://media.giphy.com/media/AcfTF7tyikWyroP0x7/source.gif" alt="baby yoda" style="zoom:50%;" />

Viva o Sus!
