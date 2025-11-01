# Femtitvå - Regles en français

Ce dépôt contient les fichiers sources, les styles et les scripts de configuration nécessaires pour générer le document "Femtitvå" (version française) dans différents formats, principalement PDF et HTML, en utilisant l'outil de conversion de documents universel [Pandoc](https://pandoc.org/).

## Les Jeux de Femtitvå

Le livret "Femtitvå" (qui signifie 52 en suédois) propose 10 jeux de société modernes réinventés pour être joués avec un simple jeu de 52 cartes standard. Chaque jeu est inspiré d'un titre de jeu de société existant.

| Jeu | Inspiré de | Description |
| :--- | :--- | :--- |
| **1. Industrie** | *Race for the Galaxy* | Un jeu de construction de ville rapide où les cartes ont des fonctions multiples (monnaie, bâtiment, ressource). |
| **2. Cour** | *7 Wonders* / *Sushi Go* | Utilise le mécanisme de draft de cartes. Les joueurs collectionnent des nobles pour former la cour la plus intéressante. |
| **3. Traître** | *Battlestar Galactica* / *Werewolf* | Un jeu à rôles cachés (traître contre équipe) où les joueurs tentent de réussir cinq missions en évitant le sabotage. |
| **4. Effraction** | *Diamant* / *InCAN Gold* | Un jeu de "Push your Luck" où les joueurs collectent de l'argent dans une banque avant qu'un deuxième garde de la même couleur ne soit tiré. |
| **5. Serpent Noir** | *Ticket to Ride* | Un jeu de pose de voies abstrait utilisant des séquences de cartes ascendantes ou descendantes. |
| **6. Marteau-Piqueur** | *Hey, That's My Fish* | Un jeu de stratégie abstrait sur une grille 6x6. Les joueurs déplacent un pion pour collecter des cartes et créer des trous. |
| **7. H.O.D. (Heure Du Décès)** | *Sleuth* | Un pur puzzle logique où les joueurs résolvent un mystère (heure, motif, arme) en posant des questions par oui/non. |
| **8. Virus** | *CA$H 'N GUN$* | Un jeu de devinettes simultanées où les joueurs utilisent des gestes pour boire des médicaments, infecter, voler ou bloquer les autres. |
| **9. Paparazzi** | *Samurai* | Les joueurs placent des cartes autour de "célébrités" (figures) sur une grille pour marquer des points et capturer les plus précieuses. |
| **10. Hache** | *Flowerfall* | Un jeu où les joueurs placent des cartes pour couvrir exactement un symbole de chaque couleur possible, marquant des points pour les symboles couverts. |

## Structure du Dépôt

| Fichier/Dossier | Description |
| :--- | :--- |
| `femtitva_french.md` | Le fichier source principal au format Markdown. |
| `style.css` | Feuille de style utilisée pour le formatage des sorties HTML et PDF. |
| `pandoc_html.yaml` | Fichier de configuration Pandoc pour la conversion en HTML. |
| `pandoc_pdf_french.yaml` | Fichier de configuration Pandoc pour la conversion en PDF. |
| `convert_doc_to_html.bat` | Script Windows pour générer le fichier HTML. |
| `convert_doc_to_pdf.bat` | Script Windows pour générer le fichier PDF. |
| `images/` | Contient les images utilisées dans le document. |
| `fonts/` | Contient les polices de caractères nécessaires pour le rendu. |
| `Femtitvå 1.2.pdf` | Une version pré-générée du document. |

## Prérequis

Pour utiliser les scripts de conversion, vous devez avoir installé :

1. **Pandoc**
2. **LaTeX** (pour la génération de PDF via Pandoc, par exemple MiKTeX ou TeX Live).

## Utilisation

Pour générer les documents, exécutez simplement les scripts batch (sur Windows) :

### Générer le PDF

```bash
convert_doc_to_pdf.bat
```

Ceci utilisera `femtitva_french.md` et la configuration `pandoc_pdf_french.yaml` pour créer `femtitva_french.pdf`.

### Générer le HTML

```bash
convert_doc_to_html.bat
```

Ceci utilisera `femtitva_french.md` et la configuration `pandoc_html.yaml` pour créer `femtitva_french.html`.
