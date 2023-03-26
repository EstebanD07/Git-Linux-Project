# Git-Linux-Project
Le code est écrit en Python et utilise la bibliothèque Dash pour créer un tableau de bord en temps réel qui affiche le prix du bitcoin et un graphique montrant son évolution au fil du temps.

Dans Q2, la commande curl est utilisée pour récupérer le prix actuel du bitcoin à partir de l'API de coingecko, et la commande grep est utilisée pour extraire la valeur du prix.

Dans Q3, une application Dash est créée avec un titre, un conteneur pour afficher le prix actuel du bitcoin, un graphique pour afficher l'historique des prix et un intervalle pour mettre à jour le prix toutes les 5 secondes. La fonction de rappel update_price récupère le prix actuel du bitcoin en utilisant la même commande curl et grep que dans Q2, puis affiche le prix dans le conteneur et le graphique.

Dans Q4, une liste historical_prices est initialisée pour stocker l'historique des prix du bitcoin. La fonction de rappel update_price est modifiée pour ajouter le prix actuel à la liste historical_prices, qui est ensuite utilisée pour afficher l'historique des prix dans le graphique.

Dans Q5, une tâche Cron est configurée pour exécuter le script du tableau de bord toutes les 5 minutes en utilisant la commande crontab -e.

Dans Q6, une fonction get_daily_metrics est définie pour récupérer les métriques quotidiennes du bitcoin. Une deuxième fonction de rappel update_daily_report est définie pour mettre à jour le rapport quotidien à 20h chaque jour en utilisant la fonction get_daily_metrics.
