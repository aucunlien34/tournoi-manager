# Tournoi Manager — feuille de route

Application en ligne : https://aucunlien34.github.io/tournoi-manager/

## V1
- Fichier unique `index.html`, sans dépendance, hébergé sur GitHub Pages.
- Sports prédéfinis (score simple ou sets), format de match et barème de points entièrement personnalisables (points par score de sets, bonus offensif/défensif, forfaits).
- Critères de départage ordonnables (points, victoires, confrontation directe, quotients, différences, tirage au sort).
- Phases enchaînables : poules (serpentin, par niveau, tirage), brassage → poules de niveau, phases finales en tableaux (matchs de classement complets, petite finale, consolante / tableau B).
- Planning : terrains, durées, battements, pauses, une poule par terrain, arbitrage par les équipes, replanification, décalage.
- Écran public (2e fenêtre, mise à jour en direct), classement final, impression.
- Sauvegarde : navigateur + points de restauration + export/import JSON + fichier lié (Chrome/Edge).

## V2 (2026-10-24) — idées réalisées
1. **Format par phase et par tableau** : nombre de sets, points par set, set décisif et durée des matchs propres à chaque phase, et à chaque tableau (principal ≠ consolante).
2. **Export PDF à tout moment** : une page A4 par phase (classements + résultats), classement final, planning ; chaque page est réduite automatiquement pour tenir sur une feuille.
3. **Match en cours / saisie libre** : statut « en cours » (listes + écran public) ; le jour du tournoi, saisir un match pas encore commencé demande confirmation, avec option « saisie libre » pour reprendre un tournoi.
4. **Estimation du temps total** : simulation complète du planning (pauses, repos, ordre des phases, durées par phase), affichée dès la création du tournoi, dans les Phases (avec horaires de chaque phase) et dans Terrains & horaires.
5. **Temps de jeu équilibré** : le planificateur donne la priorité aux équipes qui attendent depuis le plus longtemps, évite les enchaînements et compare 40 variantes pour garder la meilleure ; la finale est jouée seule au dernier créneau.
6. **Téléphone et tablette** : onglets fixes et défilants, listes compactes, planning en liste, saisie des scores plein écran avec grands champs ; affichage PC inchangé.
7. **Feuilles de terrain (PDF)** : pour la phase en cours, une page A4 par terrain avec cases pour noter les scores à la main (par set en volley), arbitre, lignes à remplir pour les équipes pas encore connues.

## Pistes
- Saisie des scores par les arbitres sur téléphone (nécessiterait un serveur).
- Feuilles de terrain avec QR code renvoyant au match.
