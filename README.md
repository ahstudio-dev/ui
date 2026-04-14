# AHStudio — UI

> Interface utilisateur frontale des applications AHStudio, construite avec Next.js.

## Stack technique

- **Next.js 14**
- **React 18**
- **Tailwind CSS** — styles
- **TypeScript** — typage statique
- **Axios** — communication avec l'API

## Démarrage rapide

### Prérequis

- Node.js 20+
- npm ou yarn
- L'API AHStudio lancée localement

### Lancer en local

```bash
# Cloner le repo
git clone https://github.com/ahstudio-dev/ui.git
cd ui

# Installer les dépendances
npm install

# Configurer les variables d'environnement
cp .env.example .env.local

# Lancer en développement
npm run dev
```

L'interface sera disponible sur `http://localhost:3000`

## Variables d'environnement

```env
NEXT_PUBLIC_API_URL=http://localhost:8080
```

## Structure du projet

```
src/
├── app/               # Pages (App Router Next.js)
├── components/        # Composants réutilisables
│   ├── ui/            # Composants de base (boutons, inputs...)
│   └── features/      # Composants métier
├── hooks/             # Hooks React personnalisés
├── services/          # Appels API
├── store/             # Gestion d'état
└── types/             # Types TypeScript
```

## Stratégie de branches

| Branche | Rôle |
|---------|------|
| `main` | Production — versions stables uniquement |
| `develop` | Branche d'intégration |
| `feat/*` | Nouvelles fonctionnalités |
| `fix/*` | Corrections de bugs |

## Convention de commits

```
feat: ajout du tableau de bord
fix: correction du formulaire de connexion
style: refonte de la navigation
refactor: optimisation des appels API
```

## Licence

MIT — © 2025 AHStudio.
