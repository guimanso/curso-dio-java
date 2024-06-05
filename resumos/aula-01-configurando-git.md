# Resumo 1° Aula - Configurando o Git

  **Área de Trabalho:** O terminal é o local no qual vamos inserir os comandos.
- Podemos abrir o Git de forma prática através do atalho OPEN GIT BASH HERE na pasta de queremos abrir
- `$` inicial para fazer os comandos Git
- `git config` informações sobre as variavéis e configurações do sistema, tanto do sistema, global ou local
- `CTRL + L` limpa o **terminal**
- `↑` copia o último código digitado acima
 
O global é responsável por armazenar configurações do usúario, como nome e email para realizar os commits.

**1° passo:** Passamos o comando `git config` para realizar a configuração no escopo global, utilizando o comando `--global`. Em seguida inserimos o que vamos configurar, no caso o nome de usúario, chamando assim o comando `user.name` e oassando o novo nome dentro de aspas. Veja:

`$ git config --global user.name "guimanso"`

**2° passo:** para configurar o email, utilizamos os mesmos comandos anteriores, mudando apenas o `user.name` para `user.email`. Veja:

`$ git config --global user.email guimanso23@gmail.com`

**3° passo:** Agora para confirmar essas informações podemos utilizar o comando `git config` mais `user.name`, para saber o nome, ou `user.email`, para vermos o email.

```
$ git config --global user.name
guimanso
```

Essas configurações serão utilizdas para serem exiidas quando for realizado um **commit**.

#### Configurando nossa Branch padrão

**📌 O que é uma Branch:** É como uma cópia do seu projeto onde você pode testar coisas novas sem prejudicar o projeto principal. Um caminho separado onde você pode trabalhar até que a cópia esteja pronto para ser combinada.

Para fazer a configuração da Branch:

**1° passo:** Passamos o comando inicial para ver o nome da Branch já existente
```
$ git config init.defaultBranch
master
```
**2° passo:** Para fazer a alteração do nome `master` utilizamos o mesmo comando para ver a Branch só que setando o local dessa configuração, `--global`, e passando o nome da nova Branch, que no caso é `main`.

```
$ git config --global init.defaultBranch main
```
Caso você queira confirmar a sua alteração, basta retornar com o comando inicial

`$ git config init.defaultBranch`

## 👨🏻‍💻 Comandos dessa Aula

|Comando| Descrição do Comando|
|-------|---------------------|
| `$`   | Inicial para fazer os comandos Git|
|`git config`| Responsável pelas configurações do Git|
|`--global`| Local das configurações|
|`user.name`| Configuração do nome de usúario|
|`user.email`| Configuração do email do usúario|
|`init.defaultBranch`| Consfiguração da Branch|
|`--list`| Lista de comandos de uam determinada configuração, `--global`, por exemplo.|


---

**📌 Importante:** Podemos ver todo esse processo através da documentação no site do Git