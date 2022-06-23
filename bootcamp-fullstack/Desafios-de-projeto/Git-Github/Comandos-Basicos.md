## **Os comandos \*Add\* e \*Commit:\***

Alterações ou adições de arquivos são adicionadas usando o comando *add*. Para adicionar qualquer arquivo, o comando é:

```
git add <nome_do_arquivo>
```

Para "salvar" as alterações é utilizado o comando *commit*:

```
git commit –m “Adicionar qualquer mensagem sobre o commit aqui”
```

## **Configuração global**

Dessa forma, as informações do desenvolvedor serão usadas por padrão em todos os repositórios do Git local:

```
git config --global user.name "Nome"
git config --global user.email usuario.padrao@gmail.com
```

## Clonando um repositório remoto

Para clonar repositório do Github 

```
git clone https://github.com/fulano/meu-repo.git 
```

## Verificando o status do repositório

É muito útil verificar como está o repositório local antes de enviar as alterações para o repositório remoto. Pode-se fazer isso usando o comando ***git status\***:

```
git status
```

## Estabelecer ligação entre o repositório local e um servidor remoto

```
git remote add origin <link do repositório remoto>
```

## Enviando para o histórico remoto (Push)

Uma vez que os arquivos e implementações foram *comitados*, é possível sincronizar esse histórico local com o histórico do repositório remoto. Isso é feito usando o comando ***git push\***:

```
git push
```

Se existir mais de um repositório vinculado, será necessário especificar o nome do repositório de destino:

```
// Comando especificando o repositório "origin"
$ git push origin
```

## Recebendo arquivos do repositório remoto (Pull)

Em projetos onde várias pessoas usam o mesmo repositório, efetuando alterações e já atualizaram o repositório remoto com coisas novas, antes de enviar o que foi feito, é preciso obter antes todas as alterações efetuadas pelos outros membros da equipe. Isso é feito usando o comando ***git pull\***:

```
// recebe o histórico do repositório remoto vinculado
$ git pull 
```

Da mesma forma que o comando *git push*, se existir mais de um repositório vinculado, será necessário especificar o nome do repositório remoto:

```
// O mesmo comando especificando o repositório "origin"
$ git pull origin
```