# Script PowerShell – Téléchargement, extraction et recompression d’archives

 **Attention** : Ce script est fourni uniquement à titre d’exemple pédagogique.  
> Il ne doit pas être utilisé avec des fichiers malveillants.  
> Utilisez-le uniquement avec vos propres archives de test ou fichiers de données sûrs.

## Description

Ce script PowerShell permet de :
1. Télécharger plusieurs fichiers ZIP depuis des URLs.
2. Les extraire avec un mot de passe (optionnel).
3. Regrouper le contenu extrait dans une nouvelle archive ZIP.

## Variables principales

- `urls` : Liste des URLs des fichiers ZIP à télécharger.
- `tempFolder` : Dossier temporaire de travail.
- `outFolder` : Dossier de sortie des fichiers extraits.
- `password` : Mot de passe des archives ZIP (si nécessaire).
- `finalZip` : Nom du fichier ZIP final généré.
- `zipPath` : Chemin vers l’exécutable de 7-Zip.

## Pré-requis

- Windows avec **PowerShell**
- **7-Zip** installé (et son chemin ajouté dans la variable `zipPath`)

## Exemple d’utilisation

```powershell
# Définir les URLs des fichiers ZIP (exemple fictif)
$urls = @(
    "https://exemple.com/fichiers/test1.zip",
    "https://exemple.com/fichiers/test2.zip"
)

# Lancer le script
.\process-archives.ps1
