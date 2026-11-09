# Calculateur de descente de charges – Eurexpo

Application web (GitHub Pages) qui calcule la charge par point d'appui ramenée au m² de plaque de répartition et la compare à la limite admissible de l'emplacement (sol enrobé, caniveau, au-dessus galerie).

- Données : **Firebase** (projet `equipe-batiment`, comme les autres applis) depuis le 9 nov. 2026 :
  - `DcConfig/refs` : plaques et emplacements, modifiables dans l'appli (carte « Références », code d'accès Bâtiment) ;
  - `DcHistorique` : calculs enregistrés, affichés dans la carte « Historique » (clic sur une ligne = recharger le calcul).
  - En secours, l'appli reprend les valeurs du classeur (4 plaques KSI, 3 emplacements).
- Règles Firestore : bloc `firestore-descente-charges.rules`, publié dans les règles du projet le 9 nov. 2026.
- Rapport PDF : toujours fabriqué par le script Google « Calculateur Descente de Charges » (`genererRapport`) à partir des données envoyées, puis téléchargé (rien dans Drive).
- Le Google Sheet « Calculateur Descente de Charges » n'est plus lu par l'appli ; il reste comme archive.
- Plan du sous-sol : `plan-sous-sol.png` (caniveaux en bleu, galeries techniques en noir). `/v2/` redirige vers la racine.
