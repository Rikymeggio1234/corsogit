COSA E' GIT
E' un software open source di version control che serve per salvare il codice, fare il backup delle versioni e condividere il codice
-----------------------------------------------------------------

COME INSTALLARE GIT
su git-scm.com, scaricare il file .exe e installarlo con le impostazioni in base alle mie esigenze
-----------------------------------------------------------------

ESTENSIONI VSC
git graph
git history
gitlens -> da utilizzare con gitkraken che è a pagamento e serve per gestire tutti i branch, respository e funzioni git direttamente da un software apposito
-----------------------------------------------------------------

COME FUNZIONA GIT
#workflow
main <-- hotfix <-- release branch <-- dev <-- features branch

main: lavoro finito che verrà messo online

hotfixes: branch di test se non funziona qualcosa

release branch: fase di rilascio dove viene caricato il lavoro finito in dev per poi essere caricato su main

dev: fase di sviluppo

features branch: dove vengono sviluppate delle piccole parti del dev per poi essere caricate sul dev

#fork
serve per clonare il repository di qualcun'altro sul proprio e vedere quante persone lo hanno fatto
-----------------------------------------------------------------

FUNZIONI GIT
#clonare un progetto
    git clone https://github.com/[nome_utente]/[nome_progetto]

#creare un nuovo repository in locale
    git init

#creare un repository online
    andare su git hub, selezionare nuovo repository, assegnare nome e impostazione

#collegare ad un repository online
    git remote add origin https://github.com/[nome_utente]/[nome_progetto]

#pushare i file nel repository online dove mi sono collegato
    git push origin [nome_branch]
    mi manderà a video una pagina per acedere dove autorizzare
    consiglio: per pushare main usare force
        git push --force origin [nome_branch] 

#vedere lo stato del branch dove sto lavorando
    git status

#tracciare le modifiche in uno specifico file
    git add [nome_file]

#tracciare le modifiche in tutti i file
    git add .

#salvare le modifiche tracciate
    git commit -m "titolo"

#vedere tutte le modifiche salvate
    git log

#resettare un add appena fatto
    git reset

#resettare il commit precedente
    git reset HEAD~1

#resettare un commit specifico
    git reset [ash]

#passare da un branch all'altro
    git checkout [nome_branch]

#caricare dev su main
    passare al branch main
        git checkout main
    caricare dev su main
        git merge dev
