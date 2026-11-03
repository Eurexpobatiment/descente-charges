# Calculateur de descente de charges – Eurexpo

Application web (GitHub Pages) qui calcule la charge par point d'appui ramenée au m² de plaque de répartition et la compare à la limite admissible de l'emplacement (sol enrobé, caniveau, au-dessus galerie).

- Plaques, emplacements et historique : Google Sheet « Calculateur Descente de Charges » (onglets Plaques, Emplacements, Historique), lus via l'API Apps Script.
- Rapport PDF généré par Apps Script et téléchargé sur l'appareil.
- Plan du sous-sol : `plan-sous-sol.png` (caniveaux en bleu, galeries techniques en noir).
