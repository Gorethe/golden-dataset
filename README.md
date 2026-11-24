
# Golden dataset : question-réponse multimodal sur manuels agricoles de la FAO

Jeu de données de référence utilisé pour évaluer un système de question-réponse multimodal  appliqué à des manuels techniques agricoles de la FAO.

## Contenu

- 130 questions-réponses : 80 questions textuelles et 50 questions visuelles
- 16 manuels agricoles de la FAO (élevage, cultures, conservation, irrigation, pisciculture, etc.)
- Réponses attendues rédigées à la main, avec les passages et images de référence associés

## Fichier

`Data-manuel-question_v3_rempli.xlsx`

| Colonne | Description |
|---|---|
| `N` | Numéro de la question |
| `Type_modalite` | Type de question : `texte` ou `image` |
| `Question` | Question posée au système |
| `Chunk_id_pertinents` | Identifiants des passages de manuel qui contiennent la réponse (format : `manuel_pPAGE_sN`) |
| `image_id_pertinents` | Identifiants des images pertinentes (questions visuelles) |
| `Reponse_attendue` | Réponse de référence |
| `Reponse_attendue_2` | Seconde formulation de la réponse de référence |
| `Reponse_systeme` | Réponse produite par le système multimodal |
| `Reponse_baseline_texte` | Réponse produite par la baseline textuelle |

La feuille `Notation` décrit le format des identifiants, et la feuille `Reserve_chevres` contient des questions de réserve non comptées dans les 130.

## Utilisation

Ce jeu de données sert à comparer les réponses d'un système à des réponses de référence, par récupération des bons passages et par qualité de la réponse générée.

## Citation

Toumba Ngongo, C. (2025). *Système de question-réponse multimodal appliqué aux manuels techniques agricoles de la FAO* [Mémoire de master]. 
International School, Vietnam National University, Hanoï.
