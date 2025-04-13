##Scraper Search.ch pour n8n
Ce nœud communautaire pour n8n permet de scraper des informations sur les entreprises suisses depuis le site search.ch. Il facilite la collecte automatisée de données comme les noms d'entreprises, numéros de téléphone, sites web et adresses.
🌟 Fonctionnalités

Recherche par mot-clé: Trouvez des entreprises en utilisant n'importe quel terme de recherche
Pagination flexible: Scrapez une page unique ou plusieurs pages spécifiques
Filtres de qualité: Filtrez les résultats par notation (excellente, moyenne, avec évaluation)
Protection IP: Support de proxy HTTP pour éviter les blocages lors de scrapage intensif
Traitement automatique des accents: Conversion automatique des caractères accentués

📦 Installation
Pour installer ce nœud communautaire dans votre instance n8n, exécutez:
bashnpm install n8n-nodes-search-ch-scraper
Alternativement, recherchez "search.ch" dans la section "Nœuds communautaires" de l'interface n8n.
🚀 Utilisation

Ajoutez le nœud "Search.ch Scraper" à votre workflow
Configurez les paramètres:

Mot clé à chercher: Par exemple "entreprise de nettoyage", "comptabilité genève"
Pages: Choisissez entre une page unique ou plusieurs pages (séparées par des virgules)
Filtre de notation: Sélectionnez le niveau de notation souhaité
Proxy HTTP (optionnel): Configurez un proxy si nécessaire


Exécutez le workflow pour récupérer les données

📊 Exemple de résultat
Le nœud retourne des données structurées pour chaque entreprise:
json{
  "nom": "Entreprise de Nettoyage SA",
  "telephone": "+41223334455",
  "siteWeb": "https://www.exemple-nettoyage.ch",
  "adresse": "Rue du Lac 10, 1200 Genève",
  "terme_recherche": "entreprise de nettoyage",
  "page": 1
}
🔍 Exemples d'utilisation
Extraction d'une liste de prestataires de services

Utilisez le nœud pour chercher "entreprise de nettoyage genève"
Filtrez pour les entreprises avec une excellente note
Exportez les résultats vers Google Sheets ou un CRM

Analyse de concurrence par secteur

Récupérez plusieurs pages de résultats pour "comptabilité lausanne"
Utilisez le nœud HTTP Request pour visiter les sites web collectés
Analysez leur présence en ligne et leurs services

⚠️ Notes importantes

Respectez les conditions d'utilisation de search.ch
Évitez de faire trop de requêtes en peu de temps
Le scraping est sensible aux changements de structure du site - le nœud pourrait nécessiter des mises à jour

🛠️ Dépannage

Aucun résultat: Vérifiez l'orthographe du mot-clé ou essayez un terme plus général
Erreurs de connexion: Si vous utilisez un proxy, vérifiez sa configuration
Données manquantes: Certaines entreprises peuvent ne pas avoir toutes les informations disponibles

📄 Licence
MIT
