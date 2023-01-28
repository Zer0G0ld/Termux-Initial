# Comandos básicos
Aqui você encontrará comandos que estará utilizando na sua linha a linha, ou dia a dia

## ls / listar diretório
```
$ ls
    Document  Pictures  Workspace

$ ls Workspace
    Project1  Project2  Project3
```
**Listar diretórios e arquivos ocultos**
```
$ ls -a
    .Secret  .termux  Pictures  Workspace 

$ ls -a ~/Workspace/Project1
    README.md  run.py  main.py
```
**Listar informações do diretório**
```
$ ls -al
Total 32
drwx------ 9 u0_a648 4096 Dec 14 05:10 .
drwx------ 4 u0_a648 4096 Dec 13 18:39 ..
drwx------ 2 u0_a648 4096 Dec 13 17:30 .Secret
drwx------ 2 u0_a648 4096 Dec 13 16:39 .termux
drwx------ 2 u0_a648 4096 Dec 13 17:42 Pictures
drwx------ 2 u0_a648 4096 Dec 14 08:56 Workspace
```
## cd / mover para diretório
```
$ cd Workspace && ls
    Project1  Project2  Project3

$ cd ~/Workspace/Project1 && ls
    README.md  run.py  main.py
```
## mkdir / criar diretório
```
$ mkdir Folder3 && ls
    Pictures  Workspace  Folder3
```
**Criar diretório & subdiretório**
```
$ mkdir -p ~/Workspace/Project4/app/main
```
##  cp / copiar arquivo
```
$ cp ~/Workspace/Project1/main.py ~/Workspace/Project2
```
**Copiar diretório**
```
$ cp -r ~/Workspace ~/Workspace2
```
## mv / mover arquivo
```
$ mv ./index.js ./Project2

$ mv Project2 ~/Workspace
```

## rm / remover arquivo
```
$ rm index.js
$ rm -f index.js  #forçar remover
```
**Remover diretório**
```
$ rm -r ~/Workspace2
$ rm -rf ~/Workspace  #forçar remover
```
> **Obs:** tenha cuidado! Após remover o conteúdo não poderá ser recuperado
## touch / criar arquivo
```
$ touch initial.txt
```
## echo / adicionar texto
```
$ echo Hello World! >> initial.txt
```
> **Obs:** caso não haja arquivo com esse nome, criará um novo
## cat / ler arquivo
```
$ cat initial.txt
    Hello World!
```
## nano / editar arquivo
```
$ nano initial.txt
```
> **Obs:** Abrirá uma tela no terminal para editar o arquivo, para sair digite ```CTRL+X``` depois Y para salvar ou N para cancelar, após isso verifique o nome do arquivo e de ```enter```


### Observações
Para não se confundir fizemos isso aqui para vocês:

- ~/ - diretório home / inicial
- ./ - diretório atual
- ../ - diretório anterior
- && - executar outro comando após o anterior (se tudo ocorrer bem)
<!--
> **Pronto, agora podemos continuar a mexer em nossa linha de comando favorita bem mais facilmente :) também temos esse documento em [video](#LinkVideo)**
-->
