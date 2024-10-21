Compréhension du projet Minishell :

Outils nécessaires : fork(), execve(), waitpid(), dup2()

Que doit gérer notre programme ?
	- Gestion des commandes simples (exécuter des commandes comme ls, echo, etc.)
	- Gestion des redirections (redirection d'entrée/sortie avec >, <)
	- Gestion des pipes (|)
	- Gestion des signaux (comme CTRL+C, CTRL+D, et CTRL+\)
	- Gestion des builtins (commandes internes comme cd, export, unset)

Ordre de processus :
	- Lire les entrées de l'utilisateur
  - Fixer un ordre de priorités
  - Interpréter les commandes et utiliser fork() et execve() pour les exécuter
