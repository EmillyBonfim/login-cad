## Página de Login e Cadastro
Nessa atividade nós criamos uma página de Login e Cadastro onde ao fazer login na página inicial ele nos direciona a página de cadastro, nele conseguimos cadastrar algo editar-lo e exclui-lo o.

## Explicações das funções e elementos em JavaScript

 * ``element``  É uma referência a um objeto ``Element``, ou null se um elemento com o ID especificado não estiver contido neste documento.
 
 * ``id``   É uma string que diferência maiúsculas e minúsculas representando o ID único do elemento sendo procurado.
 * ``Push``   O método push() adiciona um ou mais elementos ao final de um array e retorna o novo comprimento desse array.
 * ``Splice``   O método splice() altera o conteúdo de uma lista, adicionando novos elementos enquanto remove elementos antigos.

 * ``window.location.href`` Ele direciona para outra página ou seja propriedade retorna o URL da página atual.

 * ``parentNode`` O parentNode (que se traduzirmos literalmente significa "nó pai") é uma propriedade de um objeto do tipo Node , que representa um nó em uma árvore de elementos HTML, essa propriedade é utilizada para acessar o nó pai de um elemento.

 * ``rowIndex`` Retorna a posição de uma linha na coleção de linhas de uma tabela.

 * ``getElementById`` Método da ``Document`` interface retorna um ``Element`` objeto que representa o elemento cuja ``id`` propriedade corresponde à ``string`` especificada.

 * `` Var `` Declara uma variável, opcionalmente é possível atribuir à ela um valor em sua inicialização.

 * ``let`` Permite que você declare variáveis limitando seu escopo no bloco, instrução, ou em uma expressão na qual ela é usada. Isso é inverso da keyword ``var``, que define uma variável globalmente ou no escopo inteiro de uma função, independentemente do escopo de bloco.

 * ``for`` A declaração ``for`` começa declarando a variável ``i`` e inicializando-a como ``0``. Ela verifica se ``i`` é menor que nove, executa as duas instruções subsequentes e incrementa 1 a variável ``i`` após cada passagem pelo loop.

 * `` Function `` objeto fornece métodos para ``funções``. Em JavaScript, cada função é, na verdade, um ``Function`` objeto.

 * ``innerHTML`` Propriedade define ou retorna o conteúdo HTML (HTML interno) de um elemento.

 ## **Explicação do código em partes**

 ### Parte 1 - Código Função ``acessar``
![](img/1.png)

**Objetivo:** Validar se os campos de login foram preenchidos e, se sim, redirecionar para outra página.

* **Explicações:** 
* Obtém os valores dos campos de entrada de email e senha.
* Verifica se ambos os campos estão preenchidos.
* Se algum campo estiver vazio, exibe um alerta.
* Se ambos os campos estiverem preenchidos, redireciona para "cadastro.html". 

### Parte 2 - ``dadosLista``

![](img/Var.png)
* **Explicação**
``dadosLista`` é um array, ele armazena uma lista de nomes inseridos pelo usuário.

### Parte 3 - ``salvarUser``

![](img/Salvar.png)

* **Explicação:**
* **Objetivo:** Adicionar o nome inserido pelo usuário ao array ``dadosLista`` e atualizar a tabela com a lista de nomes.
* **Detalhes:**
``document.getElementById("nomeUser").value`` obtém o valor do campo de nome.
Se o campo não estiver vazio, o nome é adicionado ao array ``dadosLista`` e a função ``criaLista()`` é chamada para atualizar a tabela.
Após adicionar o nome, o campo é limpo ``(document.getElementById("nomeUser").value = "")``.
Se o campo estiver vazio, um alerta é mostrado pedindo para preencher o nome.

### Parte 4 - ``criarLista``

![](img/criarLista.png)

* **Explicação:**
* **Objetivo:** Criar e atualizar uma tabela HTML com a lista de nomes.
* **Detalhes:**
A variável tabela começa com o cabeçalho da tabela.
Um loop for percorre ``dadosLista`` e cria uma linha para cada nome. Cada linha inclui dois botões: ``"Editar"`` e ``"Excluir"``.
``parentNode.parentNode.rowIndex`` é usado para passar o índice da linha ao chamar as funções editar e excluir.
O conteúdo HTML da tabela é atualizado com a nova linha.

### Parte 5 - ``Editar``

![](img/editar.png)

* **Explicação:**
* **Objetivo:** Editar um nome da lista.
* **Detalhes:**
Preenche o campo de nome com o nome selecionado da tabela ``(dadosLista[(i - 1)])``.
Remove o nome da lista ``(dadosLista.splice((i - 1), 1))``, permitindo que o usuário edite o nome e o adicione novamente.

### Parte 6 - ``Excluir``

![](img/excluir.png)

* **Explicação:**
* **Objetivo:** Excluir um nome da lista e da tabela.
* **Detalhes:**
Remove o nome da lista ``(dadosLista.splice((i - 1), 1))``.
Remove a linha correspondente da tabela HTML ``(document.getElementById('tabela').deleteRow(i))``.

## Cadastro Projeto final 

![](gif/video2.gif)


## Tecnologias
 
<div style="display: inline_block"><br>
   <img align="center" alt="Rafa-HTML" height="30" width="40" src="https://raw.githubusercontent.com/devicons/devicon/master/icons/html5/html5-original.svg">
   <img align="center" alt="Rafa-HTML" height="30" width="40" src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/css3/css3-original.svg">
   <img align="center" alt="Rafa-Js" height="30" width="40" src="https://raw.githubusercontent.com/devicons/devicon/master/icons/javascript/javascript-plain.svg">
 
</div>

<br>
 
##
 
## Quer me conhecer?
 
<div>
   <a href="https://instagram.com/emy_bonfimf" target="_blank"><img src="https://img.shields.io/badge/-Instagram-%23E4405F?style=for-the-badge&logo=instagram&logoColor=white" target="_blank"></a>
   <a href="https://www.linkedin.com/in/emilly-bonfim-7709b2303" target="_blank"><img src="https://img.shields.io/badge/-LinkedIn-%230077B5?style=for-the-badge&logo=linkedin&logoColor=white" target="_blank"></a>
    <a href = "mailto:emillykbonfim@gmail.com"><img src="https://img.shields.io/badge/-Gmail-%23333?style=for-the-badge&logo=gmail&logoColor=white" target="_blank"></a>
</div>

