# Introdução ao Git e ao GitHub

Certificard: Introduc%CC%A7a%CC%83o%20ao%20Git%20e%20ao%20GitHub%207a2f263b4edc4226b5de791a0b443fc5/15F8929C.pdf
Completo: Yes
Iniciado: May 31, 2022 2:24 PM
Materials: https://web.dio.me/course/introducao-ao-git-e-ao-github/learning/75b9fe49-6ed4-4480-83a7-7e37fc356aa9?back=/track/tqi-fullstack-developer&tab=undefined&moduleId=undefined, https://www.markdownguide.org/
Módulo: I
Teacher: Otávio Reis, perkles.
Tecnologia: Git, GitHub, Markdown

# Entendendo o que é Git e a sua importância

Git é um sistema de versionamento de código distribuído, de controle de versão de código, criado quando Linus Torvalds estava descontente com as linguagens de versionamento na época que ele e sua equipe (ao redor do mundo) estavam construindo o Linux.

A necessidade de um software de versionamento de código bom, e complexo o suficiente pra aguentar os muitos colaboradores do linux, de todos os lugares do mundo, alterando um mesmo doc.

Empresas foram surgindo pra guardar todas essas versões de código de um mesmo projeto, e a mais utilizada e conhecida é o GitHub, um repositório online opensource, mas existem outros tbm.

Pontos bacanas que se ganha em aprender git e github:

- Controle de versão
- Armazenamento em nuvem
- Trabalho em equipe
- Melhorar seu código
- Reconhecimento

# Comandos básicos para um bom desempenho no terminal

O Git é um CLI e não um GUI, então ele não tem uma interface gráfica, o foco dele é nas linhas de comando. Hoje em dia tem alguns programas que automatizam isso, pra quem preferir.

## Comandos básicos e Sistemas

| Função | Windows | Linux |
| --- | --- | --- |
| Mudar de pastas | - cd <nome_da_pasta> - cd .. | - cd <nome_da_pasta> - cd .. |
| Listar as pastas | - dir | - ld |
| Criar pastas / arquivos | - mkdir | - mkdir |
| Deletar arquivos / pasta | - del / rmdir | - rm -rf |
| Limpar o terminal | - cls | - clear |
| Printa no terminal | - echo | - echo |

TAB completa os nomes de forma inteligente;

ctrl + L limpa o terminal tbm, maas no linux;

o - cd / leva pra a pasta C raíz;

o - cd .. volta uma pasta;

“>”é um redirecionador de curso;

no windows, pra remover  de forma simples o diretório tbm eh - rmdir /S /Q, no linux eh - rm -rf;

 - pwd mostra o caminho;

# Entendendo como o Git funciona por baixo dos panos

## SHA1

É um algoritmo de criptação, projetado pela NSA como um SHA (Secure Hash Algorithm), é um conjunto de funções hash criptográficas. A encriptação gera um conjunto de caracteres identificador de 40 dígitos, e isso é uma chave muito eficiente.

```
echo “ola mundo” | openssl sha1

echo hello > texto.txt

openssl sha1 texto.txt
```

## Objetos fundamentais

### Blobs, trees e commits.

Os arquivos ficam armazenados dentro dos blobs, que contém metadados, identificando o tipo de arquivo, o tamanho, um \0 e o conteúdo do arquivo e o sha1. O blob é uma bolha pessoal pro arquivo. O blob é um objeto.

```
echo ‘conteudo’ | git hash-object -- stdin

echo -e ‘conteudo | openssl sha1

echo -e ‘blob 9\0conteudo’ | openssl sha1
```

As Trees armazenam Blobs, também contendo metadados, o tamanho, o \0, o sha1 e o nome do arquivo. A árvore vai ser responsável por toda a estrutura de onde vão estar os arquivos, onde estão localizados, podendo apontar para blobs ou outras árvores.

Se mudar um arquivo, seu sha vai mudar, o sha do blob que ele está vai mudar e o sha da tree onde o blob onde o arquivo está vai mudar. Tudo tá relacionado.

O commit é o objeto que vai juntar tudo. Ele aponta pra uma árvore, pro parente, pro autor, contém a mensagem e o timestamp do commit. E o commit tem um sha1, que vai ser o hash de toooooooooda aquela informação específica.

## Sistema distribuído e seguro

Depois de conhecer os blobs, as trees e os commits, percebemos o quanto que o git é distribuído e seguro. É extremamente difícil (impossível) de ser alterado maliciosamente, e as versões mais atuais de um código guarda o histórico dos primeiros passos do programa.

## Chaves SSH e Token

Pra deixar o GitHub mais seguro, o GitHub introduziu um método mais efetivo. Chaves SSH e Tokens 🙂

Chave SSH é uma forma de fazer uma conexão segura e encriptada. Ela é configurada uma vez, como uma assinatura pessoal do seu computador.

```
ssh-keygen -t ed25519 -C “seu_email@gmail.com”
```

enter enter enter

```
cat id_ed25519.pub
```

copia e usa a chave SSH pública no github

SSH agent: (pra cuidar das chaves)

```
eval $(ssh-agent -s)

ssh-add id_ed25519
```

enter

Token de acesso pessoal serve como uma senha, pra autenticação antiga. Você cria um token na sua conta do GitHub e copia e cola ele em um lugar seguro.

# Primeiros comandos com Git

- Iniciar o git
    - - git init
- Iniciar o versionamento
    - - git add
- Criar um commit
    - - git commit

<aside>
📎 No terminal, todo comando git leva o git na frente.

</aside>

flag -a mostra arquivos ocultos;

### Setando o email e name da autora:

```
git config --global --add user.email "ellen.rebeca10@gmail.com"

git config --global user.name B3cky12
```

### Adicionando um arquivo markdown:

Número de # diz o nível do texto;

```
echo strogonoff > strogonoff.md
```

//aí agora a gente vai precisar do VSCode

![Untitled](Introduc%CC%A7a%CC%83o%20ao%20Git%20e%20ao%20GitHub%207a2f263b4edc4226b5de791a0b443fc5/Untitled.png)

// dps volta pro git bash

![Untitled](Introduc%CC%A7a%CC%83o%20ao%20Git%20e%20ao%20GitHub%207a2f263b4edc4226b5de791a0b443fc5/Untitled%201.png)

23da246 é os primeiros caracteres do sha1 do commit;

# Ciclo de vida do git

O git init cria um repositório. 

Tracked arquivos são os que a gente sabe, que são rastreados pelo git, e os untracked são os que a gente não sabe. Dentre os tracked, temos os unmodified, modified e staged, e os nomes são auto-explicativos, menos o stage. O stage é onde ficam os arquivos que estão se preparando pra entrar em ação.

Quando usamos o git add no strogonoff.md, o arquivo tava untracked e foi direto pra staged. os unmodified são arquivos dentro do repositório e sem modificação, e aí quando muda o sha1, o git percebe e passa eles pra modified. Se rodar o git add de novo num arquivo modified, ele vai pra staged de novo. Se do nada a gente remove o arquivo, ele vai pra untracked.

Os arquivos dentro do staged estão esperando e se preparando pra um commit. O commit devolve todos aqueles arquivos pra unmodified. Então é um ciclo.

O github se torna um servidor, um repositório remoto, enquanto trabalhamos no ambiente de desenvolvimento, observando o working directory, o staging area e o local repository. Os arquivos ficam transitando entre o working directory e o staging area, mas quando fazemos um commit passamos os arquivos do staging area pra o local repository.

Tudo que está no local repository tem que estar commitado, pra que possamos passar do repositório local pro remoto, no nosso caso, o GitHub.

```
git status

mv <arquivo> ./pasta_onde_quer_colocar
```

git add * ou . adiciona todas as mudanças untracked pra staged. Isso ajuda.

# Trabalhando com GitHub

Facilita a conexão entre o github e o git bash se o email e o nome do usuário são os mesmos nos dois. Da pra verificar as configurações do git bash escrevendo:

 - git config --list

Aí, caso é preciso alterar algo nesses settings faz:

 - git config --global -- unset user.email

 - git config --global -- unset user.name

E pronto. Pra criar os novos, já vimos.

Cria o repositório remoto no github e pega o endereço dele, aí com pra apontar o remoto pro local escrevemos:

 - git remote add origin “EndereçoHttpsOuSsh”

E pra ver a lista podemos fazer:

 - git remote -v

Lembrando que pra fazer o push, o repositório local precisa estar on branch, tudo já commitado certinho. Mas pra dar o push, também precisamos indicar o branch remoto que é pra ir.

```
git branch -M main
git push -u origin main
```

Assim, se o objetivo é dar o push já no main branch. Olhando nos sha dos commit, podemos ver as mudanças acontecendo.

# Resolvendo conflitos no GitHub

Quando se ocorre um desencontro de duas edições diferentes do mesmo arquivo, dizemos que as versões estão em conflito. Pra resolver eh manual, e só depois fazer os push necessários. O github não toma a frente pra resolver os conflitos.