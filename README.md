# ansible
le playbook que j'ai préparé  permet d'automatiser la configuration d'une machine
le playbook que j'ai préparé  contient  variable:
target_group :le groupe que vous voulez creer 
target_username:le user que vous voulez creer 
et is_sudoer : si vous voulez que ce user soit sudoer ou non 
package_name1 et package_name2
-creation d'un fichier "success.log" ou chaque etape reussite est ecrite dedans .
-verifie si le groupe existe et retourne un message sur le terminal et en "success.log "
sinon il realise sa creation 
-verifie si le user existe et retourne un message sur le terminal et en "success.log" 
sinon il realise sa creation
-ajoute ce user au "target_group"
- ajoute ce user au sudoers selon la variable is_sudoer 
-assure .ssh directory est existante pour ce user 
-set authorised_keys file permissions 
-genere ssh key pair pour le user 
-ajoute "public key" to authorized_keys 
-mise a jour de apt cache 
-installation de packages 1 et 2
