COSA E' GIT<br>
e' un software open source di version control che serve per salvare il codice, fare il backup delle versioni e condividere il codice<br>
-----------------------------------------------------------------

COME INSTALLARE GIT<br>
su git-scm.com, scaricare il file .exe e installarlo con le impostazioni in base alle mie esigenze<br>
-----------------------------------------------------------------

ESTENSIONI VSC<br>
git graph<br>
git history<br>
gitlens -> da utilizzare con gitkraken che è a pagamento e serve per gestire tutti i branch, respository e funzioni git direttamente da un software apposito<br>
-----------------------------------------------------------------

COME FUNZIONA GIT<br>
#workflow<br>
main <-- hotfix <-- release branch <-- dev <-- features branch<br>
main: lavoro finito che verrà messo online<br>
hotfixes: branch di test se non funziona qualcosa<br>
release branch: fase di rilascio dove viene caricato il lavoro finito in dev per poi essere caricato su main<br>
dev: fase di sviluppo<br>
features branch: dove vengono sviluppate delle piccole parti del dev per poi essere caricate sul dev<br>
-----------------------------------------------------------------

FORK<br>
serve per clonare il repository di qualcun'altro sul proprio e vedere quante persone lo hanno fatto<br>
-----------------------------------------------------------------

FUNZIONI GIT<br>
#clonare un progetto<br>
git clone https://github.com/[nome_utente]/[nome_progetto]<br>
<br>
#creare un repository online<br>
andare su git hub, selezionare nuovo repository, assegnare nome e impostazione<br>
<br>
#creare un nuovo repository in locale<br>
git init<br>
<br>
#collegare ad un repository online<br>
git remote add origin https://github.com/[nome_utente]/[nome_progetto]<br>
<br>
#pushare i file nel repository online dove mi sono collegato<br>
git push origin [nome_branch]<br>
mi manderà a video una pagina per acedere dove autorizzare<br>
consiglio: per pushare main usare force<br>
git push --force origin [nome_branch] <br>
<br>
#vedere lo stato del branch dove sto lavorando<br>
git status<br>
<br>
#tracciare le modifiche di uno specifico file<br>
git add [nome_file]<br>
<br>
#tracciare le modifiche di tutti i file<br>
git add .<br>
<br>
#resettare un add appena fatto<br>
git reset<br>
<br>
#salvare le modifiche tracciate<br>
git commit -m "titolo"<br>
<br>
#vedere tutte le modifiche salvate<br>
git log<br>
<br>
#resettare il commit precedente<br>
git reset HEAD~1<br>
<br>
#resettare un commit specifico<br>
git reset [ash]<br>
<br>
#creare un nuovo branch<br>
git checkout -b [nome_branch]<br>
#passare da un branch all'altro<br>
git checkout [nome_branch]<br>
<br>
#caricare dev su main<br>
passare al branch main prima di svolgere la funzione<br>
git merge dev<br>
<br>
