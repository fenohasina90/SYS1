## REPONSE ET ETAPES POUR RESOUDRE LES DEVOIRS ROOT ME

## FTP - Authentification
- En démarant le challenge, il y le telechargement du fichier `ch1.pcpa`.
- Ouvrir ce fichier avec Wireshark.
- Faire un recherche `ftp` dans la barre de recherche de wireshark.
- Suivre le flux TCP (tcp.stream eq 0) . ch1.pcpa .
- Le mot de passe est: `cdts3500`.

## TELNET - authentification
- En démarrant le challenge, il y a le téléchargement du fichier `ch2.pcpa`.
- Ouvrir ce fichier avec Wireshark.
- Faire un recherche `telnet` dans la barre de recherche de wireshark.
- Suivre le flux TCP (tcp.stream eq 0) . ch2.pcpa .
- Le mot de passe est: `user`.

## ETHERNET - trame
- En demarrant le challenge trame, il y a une code `hexadécimale de données`.
- Pour decoder ce code, on doit l'envoyer dans un site qui le convertie en base 64.
- On decode ce base 64 dans une autre site pour trouver l'utilisateur et le mot de passe.
- Le mot de passe est: `confi:dential`.

## Authentification twitter
- En demarrant le challenge, il y a le téléchargement du fichier `ch3.pcap`.
- On ouvre ce fichier avec wireshark.
- Suivre le flux TCP (tcp.stream eq 0) . ch3.pcpa.
- On decode la base64: `dXNlcnRlc3Q6cGFzc3dvcmQ=`.
- On obtient: `usertest:password`, `usertest` represente le nom d'utilisateur et `password` est son mot de passe.
- Pour cette Authentification on veut seulement le mot de passe.
- Donc la réponse est: `password`.

## Bluetooth - Fichier inconnu
- En demarrant le challenge, il y a le téléchargement du fichier `ch18.pcap`.
- On ouvre ce dernier avec wireshark.
- On ouvre la section `wireless` et puis, on click sur l'option `équipement bleutooth`. 
- 0n copie l'adresse mac puis le model du téléphone comme cela: `0C:B3:19:B9:4F:C6GT-S7390G`.
- On le decode sur https://www.sha1.fr/.
- La reponse est: `c1d0349c153ed96fe2fadf44e880aef9e69c122b`.