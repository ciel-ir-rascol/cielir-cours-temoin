# kit — c01 : Du code source au programme

**Informatique — BTS CIEL-IR 1re année** · Lycée Louis Rascol, Albi

📽️ **Les slides : <https://ciel-ir-rascol.github.io/cielir-cours-temoin/>**
📄 **Les fiches en PDF : [dernière release](https://github.com/ciel-ir-rascol/cielir-cours-temoin/releases/latest)**

Ce dépôt n'est pas un vrai cours : c'est le **témoin** de [`cielir-cours-kit`](https://github.com/ciel-ir-rascol/cielir-cours-kit). Un cours jouet d'environ **1 h**, bâti pour exercer d'un coup toute la mise en page du kit — et pour servir d'exemple complet du standard.

Il est régénéré à chaque modification du kit. Le tag `v1` du kit ne bouge qu'après l'avoir régénéré sans régression, et relu à l'œil, en couleur puis en niveaux de gris.

Ce qu'il exerce : trous dans une phrase, trous dans un tableau, lignes de réponse rédigée, les cinq encadrés, bloc terminal, code coloré, schéma SVG à compléter.

## Capacités visées

- Distinguer code source, code objet et programme
- Compiler et exécuter un programme C++ en ligne de commande

## Déroulé (1 h)

| Partie | Contenu | Slides | Durée indicative |
| :---: | --- | :---: | :---: |
| — | Pourquoi le C++ : vitesse, portabilité, deux paradigmes | 1–2 | 10 min |
| 1 | La chaîne de construction, schéma à compléter | 3 | 20 min |
| 2 | Un premier programme, compilation et exécution | 4–5 | 25 min |
| — | Crédits | 6 | 5 min |

## Arborescence

```text
.
├── cours.yml                        métadonnées du bloc
├── COURS.md                         le cours — source unique des deux fiches
├── slides/
│   ├── 01-temoin.md                 source des slides (Marp)
│   └── img/schema.svg               chaîne de construction, à compléter
├── .vscode/settings.json            thème Marp pour l'aperçu dans VS Code
└── .github/workflows/publier.yml    copie de gabarits/publier.yml du kit
```

Aucun fichier généré n'est enregistré ici : les PDF et les slides en ligne sont produits à la publication.

## Travailler le cours

L'aperçu des slides se fait dans VS Code avec l'extension **Marp for VS Code** ; le thème `ciel` est déjà déclaré dans `.vscode/settings.json`.

Pour régénérer les trois PDF en local, depuis une copie du kit :

```bash
make temoin DEPOT=../cielir-cours-temoin
```

### Publier

```bash
git tag v1.01 && git push origin v1.01
```

`vX` est la mouture d'une promotion, `vX.YY` une retouche de cours d'année. Le reste est automatique : contrôle de confidentialité, trois PDF, slides en ligne, release. Réglage à faire une fois : *Settings > Pages > Source* = « GitHub Actions ».

## Crédits des images

| Image | Auteur | Licence | Source |
| --- | --- | --- | --- |
| Schéma de la chaîne de construction (`slides/img/schema.svg`) | auteur du cours | CC BY-NC-SA 4.0 | ce dépôt |

## Licence

[CC BY-NC-SA 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/deed.fr)
