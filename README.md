1. le playbook récupère l'IP des serveurs (localhost en l'occurence mais l'inventaire demande juste à être completé puis la variable "hosts" du playbook à être mise à jour)
2. L'IP est utilisée pour completer les fichiers result_dns.yml.j2 et result_ntp.yml.j2
3. On compare les fichiers de resultats et les referentiels
4. La tâche FAIL si les deux fichiers sont différents

Il manque:
- renseigner des machines dans l'inventaire
- on récupère qu'un seul fact d'un seul serveur donc à adapter à plusieurs facts de plusieurs serveurs
