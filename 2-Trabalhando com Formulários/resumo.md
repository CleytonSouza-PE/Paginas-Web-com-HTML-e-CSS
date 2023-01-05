# Trabalhando com Formulários


* **Formulário:**

É um trecho do html que vai existir campos onde o usuário vai inserir informações., podendo ser um campo texto, um campo numero, um campo de múltipla seleção entre outros. O formulário anda ao lado do servido, pois o mesmo coleta os dados fornecidos pelos usuário que ao clicar no botão enviar automaticamente os enviam através da internet diretamente para o servidor através da comunicação Client X Server que pode guardar ou não essas informações em um banco de dados.

* **Banco de dados:**

É uma aplicação que fica em um mesmo servidor ou em outro que tem a responsabilidade de armazena as informações.

O formulário consiste na tag `<form>` que por sua vez abre e fecha e dentro dela são colocados os campos. Para inserir campos no formulário vamos utilizar uma tag filha do da tag `<form>` que é a trag `<input />` a mesma até aparece fora da tag `<form>` porém seriam em esporádicas vezes para ser utilizada via CSS.

* `<input/>`: A tag coloca um campo na tela onde o usuário consegue digitar uma informação. A referida tag vem acompanhada de alguns atributos como: `type` e `name` entre outros.

    * `type`: Define o tipo do campo que por exemplo pode ser `text`, `number` e `password` entre outros.

    * `text` - Configura o campo do formulário para receber dados do tipo texto.
    
        Ex.:
        ```
        <form>
	    Nome: <input type=”text” />
        </form>
        ```

    * `number`: Configura o campo do formulário para receber dados do tipo números

        Ex.:
        ```
        <form>
	    Nome: <input type=”number” />
        </form>
        ```

    * `password`: Configura o campo do formulário para receber dados do tipo password, ou seja do tipo senha.

        Ex.:
        ```
        <form>
	    Nome: <input type=”password”  />
        </form>

Exemplo da utilização da tag `<input>` e alguns atributos em um formulário
```
<html>
	<head><title>Formuário de Cadastro</title>
	<body>
		<form>
			Nome: <input type=”text” name=”name” /><br>
			Idade: <input type=”number” name=”age” /><br>
			Senha: <input type=”password” name=”password” /><br>
			<button type=”submit”>Enviar</button>
		</form>
	</body>
</html>
```


Na tag `<form>` podemos utilizar alguns atributos:

* name: Atributo que dá nome ao formulário e aos campos do formulário
        
    Ex.:

    * tag `name`utilizada para dar nome ao formulário:
    ```
    <form name=”signup”>
    </form>
    ```
    * tag `name`utilizada para dar nome ao campo do  formulário:
    ```
    <form name="signup" autocomplete="off" method="post" action="">
        Name: <input type="text" name="name" />
        <Button type="submit">Enviar</Button>
    </form>
    ```

