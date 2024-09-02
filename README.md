# SOC-as-Service

**SOC as a Service (SOCaaS)** externalise la gestion de la sécurité informatique, offrant une surveillance 24/7, une gestion des incidents, une analyse des menaces, et des rapports détaillés. Bénéficiez d'une expertise avancée sans infrastructure interne, idéal pour renforcer la sécurité de manière scalable.

## Tech Stack

- **Clients :** Filebeat, Webapp, BD, VoIP
- **Services Internes :** Logstash, Elasticsearch, Kibana, Elastalert, Sigma
- **Services Externes :** Jira, Mail Server, Slack

## Features

- Surveillance des logs en temps réel
- Enrichissement et visualisation des données
- Gestion des alertes avec intégration multi-canaux
- Règles de détection personnalisables

## Deployment

1. **Filebeat** envoie les logs à **Logstash**.
2. **Logstash** enrichit les logs et les transmet à **Elasticsearch**.
3. **Elasticsearch** fournit les données à **Kibana** pour la visualisation et à **Elastalert** pour la gestion des alertes.
4. **Sigma** fournit des règles de détection à **Elastalert**.
5. **Elastalert** envoie des alertes à **Jira**, **Mail Server**, et **Slack**.
6. **Kibana** permet aux analystes SOC de visualiser et analyser les données.

### Schema

![App Screenshot](https://raw.githubusercontent.com/Agb242/Soc-as-Service/main/Screen%20Shot%202024-08-31%20at%2021.30.54.png)

### Diagramme 

![App Screenshot]([https://raw.githubusercontent.com/Agb242/Soc-as-Service/main/Screen%20Shot%202024-08-31%20at%2021.30.54.png](https://raw.githubusercontent.com/Agb242/Soc-as-Service/main/deployment_diagram%20(3).png))
