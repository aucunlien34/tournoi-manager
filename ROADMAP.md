# Tournoi Manager — feuille de route

## V1 (en place)
- Fichier unique `index.html`, sans dépendance, hébergeable sur GitHub Pages.
- Sports prédéfinis (score simple ou sets), format de match et barème de points entièrement personnalisables (points par score de sets, bonus offensif/défensif, forfaits).
- Critères de départage ordonnables (points, victoires, confrontation directe, quotients, différences, tirage au sort).
- Phases enchaînables : poules (serpentin, par niveau, tirage), brassage → poules de niveau, phases finales en tableaux (matchs de classement complets, petite finale, consolante / tableau B).
- Planning : terrains, durées, battements, pauses, repos entre matchs, une poule par terrain, arbitrage par les équipes, replanification, décalage.
- Écran public (2e fenêtre, mise à jour en direct), classement final, impression.
- Sauvegarde : navigateur + points de restauration + export/import JSON + fichier lié (Chrome/Edge).

## Idées à développer (demandées le 2026-10-24)
1. **Format différent par phase et par tableau** : nombre de sets, points par set, durée, etc. pour chaque phase, y compris tableau principal ≠ consolante. *(V1 : seuls la durée des matchs et l'heure de début sont réglables par phase.)*
2. **Export PDF des résultats à tout moment**, idéalement une page A4 recto par phase. *(V1 : bouton Imprimer sur le planning et le classement final, sans mise en page dédiée.)*
3. **Reprise d'un tournoi / saisie libre** : saisir les résultats sans contrainte d'horaire, avec statut « match en cours » et confirmation de saisie. *(V1 : aucune contrainte d'horaire, tout match dont les équipes sont connues peut être saisi ; pas de statut « en cours ».)*
4. **Estimation du temps total minimum** affichée pendant la création de la structure. *(V1 : estimation simple — nombre de matchs / terrains × créneau — dans Configuration › Phases ; à rendre plus précise et plus visible.)*
5. **Gestion intelligente du temps de jeu** : temps de pause équilibrés entre les matchs d'une équipe, pas de longues attentes (ex. 3 créneaux). *(V1 : seulement « éviter deux créneaux d'affilée ».)* Profiter de ce chantier pour placer la finale seule en dernier créneau.
6. **Téléphone et tablette** : affichage réorganisé pour les petits écrans (navigation, saisie des scores, tableaux, planning), tout en gardant le grand affichage sur PC. *(V1 : mise en page en partie adaptative — listes de matchs et grilles qui se replient — mais pas pensée pour le téléphone ; tableaux et planning défilent en largeur.)*
