
# Tags para arquivos Marckdown.
## Titulo 
    1 - Colocar uma hashtag # antes do texto em marckdown é o mesmo que colocar a tab <h1> no HTML
    2 - Colcoar duas hashtag ## antes do texto em marckdown é o mesmo que colocar a tab <h2> no HTML
    3 - Colocar tres hashtag ### antes do texto em marckdown é o mesmo que colocar a tab <h3> no HTML
    4 - Colocar tres hashtag #### antes do texto em marckdown é o mesmo que colocar a tab <h4> no HTML
    5 - Colocar tres hashtag ##### antes do texto em marckdown é o mesmo que colocar a tab <h5> no HTML
    6 - Colocar tres hashtag ###### antes do texto em marckdown é o mesmo que colocar a tab <h6> no HTML


## Colocar em **negrito**.
###### Deve ser colocado dois asteriscos antes e depois da **l**etras, **palafra** ou **uma frase**. 
**Negritando dados com MarckDown - Colcoar dois asteriscos antes e depois do testo**


## Colocar em   _italico_ .
###### Colcoar um anderlaine no inicio e outro no fim da _l_etra, _palavra_ ou _uma frase_.


## Comandos base do GIT
**GIT INIT** - Inicializa o git

**GIT ADD** - Adiciona os arquivos - Inidica que esse arquivo será controlado pelo GIT

**GIT STATUS** - Apresenta como esta o estado do arquivo

**GIT COMMIT -m** - Utilizado para commitar um arquivo e indicar quais modificações foram feitas atravez da 
string digitada logo apos o -m.

**GIT CONFIG --list** - Lista todas as configurações que foram feitas na sua maquina para o GIT

**GII CONFIG --GLOBAL --UNSET** - Retira o atributo definido após o unset, para retirar a configuração do email deve ser digitado --> git config --global --unset user.email

**GIT CONFIG --GLOBAL user.email "seu email"** - Acrescenta o email as configurações local.

**GIT CONFIG --GLOBAL user.name "NOme cadastrado no GIT** -  Acrescenta o nome as configurações local.

#Removendo pastas ou arquivos no GIT

    1 - Primeiro cetificar se o repositório está sincronizado:
        git pull origin master - "OU a branch remota"

    2 - Remover a pasta ou arquivo local
        git rm -r "Arquivo"

    3 - Fazer o commit:
        git commit -m "Removido ..."
        
    4 - Sincronizar com o repositório
        git push origin master - "Ou a branch que deseja subir o repo"


#Criar Senha SSH e configurar

    1 - Criar a senha com o comando:
        ssh-keygen -t ed25519 -C "your_email@example.com"
    
    2 - Acessar a pasta que a chave foi criada e edicar o arquivo .pub

    3 - Abrir o GIT Config e Incluir a chave.