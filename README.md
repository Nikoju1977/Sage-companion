# Sage — compagnon vocal

Compagnon vocal en français, single-file HTML, par **Studio Niko Design**.

- Voix dans les deux sens (reconnaissance + synthèse du navigateur), interruption en touchant l'orbe, conversation continue mains libres.
- Cerveau **Mistral uniquement** (`mistral-small-latest`), avec garde « 0 € » : aucune génération tant que le mode Gratuit n'est pas confirmé.
- Conseil multi-agent (Auto / Supra / Fulgurant), vision sur photo, outils : Wikipédia, météo Open-Meteo, position, batterie.
- Actions téléphone confirmées d'un toucher : appel, SMS, e-mail, carte, musique, minuteur, rappel `.ics`, lampe.
- Données locales (IndexedDB) : réglages, historique, notes, profil vocal acoustique indicatif.
- Installable (PWA).

## Utilisation
1. Ouvrir la page dans Chrome (Android conseillé).
2. ⚙ → coller la clé Mistral → **Valider ma clé Mistral** → cocher la confirmation mode 0 € → **Enregistrer**.
3. Toucher l'orbe et parler.

## Limites honnêtes
Une page web ne pilote pas le téléphone en arrière-plan : chaque action passe par un toucher de confirmation. La garantie 0 € dépend aussi du réglage du compte Mistral (mode Gratuit, paiement à l'usage désactivé). L'offre gratuite Mistral est limitée en débit : les appels sont espacés automatiquement.

Conventions : XHR uniquement, `sanitizeKey()`, `safeStorage` (IndexedDB + repli mémoire).
