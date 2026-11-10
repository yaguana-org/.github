# Contribuer à yaguana.org

yaguana.org est le portail numérique de la commune de Léogâne, Haïti : un
projet open source, par la communauté, pour la communauté. Tout le monde peut
y participer, que l’on écrive du code ou non.

*English speakers are welcome too: issues and pull requests can be written in
English, French or Kreyòl.*

## Sans écrire de code

Le site a surtout besoin de contenu. Ouvrez une *issue* sur GitHub pour
proposer :

- **une actualité** de la commune ou d’une section communale ;
- **une institution** (école, centre de santé, service public) ;
- **une personnalité** de Léogâne ;
- **des photos**, avec le nom du photographe et son accord ;
- **des documents anciens** : vieilles photos, lettres, journaux, cartes,
  ou un témoignage enregistré, avec leur date et leur origine si on les
  connaît ;
- **une correction** : une information inexacte, une faute, une traduction ;
- **une traduction** en kreyòl ou en anglais d’un texte qui n’existe qu’en
  français.

Pour une personne ou une photo, demandez toujours la permission de la
personne (ou de sa famille) et du photographe avant de l’envoyer. Pour un
document ancien, dites qui l’a conservé et si elle peut être publiée. Un document
fragile n’a pas besoin d’être donné : une photo ou un scan suffit.

## Avec du code

1. Faites un *fork* du dépôt et créez une branche.
2. Installez et lancez le site :

       npm install
       npm run dev             # http://localhost:3000

   Copiez `env.example` en `.env` si vous avez besoin du formulaire de contact
   ou de la newsletter ; le reste du site fonctionne sans.
3. Faites vos changements, puis vérifiez :

       npm run build
       npm run check:sections

4. Ouvrez une *pull request* qui explique ce qui change et pourquoi.

Le `README.md` explique comment ajouter une actualité, une institution ou
une personnalité, et `docs/CONTENT_GUIDE.md` détaille chaque champ.

## Quelques règles

- **Trois langues.** Chaque texte existe en français (`fr`), en kreyòl
  (`ht`) et en anglais (`en`), avec les mêmes clés dans les trois fichiers.
- **Mobile d’abord.** La plupart des visiteurs sont sur téléphone : les
  classes sans préfixe sont pour les téléphones, `sm:`, `md:` et `lg:`
  s’ajoutent pour les grands écrans, et les zones à toucher font au moins
  44 px.
- **Des sources.** Les faits sur l’histoire, les institutions et les
  personnes doivent pouvoir être vérifiés.
- **Aucun secret** dans le dépôt : pas de mot de passe, de clé ni de jeton,
  ni dans le code ni dans les fichiers `.env`.
- **Des commits courts et clairs**, une phrase qui dit ce qui change.

## Licence

Le projet est sous licence GNU AGPL-3.0 (voir `LICENSE`). En proposant une
contribution, vous acceptez qu’elle soit publiée sous cette même licence.

## Respect

Soyez courtois et bienveillants. Les désaccords se règlent par les
arguments, jamais par des attaques contre les personnes.
