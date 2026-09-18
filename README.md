# Cyber Watch n8n

Automatisation personnelle de veille cybersécurité avec n8n.

## Fonctionnement

Tous les jours à 7h30 :

1. récupération de plusieurs flux RSS cybersécurité
2. filtrage des éléments récents
3. agrégation des résultats
4. génération d'un email HTML
5. envoi automatique du digest

## Sources

- CERT-FR
- CERT-FR SCADA
- The Hacker News
- Riskintel Media

## Stack

- n8n
- Docker
- Linux
- OVHcloud VPS
- RSS
- SMTP

## Workflow

Schedule Trigger
→ RSS Feeds
→ Merge
→ Filter
→ Aggregate
→ JavaScript
→ Send Email

## Sécurité

Les credentials, secrets et fichiers `.env` ne sont pas versionnés.
