# CMCE — Centre Médical du Château d'Eau

Site vitrine statique pour le Centre Médical du Château d'Eau (Philippe et
Maëlle Lefevre, kinésithérapeutes), à Braine-l'Alleud.

Domaine visé : cmce.be (pas encore enregistré).
Sous-domaine de test actuel : cmce.dmebud.eu.

Stratégie de déploiement identique aux autres projets (voir nat-r) :
branche `draft` → sous-domaine de test, branche `main` → domaine définitif
(créée plus tard une fois le domaine prêt).

## À faire avant le premier déploiement
- Créer le dépôt GitHub `Bud-90/cmce` et pousser la branche `draft`.
- Sur le VPS (CloudPanel) : créer le sous-domaine `cmce.dmebud.eu` et un
  utilisateur SSH de déploiement dédié (ex. `deployer_cmce`).
- Ajouter les secrets GitHub Actions `SSH_PRIVATE_KEY` et `SSH_HOST`.
- Mettre à jour le nom d'utilisateur SSH dans `.github/workflows/deploy.yml`
  si besoin.

## Contenu à compléter
- Bios de Philippe et Maëlle Lefevre (page équipe).
- Liste détaillée des services proposés (page services).
- Lien vers le système de prise de rendez-vous en ligne (page contact).
