REWARD PLATFORM - DEPLOIEMENT POSTGRESQL

Configuration requise
- Node.js 20+
- PostgreSQL
- Variables d'environnement:
  NODE_ENV=production
  DATABASE_URL=... (URL PostgreSQL)
  SESSION_SECRET=secret aléatoire >= 32 caractères
  ADMIN_EMAIL=adresse admin
  ADMIN_PASSWORD=mot de passe admin >= 12 caractères

Démarrage local
1. npm install
2. définir DATABASE_URL et les autres variables
3. npm start

La base est initialisée automatiquement au premier démarrage.
Une publicité de 10 secondes à 500 F CFA est créée si aucune publicité n'existe.
Le retrait minimum est de 10 000 F CFA.
Les retraits sont manuels: l'administrateur paie puis confirme avec une référence de transaction; un refus recrédite le solde.

IMPORTANT
- Ne jamais committer .env, les secrets ou une ancienne base SQLite.
- Sur Render, utiliser l'URL PostgreSQL fournie par la base Render.
