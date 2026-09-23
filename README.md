# Demandes — version GitHub partagée

Cette version corrige le problème du téléphone et du PC qui n'ont pas les mêmes demandes :
les demandes et les comptes sont stockés dans Supabase au lieu de `localStorage`.

## À mettre sur GitHub

Mets **ces 4 fichiers** dans ton dépôt GitHub :
- `index.html`
- `config.js`
- `supabase.sql`
- `README.md`

## 1. Créer la base Supabase

1. Va sur Supabase et crée un projet.
2. Ouvre **SQL Editor**.
3. Copie-colle tout le contenu de `supabase.sql`.
4. Exécute le script.

## 2. Récupérer les 2 informations Supabase

Dans Supabase : **Project Settings → API** :
- Project URL
- clé **anon / publishable**

Ouvre `config.js` et remplace :
- `https://TON-PROJET.supabase.co`
- `TA_CLE_ANON`

Ne mets **jamais** la clé `service_role` dans GitHub.

## 3. Mettre sur GitHub

Mets uniquement les 4 fichiers ci-dessus à la racine du dépôt.

Puis :
**Settings → Pages → Deploy from a branch → main → / (root)**

## Comptes équipe

- Mathis / `Mathis2026!` → tous les droits
- Andry / `Andry2026!` → tous les droits
- Joshua / `Joshua2026!` → valider/refuser
- Secretaire / `Secret2026!` → répondre/supprimer

## Important

Le site est maintenant partagé : une demande envoyée depuis le téléphone est enregistrée dans Supabase et peut être consultée depuis le PC.

Cette version est conçue pour un petit usage privé. Le système de connexion est volontairement simple ; pour une application publique avec données sensibles, il faut remplacer cette authentification par Supabase Auth et des règles RLS plus strictes.

