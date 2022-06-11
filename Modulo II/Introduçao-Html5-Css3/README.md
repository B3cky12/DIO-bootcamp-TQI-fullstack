# Introdução a Html5 e Css3

###### Iniciado: June 7, 2022 11:53 AM

###### Completo: Yes

###### Teacher: [Lucas Vilaboim](https://github.com/vilaboim)

###### [Link da aula](https://web.dio.me/course/introducao-criacao-de-websites-com-html5-e-css3/learning/462f831d-5fdf-485e-bf07-1d391eb94ac8?back=/track/tqi-fullstack-developer&tab=path)

###### Tecnologia: CSS3, HTML5

###### Requisitos: um editor de código e um navegador.

# Html5

## Estrutura básica

O HTML foi criado em 91, por Tim Berners-Lee e de lá até hoje surgiram 5 versões. A atual e mais usada é o HTML5, lançada em 2014.

A base do HTML é o elemento, composto pela tag de abertura, possíveis atributos, o conteúdo e a tag de fechamento. O documento html5 é criado com uma estrutura básica:

```html
<!DOCTYPE html>
<html>
  <head>
    <meta />
    <title></title>
  </head>
  <body></body>
</html>
```

### Exercício 1:

```html
<!DOCTYPE html>
<html>
  <head>
    <meta chaset="utf-8" />
    <title>Ellen Rebeca</title>
  </head>
  <body>
    Ellen Rebeca
  </body>
</html>
```

// Comentário pessoal: Não explicou como o código foi do editor pro navegador. Eu sei pq já vi em outros lugares, mas iniciante cru vai ficar perdido nessa . “utf-8 pq eh a mais comum”? Isso pareceu muito simplificado, eu tenho certeza que existe uma explicação mais técnica.

// Edit: utf-8 é o mais comum do tipo de codificação de caracteres mais abrangente e complexa - o código multibyte - conseguindo representar unicode e ASCII. Por conta da variabilidade do número de bytes usados por cada caractere, a decodificação seria um um problema, mas o utf-8 foi criado de um jeito que os primeiros bits de um código já informam quantos bytes o código ocupa. Legal, né?

## Semântica

Antes do Html5 a tag mais utilizada era a div, não somente porque ela eh muito útil, mas porque não tinha muitas tags específicas como o header, o footer, uma section, o article, o aside, etc… . O que se fazia eram muitas e muitas divs, uma dentro da outra, e uma classe pra cada, no final ficava uma bagunça. No Html5 foram criadas novas tags pra ajudar a especificar melhor a estrutura da página sem sobrecarregar o número de divs.

### Exercício 2:

```html
<!DOCTYPE html>
<html>
	<head>
		<meta chaset="utf-8">
		<title>Ellen Rebeca</title>
	</head>
	<body>
		<header>
			<h1>Ellen Rebeca</h1>
		</header>
		<section>
			<header>
				<h2>Posts</h2>
			</header>
			<article>
				<header>
					<h3>Post #1</h3>
				</header>
			</article>
		<section>
		<footer></footer>
	</body>
</html>
```

## Textos e Links

### Tags para textos

Os elementos h1 ao h6 são importantes para identificar os títulos presentes em uma página, mas pra textos maiores e mais densos é mais útil usar a tag de parágrafo, o elemento p.

### Tags para links

O elemento muito interessante para interligar é o a, que é uma âncora, que aponta para outras páginas. Dois dos atributos mais importantes da tag a é a referência href e o modo target.

### Exercício 3:

```html
<!DOCTYPE html>
<html>
	<head>
		<meta chaset="utf-8">
		<title>Ellen Rebeca</title>
	</head>
	<body>
		<header>
			<h1>Ellen Rebeca</h1>
		</header>
		<section>
			<header>
				<h2>Posts</h2>
			</header>
			<article>
				<header>
					<h3>Post #1</h3>
				</header>
				<p>
				Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nulla facilisis tempus ornare. Donec id accumsan eros, non mollis mi. Interdum et malesuada fames ac ante ipsum primis in faucibus. Proin ut sodales ligula. Donec malesuada at velit nec condimentum. Donec nec consequat turpis. Maecenas sed urna at <a href="mailto:ellen.aguiar@ufpe.br">massa iaculis</a> pulvinar.
				</p>
				<p>
				Ut finibus elit nunc, pellentesque auctor <a href="https://www.linkedin.com/in/ellen-rebeca-aguiar/" target="_blank">Ellen</a> tellus ullamcorper et. Cras odio orci, maximus sollicitudin nisl nec, porttitor eleifend dui. Duis vitae dolor sed magna tempor aliquet id ut nisl. Phasellus vel blandit nunc. Praesent vitae tempus augue, ac mattis ex. Aliquam at eros quis dui volutpat tempor. Aenean nisl <a href="tel:9999999">leoa</a>, laoreet at elementum eu, rutrum ut sapien.
				</p>
			</article>
		<section>
		<footer></footer>
	</body>
</html>
```

## Imagem

Imagens falam mais que mil Lorem ipsums, e pra mostra-las usamos o elemento img, detalhe: não tem tag de fechamento. Dois atributos importantes da tag img é src e alt, o primeiro é obrigatótio colocar pq ele guarda o caminho da imagem, e o segundo é uma descrição do conteúdo da imagem, que é mostrada quando ocorre algum problema e a imagem não é mostrada ou pra quando o usuário do outro lado tem alguma deficiência e usa um leitor específico.

### Exercício 4:

```html
<!DOCTYPE html>
<html>
	<head>
		<meta chaset="utf-8">
		<title>Ellen Rebeca</title>
	</head>
	<body>
		<header>
			<img src="https://picrew.me/shareImg/org/202206/338224_R6OCzYH0.png" alt="Ilustração de uma Ellen Rebeca corada e segurando um bubble tea" >
			<h1>Ellen Rebeca</h1>
		</header>
		<section>
			<header>
				<h2>Posts</h2>
			</header>
			<article>
				<header>
					<h3>Post #1</h3>
				</header>
				<p>
				Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nulla facilisis tempus ornare. Donec id accumsan eros, non mollis mi. Interdum et malesuada fames ac ante ipsum primis in faucibus. Proin ut sodales ligula. Donec malesuada at velit nec condimentum. Donec nec consequat turpis. Maecenas sed urna at <a href="mailto:ellen.aguiar@ufpe.br">massa iaculis</a> pulvinar.
				</p>
				<p>
				Ut finibus elit nunc, pellentesque auctor <a href="https://www.linkedin.com/in/ellen-rebeca-aguiar/" target="_blank">Ellen</a> tellus ullamcorper et. Cras odio orci, maximus sollicitudin nisl nec, porttitor eleifend dui. Duis vitae dolor sed magna tempor aliquet id ut nisl. Phasellus vel blandit nunc. Praesent vitae tempus augue, ac mattis ex. Aliquam at eros quis dui volutpat tempor. Aenean nisl <a href="tel:9999999">leoa</a>, laoreet at elementum eu, rutrum ut sapien.
				</p>
			</article>
		<section>
		<footer></footer>
	</body>
</html>
```

link útil para otimizar imagens: [TinyPNG – Compress WebP, PNG and JPEG images intelligently](https://tinypng.com/)

## Listas

Listas servem pra agrupar uma seleção de itens, e exitem dois tipos:

- a lista ordenada, elemento ol
- a lista não ordenada, elemento ul

E no html5 também tem o elemento li que representa cada item da lista.

### Exercício 5:

```html
<!DOCTYPE html>
<html>
	<head>
		<meta chaset="utf-8">
		<title>Ellen Rebeca</title>
	</head>
	<body>
		<header>
			<img src="https://picrew.me/shareImg/org/202206/338224_R6OCzYH0.png" alt="Ilustração de uma Ellen Rebeca corada e segurando um bubble tea" >
			<h1>Ellen Rebeca</h1>
		</header>
		<section>
			<header>
				<h2>Posts</h2>
			</header>
			<article>
				<header>
					<h3>Post #1</h3>
				</header>
				<p>
				Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nulla facilisis tempus ornare. Donec id accumsan eros, non mollis mi. Interdum et malesuada fames ac ante ipsum primis in faucibus. Proin ut sodales ligula. Donec malesuada at velit nec condimentum. Donec nec consequat turpis. Maecenas sed urna at <a href="mailto:ellen.aguiar@ufpe.br">massa iaculis</a> pulvinar.
				</p>
				<p>
				Ut finibus elit nunc, pellentesque auctor <a href="https://www.linkedin.com/in/ellen-rebeca-aguiar/" target="_blank">Ellen</a> tellus ullamcorper et. Cras odio orci, maximus sollicitudin nisl nec, porttitor eleifend dui. Duis vitae dolor sed magna tempor aliquet id ut nisl. Phasellus vel blandit nunc. Praesent vitae tempus augue, ac mattis ex. Aliquam at eros quis dui volutpat tempor. Aenean nisl <a href="tel:9999999">leoa</a>, laoreet at elementum eu, rutrum ut sapien.
				</p>
			</article>
		<section>
		<footer>
			<ul>
        <li>
          <a href="mailto:ellen.rebeca10@gmail.com" target="_blank" >ellen.rebeca10@gmail.com</a>
        </li>
        <li>
          <a href="https://www.linkedin.com/in/ellen-rebeca-aguiar/" target="_blank" >LinkedIn</a>
        </li>
        <li>
          <a href="https://github.com/B3cky12" target="_blank" >Github</a>
        </li>
      </ul>
		</footer>
	</body>
</html>
```

# Css3

O css é uma linguagem de estilo, criada para poder formatar páginas, criando regras de estilo pra formatar elementos html. Uma regra css é formada por um ou mais seletores e uma ou mais declarações, as declarações atuam mudanças nas propriedades dos seletores.

Em css temos identificadores, os id, e classes, as class, e eles servem como ganchos do css no html, mas pra propósitos específicos distintos. Por exemplo, cada id só pode ser usado em um elemento na página, e as class podem ser reutilizadas várias vezes em vários elementos. Outra coisa é que as classes são escritas no css com um ponto e as ids são com uma #.

```html
<!DOCTYPE html>
<html>
	<head>
		<meta chaset="utf-8">
		<title>Ellen Rebeca</title>
    <link rel="stylesheet" href="style.css">
	</head>
	<body>
		<header>
			<img src="https://picrew.me/shareImg/org/202206/338224_R6OCzYH0.png" alt="Ilustração de uma Ellen Rebeca corada e segurando um bubble tea" >
			<h1 id="title" >Ellen Rebeca</h1>
		</header>
		<section>
			<header>
				<h2 class="subtitle" >Posts</h2>
			</header>
			<article>
				<header>
					<h3 class="post-title" >Post #1</h3>
				</header>
				<p>
				Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nulla facilisis tempus ornare. Donec id accumsan eros, non mollis mi. Interdum et malesuada fames ac ante ipsum primis in faucibus. Proin ut sodales ligula. Donec malesuada at velit nec condimentum. Donec nec consequat turpis. Maecenas sed urna at <a href="mailto:ellen.aguiar@ufpe.br">massa iaculis</a> pulvinar.
				</p>
				<p>
				Ut finibus elit nunc, pellentesque auctor <a href="https://www.linkedin.com/in/ellen-rebeca-aguiar/" target="_blank">Ellen</a> tellus ullamcorper et. Cras odio orci, maximus sollicitudin nisl nec, porttitor eleifend dui. Duis vitae dolor sed magna tempor aliquet id ut nisl. Phasellus vel blandit nunc. Praesent vitae tempus augue, ac mattis ex. Aliquam at eros quis dui volutpat tempor. Aenean nisl <a href="tel:9999999">leoa</a>, laoreet at elementum eu, rutrum ut sapien.
				</p>
			</article>
		<section>
		<footer>
			<ul>
        <li>
          <a href="mailto:ellen.rebeca10@gmail.com" target="_blank" >ellen.rebeca10@gmail.com</a>
        </li>
        <li>
          <a href="https://www.linkedin.com/in/ellen-rebeca-aguiar/" target="_blank" >LinkedIn</a>
        </li>
        <li>
          <a href="https://github.com/B3cky12" target="_blank" >Github</a>
        </li>
      </ul>
		</footer>
	</body>
</html>
```

```css
#title,
.subtitle,
.post-title {
  color: pink;
  background-color: brown;
}

.post-title {
  font-size: 16px;
  font-style: italic;
}
```

## Conceitos básicos

Podemos visualizar as páginas web como caixas cheias de caixas, e cada coisinha diferente dentro de uma caixa. Isso se chama de box model, ou modelo de caixa, composto de margin, border, padding e content, nessa ordem de mais externo pra mais interno.

```html
<!DOCTYPE html>
<html>

<head>
    <meta charset="utf-8">
    <title>Ellen Rebeca</title>
    <link rel="stylesheet" href="style.css">
</head>

<body>
    <header>
        <img src="https://picrew.me/shareImg/org/202206/338224_R6OCzYH0.png" alt="Ilustração de uma Ellen Rebeca corada e segurando um bubble tea" id="bubble-t">
        <h1 id="title">Ellen Rebeca</h1>
    </header>
    <section>
        <header>
            <h2 class="subtitle">Posts</h2>
        </header>
        <article class="post">
            <header>
                <h3 class="post-title">Post #1</h3>
            </header>
            <p>
                Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nulla facilisis tempus ornare. Donec id accumsan eros, non mollis mi. Interdum et malesuada fames ac ante ipsum primis in faucibus. Proin ut sodales ligula. Donec malesuada at velit nec condimentum.
                Donec nec consequat turpis. Maecenas sed urna at <a href="mailto:ellen.aguiar@ufpe.br">massa iaculis</a> pulvinar.
            </p>
            <p>
                Ut finibus elit nunc, pellentesque auctor <a href="https://www.linkedin.com/in/ellen-rebeca-aguiar/" target="_blank">Ellen</a> tellus ullamcorper et. Cras odio orci, maximus sollicitudin nisl nec, porttitor eleifend dui. Duis vitae dolor
                sed magna tempor aliquet id ut nisl. Phasellus vel blandit nunc. Praesent vitae tempus augue, ac mattis ex. Aliquam at eros quis dui volutpat tempor. Aenean nisl <a href="tel:9999999">leoa</a>, laoreet at elementum eu, rutrum ut sapien.
            </p>
        </article>
        <section>
            <footer>
                <ul>
                    <li>
                        <a href="mailto:ellen.rebeca10@gmail.com" target="_blank">ellen.rebeca10@gmail.com</a>
                    </li>
                    <li>
                        <a href="https://www.linkedin.com/in/ellen-rebeca-aguiar/" target="_blank">LinkedIn</a>
                    </li>
                    <li>
                        <a href="https://github.com/B3cky12" target="_blank">Github</a>
                    </li>
                </ul>
            </footer>
</body>

</html>
```

```css
body {
  background: rgb(201, 68, 68);
}

#title,
.subtitle,
.post-title {
  color: rgb(252, 122, 155);
}

#bubble-t {
  height: 150px;
}

.post-title {
  font-size: 16px;
  font-style: italic;
}

.post {
  background-color: #ffffff;
  padding: 10px;
  border: 3px solid black;
  margin: 10px;
}
```

## Estilizando elementos

Ao definir os tamanhos que queremos para as caixas, podemos querer cada lado de um valor diferente, nesse caso é só lembrar de um caminho clockwise na hora de escrever paddings e margins. Pra definir cores podemos usar o método rgb, #000000 ou o nome da cor em inglês. As bordas podem ser descritas em pixels, cms, mls, sólida, pontilhada, tracejada, etc… Border-radius é muito legal 🙂

```html
<!DOCTYPE html>
<html>

<head>
    <meta charset="utf-8">
    <title>Ellen Rebeca</title>
    <link rel="stylesheet" href="style.css">
</head>

<body>
    <header>
        <img src="https://picrew.me/shareImg/org/202206/338224_R6OCzYH0.png" alt="Ilustração de uma Ellen Rebeca corada e segurando um bubble tea" id="bubble-t">
        <h1 id="title">Ellen Rebeca</h1>
    </header>
    <section>
        <header>
            <h2 class="subtitle">Posts</h2>
        </header>
        <article class="post">
            <header>
                <h3 class="post-title">Post #1</h3>
                <img src="https://i.pinimg.com/originals/9b/ee/9c/9bee9ccfece6c7750dca6fc3708b5252.gif" alt="clear skies gif" class="post-image">
            </header>
            <p class="post-content">
                Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nulla facilisis tempus ornare. Donec id accumsan eros, non mollis mi. Interdum et malesuada fames ac ante ipsum primis in faucibus. Proin ut sodales ligula. Donec malesuada at velit nec condimentum.
                Donec nec consequat turpis. Maecenas sed urna at <a href="mailto:ellen.aguiar@ufpe.br">massa iaculis</a> pulvinar.
            </p>
            <p class="post-content">
                Ut finibus elit nunc, pellentesque auctor <a href="https://www.linkedin.com/in/ellen-rebeca-aguiar/" target="_blank">Ellen</a> tellus ullamcorper et. Cras odio orci, maximus sollicitudin nisl nec, porttitor eleifend dui. Duis vitae dolor
                sed magna tempor aliquet id ut nisl. Phasellus vel blandit nunc. Praesent vitae tempus augue, ac mattis ex. Aliquam at eros quis dui volutpat tempor. Aenean nisl <a href="tel:9999999">leoa</a>, laoreet at elementum eu, rutrum ut sapien.
            </p>
        </article>
        <section>
            <footer>
                <ul>
                    <li>
                        <a href="mailto:ellen.rebeca10@gmail.com" target="_blank">ellen.rebeca10@gmail.com</a>
                    </li>
                    <li>
                        <a href="https://www.linkedin.com/in/ellen-rebeca-aguiar/" target="_blank">LinkedIn</a>
                    </li>
                    <li>
                        <a href="https://github.com/B3cky12" target="_blank">Github</a>
                    </li>
                </ul>
            </footer>
</body>

</html>
```

```css
body {
  background: rgb(253, 150, 150);
}

#title,
.subtitle,
.post-title {
  color: rgb(61, 7, 21);
}

#bubble-t {
  height: 150px;
  border-radius: 15px;
  border: 2px rgb(61, 7, 21);
}

.post-title {
  font-size: 16px;
  font-style: italic;
  margin: 0;
  margin-bottom: 15px;
}

.post-image {
  margin: 0 0 15px 0;
  border-radius: 2px;
  padding: auto;
}

.post {
  background-color: #f7f7f7;
  padding: 15px;
  border: 3px solid rgb(61, 7, 21);
  border-radius: 5px;
  margin: 0 0 15px 0;
}

.post-content {
  margin: 0;
  margin-bottom: 15px;
}
```

## Estilizando textos

Font-family é usada para definir a fonte base do texto. Size é tamanho, style é aparência, weight é o peso, transform alterna o texto entre maiúsculo e minúsculo, decoration consegue dar destaque ao texto, etc…

### Exercício 6:

```html
<!DOCTYPE html>
<html>

<head>
    <meta charset="utf-8">
    <title>Ellen Rebeca</title>
    <link rel="stylesheet" href="style.css">
</head>

<body>
    <header>
        <img src="https://picrew.me/shareImg/org/202206/338224_R6OCzYH0.png" alt="Ilustração de uma Ellen Rebeca corada e segurando um bubble tea" id="bubble-t">
        <h1 id="title">Ellen Rebeca</h1>
    </header>
    <section>
        <header>
            <h2 class="subtitle">Posts</h2>
        </header>
        <article class="post">
            <header>
                <h3 class="post-title">Post #1</h3>
                <img src="https://i.pinimg.com/originals/9b/ee/9c/9bee9ccfece6c7750dca6fc3708b5252.gif" alt="clear skies gif" class="post-image">
            </header>
            <p class="post-content">
                Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nulla facilisis tempus ornare. Donec id accumsan eros, non mollis mi. Interdum et malesuada fames ac ante ipsum primis in faucibus. Proin ut sodales ligula. Donec malesuada at velit nec condimentum.
                Donec nec consequat turpis. Maecenas sed urna at <a href="mailto:ellen.aguiar@ufpe.br">massa iaculis</a> pulvinar.
            </p>
            <p class="post-content">
                Ut finibus elit nunc, pellentesque auctor <a href="https://www.linkedin.com/in/ellen-rebeca-aguiar/" target="_blank">Ellen</a> tellus ullamcorper et. Cras odio orci, maximus sollicitudin nisl nec, porttitor eleifend dui. Duis vitae dolor
                sed magna tempor aliquet id ut nisl. Phasellus vel blandit nunc. Praesent vitae tempus augue, ac mattis ex. Aliquam at eros quis dui volutpat tempor. Aenean nisl <a href="tel:9999999">leoa</a>, laoreet at elementum eu, rutrum ut sapien.
            </p>
        </article>
        <section>
            <footer>
                <ul>
                    <li>
                        <a href="mailto:ellen.rebeca10@gmail.com" target="_blank">ellen.rebeca10@gmail.com</a>
                    </li>
                    <li>
                        <a href="https://www.linkedin.com/in/ellen-rebeca-aguiar/" target="_blank">LinkedIn</a>
                    </li>
                    <li>
                        <a href="https://github.com/B3cky12" target="_blank">Github</a>
                    </li>
                </ul>
            </footer>
</body>

</html>
```

```css
body {
  background: rgb(253, 150, 150);
  font-family: Arial, Helvetica, sans-serif;
}

#title,
.subtitle,
.post-title {
  color: rgb(61, 7, 21);
}

#title {
  font-size: 50px;
  text-transform: uppercase;
}

a {
  text-decoration: underline;
  color: crimson;
}

#bubble-t {
  height: 150px;
  border-radius: 15px;
  border: 2px rgb(61, 7, 21);
}

.post-title {
  font-size: 16px;
  font-style: italic;
  margin: 0;
  margin-bottom: 15px;
}

.post-image {
  margin: 0 0 15px 0;
  border-radius: 2px;
  padding: auto;
}

.post {
  background-color: #f7f7f7;
  padding: 15px;
  border: 3px solid rgb(61, 7, 21);
  border-radius: 5px;
  margin: 0 0 15px 0;
}

.post-content {
  margin: 0;
  margin-bottom: 15px;
  text-transform: capitalize;
}
```

## Estilizando listas

Nas listas, podemos alterar os símbolos das não ordenadas ou o tipo de número das ordenadas.

// Edit: O vscode me lembrou pra colodar a lingua na tag html, 'pt-br' nesse caso.

### Exercício 7:

```html
<!DOCTYPE html>
<html lang="pt-br">

<head>
    <meta charset="utf-8">
    <title>Ellen Rebeca</title>
    <link rel="stylesheet" href="style.css">
</head>

<body>
    <header>
        <img src="https://picrew.me/shareImg/org/202206/338224_R6OCzYH0.png" alt="Ilustração de uma Ellen Rebeca corada e segurando um bubble tea" id="bubble-t">
        <h1 id="title">Ellen Rebeca</h1>
    </header>
    <section>
        <header>
            <h2 class="subtitle">Posts</h2>
        </header>
        <article class="post">
            <header>
                <h3 class="post-title">Post #1</h3>
                <img src="https://i.pinimg.com/originals/9b/ee/9c/9bee9ccfece6c7750dca6fc3708b5252.gif" alt="clear skies gif" class="post-image">
            </header>
            <p class="post-content">
                Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nulla facilisis tempus ornare. Donec id accumsan eros, non mollis mi. Interdum et malesuada fames ac ante ipsum primis in faucibus. Proin ut sodales ligula. Donec malesuada at velit nec condimentum.
                Donec nec consequat turpis. Maecenas sed urna at <a href="mailto:ellen.aguiar@ufpe.br">massa iaculis</a> pulvinar.
            </p>
            <p class="post-content">
                Ut finibus elit nunc, pellentesque auctor <a href="https://www.linkedin.com/in/ellen-rebeca-aguiar/" target="_blank">Ellen</a> tellus ullamcorper et. Cras odio orci, maximus sollicitudin nisl nec, porttitor eleifend dui. Duis vitae dolor
                sed magna tempor aliquet id ut nisl. Phasellus vel blandit nunc. Praesent vitae tempus augue, ac mattis ex. Aliquam at eros quis dui volutpat tempor. Aenean nisl <a href="tel:9999999">leoa</a>, laoreet at elementum eu, rutrum ut sapien.
            </p>
        </article>
        <section>
            <footer>
                <ul class="contacts-list">
                    <li>
                        <a href="mailto:ellen.rebeca10@gmail.com" target="_blank">ellen.rebeca10@gmail.com</a>
                    </li>
                    <li>
                        <a href="https://www.linkedin.com/in/ellen-rebeca-aguiar/" target="_blank">LinkedIn</a>
                    </li>
                    <li>
                        <a href="https://github.com/B3cky12" target="_blank">Github</a>
                    </li>
                </ul>
            </footer>
</body>

</html>
```

```css
body {
  background: rgb(253, 150, 150);
  font-family: Arial, Helvetica, sans-serif;
}

#title,
.subtitle,
.post-title {
  color: rgb(61, 7, 21);
}

#title {
  font-size: 50px;
  text-transform: uppercase;
}

a {
  text-decoration: underline;
  color: crimson;
}

#bubble-t {
  height: 150px;
  border-radius: 15px;
  border: 2px rgb(61, 7, 21);
}

.post-title {
  font-size: 16px;
  font-style: italic;
  margin: 0;
  margin-bottom: 15px;
}

.post-image {
  margin: 0 0 15px 0;
  border-radius: 2px;
  padding: auto;
}

.post {
  background-color: #f7f7f7;
  padding: 15px;
  border: 3px solid rgb(61, 7, 21);
  border-radius: 5px;
  margin: 0 0 15px 0;
}

.post-content {
  margin: 0;
  margin-bottom: 15px;
  text-transform: capitalize;
}

.contacts-list {
  list-style-type: none;
  margin: 0;
  padding-left: 15px;
}

.contacts-list li a {
  color: rgb(61, 7, 21);
}
```

## Propriedades de dimensões e alinhamento

Para ajudar a posicionar nossas caixas na página, precisamos entender bem as dimensões que queremos para os itens. Podemos usar os atributos width, height e text-align.

### Exercício 8:

```html
<!DOCTYPE html>
<html lang="pt-br">

<head>
    <meta charset="utf-8">
    <title>Ellen Rebeca</title>
    <link rel="stylesheet" href="style.css">
</head>

<body>
    <header>
        <img src="https://picrew.me/shareImg/org/202206/338224_R6OCzYH0.png" alt="Ilustração de uma Ellen Rebeca corada e segurando um bubble tea" id="bubble-t">
        <h1 id="title">Ellen Rebeca</h1>
    </header>
    <section>
        <header>
            <h2 class="subtitle">Posts</h2>
        </header>
        <article class="post">
            <header>
                <h3 class="post-title">Post #1</h3>
                <img src="https://i.pinimg.com/originals/9b/ee/9c/9bee9ccfece6c7750dca6fc3708b5252.gif" alt="clear skies gif" class="post-image">
            </header>
            <p class="post-content">
                Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nulla facilisis tempus ornare. Donec id accumsan eros, non mollis mi. Interdum et malesuada fames ac ante ipsum primis in faucibus. Proin ut sodales ligula. Donec malesuada at velit nec condimentum.
                Donec nec consequat turpis. Maecenas sed urna at <a href="mailto:ellen.aguiar@ufpe.br">massa iaculis</a> pulvinar.
            </p>
            <p class="post-content">
                Ut finibus elit nunc, pellentesque auctor <a href="https://www.linkedin.com/in/ellen-rebeca-aguiar/" target="_blank">Ellen</a> tellus ullamcorper et. Cras odio orci, maximus sollicitudin nisl nec, porttitor eleifend dui. Duis vitae dolor
                sed magna tempor aliquet id ut nisl. Phasellus vel blandit nunc. Praesent vitae tempus augue, ac mattis ex. Aliquam at eros quis dui volutpat tempor. Aenean nisl <a href="tel:9999999">leoa</a>, laoreet at elementum eu, rutrum ut sapien.
            </p>
        </article>
        <section>
            <footer>
                <ul class="contacts-list">
                    <li>
                        <a href="mailto:ellen.rebeca10@gmail.com" target="_blank">ellen.rebeca10@gmail.com</a>
                    </li>
                    <li>
                        <a href="https://www.linkedin.com/in/ellen-rebeca-aguiar/" target="_blank">LinkedIn</a>
                    </li>
                    <li>
                        <a href="https://github.com/B3cky12" target="_blank">Github</a>
                    </li>
                </ul>
            </footer>
</body>

</html>
```

```css
body {
  background: rgb(253, 150, 150);
  font-family: Arial, Helvetica, sans-serif;
  max-width: 1000px;
  margin: auto;
}

#title,
.subtitle,
.post-title {
  color: rgb(61, 7, 21);
}

#title {
  font-size: 50px;
  text-transform: uppercase;
}

a {
  text-decoration: underline;
  color: crimson;
}

#bubble-t {
  height: 150px;
  border-radius: 15px;
  border: 2px rgb(61, 7, 21);
  margin-top: 15px;
}

.post-title {
  font-size: 16px;
  font-style: italic;
  margin: 0;
  margin-bottom: 15px;
}

.post-image {
  margin: 0 0 15px 0;
  border-radius: 2px;
  padding: auto;
  width: 100%;
}

.post {
  background-color: #f7f7f7;
  padding: 15px;
  border: 3px solid rgb(61, 7, 21);
  border-radius: 5px;
  margin: 0 0 15px 0;
}

.post-content {
  margin: 0;
  margin-bottom: 15px;
  text-transform: capitalize;
  text-align: justify;
}

.contacts-list {
  list-style-type: none;
  margin: 0;
  padding-left: 15px;
}

.contacts-list li a {
  color: rgb(61, 7, 21);
}
```
