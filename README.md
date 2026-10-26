# Réveil des sites

Garde les sites hébergés sur l'offre gratuite de Render éveillés aux heures d'école, pour éviter
le réveil lent (environ 25 s) au premier visiteur. Ce dépôt est public pour que les minutes
GitHub Actions restent gratuites : il ne contient aucun secret, seulement l'adresse publique
des sites.

- `ping-ecole-manager.yml` : appelle `/up` toutes les 10 min, de 6 h à 21 h (heure de Lomé),
  du lundi au samedi, et réveille le site avant les tâches planifiées (07:40 chaque jour,
  02:40 le 1er du mois).
- `maintien-activite.yml` : GitHub désactive les tâches planifiées d'un dépôt public sans
  activité pendant 60 jours ; ce workflow ajoute un commit vide une fois par mois.
