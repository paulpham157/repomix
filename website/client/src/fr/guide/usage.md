# Utilisation de base

## Démarrage rapide

Empaquetez tout votre dépôt:

```bash
repomix
```

## Cas d'utilisation courants

### Empaqueter des répertoires spécifiques

```bash
repomix path/to/directory
```

### Inclure des fichiers spécifiques

Utilisez des [motifs glob](https://github.com/mrmlnc/fast-glob?tab=readme-ov-file#pattern-syntax):

```bash
repomix --include "src/**/*.ts,**/*.md"
```

### Exclure des fichiers

```bash
repomix --ignore "**/*.log,tmp/"
```

### Dépôts distants

```bash
# En utilisant l'URL GitHub
repomix --remote https://github.com/user/repo
# En utilisant le format abrégé
repomix --remote user/repo
# Branche/tag/commit spécifique
repomix --remote user/repo --remote-branch main
repomix --remote user/repo --remote-branch 935b695
```

### Compression de code

```bash
repomix --compress
# Vous pouvez également l'utiliser avec des dépôts distants:
repomix --remote yamadashy/repomix --compress
```

## Formats de sortie

### XML (Par défaut)

```bash
repomix --style xml
```

### Markdown

```bash
repomix --style markdown
```

### Texte brut

```bash
repomix --style plain
```

## Options supplémentaires

### Supprimer les commentaires

```bash
repomix --remove-comments
```

### Afficher les numéros de ligne

```bash
repomix --output-show-line-numbers
```

### Copier dans le presse-papiers

```bash
repomix --copy
```

### Désactiver la vérification de sécurité

```bash
repomix --no-security-check
```

## Configuration

Initialiser le fichier de configuration:

```bash
repomix --init
```

Consultez le [Guide de configuration](/fr/guide/configuration) pour les options détaillées.
