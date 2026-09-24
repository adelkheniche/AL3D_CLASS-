# Awesome Onshape & impression 3D

Une liste de ressources pour découvrir la fabrication additive, prendre des mesures et modéliser le boîtier d’un VU-mètre avec Onshape.

**Bachelor Human IT · ENSEA · Première année**

## Sommaire

* [Comprendre l’impression 3D](#comprendre-limpression-3d)
* [Choisir la matière et concevoir la pièce](#choisir-la-matière-et-concevoir-la-pièce)
* [Procédés et pistes pour demain](#procédés-et-pistes-pour-demain)
* [Du modèle au fichier imprimable](#du-modèle-au-fichier-imprimable)
* [Onshape et prise de mesure](#onshape-et-prise-de-mesure)
* [Source](#source)

## Comprendre l’impression 3D

* **Fabrication soustractive ou additive** — [Procédés soustractifs](https://medium.com/cnc-life/history-of-cnc-machining-part-1-2a4b290d994d) · [Histoire de l’impression 3D — V&A](https://www.vam.ac.uk/articles/at-the-press-of-a-button-a-va-history-of-3d-printing)  
  *L’usinage retire de la matière, l’impression 3D la dépose ou la solidifie. Le bon procédé dépend de la forme, du matériau, du délai et du nombre de pièces.*

* **Des objets difficiles à fabriquer autrement** — [Montre 3D printed](http://www.laimer.ch) · [OpenFlexure Delta Stage](https://openflexure.org/projects/deltastage/) · [Pico V2](https://fab.cba.mit.edu/classes/865.21/people/rahul/PicoV2/)  
  *faire du complexe: intégrer des fonctions, fabriquer des formes complexes et itérer rapidement sans outillage spécifique.*

* **Contraintes et échecs** — [3DBenchy : les points à observer](https://www.3dbenchy.com/features/) · [Exemple d’échec](https://academy.cba.mit.edu/classes/scanning_printing/fail.jpg)  
  *comprendre pourquoi : température, adhérence, orientation, matière ou géométrie. Le Benchy apprend à lire les défauts.*

* **Résolution, temps et coût** — [Speed Benchy : règles et réglages](https://stldenise3d.com/speed-benchy-settings-and-rules/)  
  *vitesse ou precision: une petite hauteur de couche augmente fortement le temps. Pour un prototype, on cherche une précision suffisante et un délai raisonnable.*

* **Ventilation et sécurité** — [Émissions et ventilation — MIT](https://academy.cba.mit.edu/classes/scanning_printing/emissions.pdf) · [Certification GREENGUARD — Prusa](https://blog.prusa3d.com/the-original-prusa-mk4-and-mk4s-are-ul-greenguard-certified_101657)  
  *Une imprimante chauffe des polymères : on ventile, on évite de rester inutilement près de la machine et on ne touche jamais la buse ni le plateau chaud.*

## Choisir la matière et concevoir la pièce

* **Guide des matériaux** — [Tableau des matériaux — Prusa](https://help.prusa3d.com/en/materials) · [Comparatif des propriétés — Simplify3D](https://www.simplify3d.com/support/materials-guide/properties-table/)  
  *comment choisir un materiaux: température d’usage, rigidité, chocs, extérieur, souplesse et facilité d’impression.*

* **PLA, PETG et PHA** — [Guide filament Prusa](https://help.prusa3d.com/category/material-guide_220)  
  *Pour débuter, le PLA est le plus simple. uniquement au fablab Le PETG résiste mieux à la chaleur et aux chocs mais demande plus de réglages. Le PHA ouvre la discussion sur les polymères biosourcés.*

* **Filaments techniques et composites** — [Composites chargés métal](https://www.matterhackers.com/store/c/metallic-3d-printing-filament) · [Composites chargés bois](https://www.matterhackers.com/store/c/fillamentum/fillamentum-timberfill-series)  
  *Ajouter des fibres ou des particules change l’aspect et parfois les performances, mais use davantage la buse et rend l’impression plus exigeante.*

* **Humidité, cycle de vie et matériaux adaptatifs** — [Biomatériaux et cycle de vie — MIT](http://cba.mit.edu/docs/papers/22.12.Biomaterials.pdf) · [Imprimer avec un matériau inconnu — MIT](https://news.mit.edu/2024/3d-printer-can-print-with-unknown-material-0408)  
  *Beaucoup de filaments absorbent l’eau et deviennent difficiles à imprimer. Demain, les machines pourront aussi identifier une matière et adapter leurs paramètres.*

* **Règles de conception** — [Planche de règles — MIT](https://academy.cba.mit.edu/classes/scanning_printing/designrules.jpg)  
  *Chaque couple machine–matière a ses limites.*

* **Supports, surplombs et ponts** — [Objets articulés imprimés en place](https://n-e-r-v-o-u-s.com/projects/albums/kinematics-link/) · [Types de supports — Prusa](https://help.prusa3d.com/article/support-material_1698) · [Exemple de pont — MIT](https://academy.cba.mit.edu/classes/scanning_printing/Prusa/bridging.jpg)  
  *Un bon modèle limite les supports : moins de matière, moins de temps et de meilleures surfaces. Les ponts courts peuvent souvent être imprimés dans le vide.*

* **Jeu, dimensions et épaisseur de paroi** — [Test de jeu — MIT](https://academy.cba.mit.edu/classes/scanning_printing/Prusa/clearance.jpg) · [Test dimensionnel — MIT](https://academy.cba.mit.edu/classes/scanning_printing/Prusa/dimension.jpg) · [Épaisseur minimale — MIT](https://academy.cba.mit.edu/classes/scanning_printing/Form3/thickness.jpg)  
  *Deux pièces dessinées à la même cote ne s’emboîtent pas forcément. On prévoit un jeu, on mesure la pièce imprimée et on corrige le modèle.*

* **Anisotropie et orientation** — [Test d’anisotropie — MIT](https://academy.cba.mit.edu/classes/scanning_printing/Prusa/anisotropy.jpg)  
  *Une pièce FDM est généralement plus fragile entre les couches. On l’oriente pour que les efforts principaux restent autant que possible dans le plan des couches.*

* **Première couche, nivellement et adhérence** — [Calibration de la première couche — Prusa](https://help.prusa3d.com/article/first-layer-calibration-i3_112364) · [Problèmes d’adhérence — Prusa](https://help.prusa3d.com/article/first-layer-issues_1804)  
  *La première couche conditionne toute l’impression. Elle doit être continue, légèrement écrasée et déposée sur un plateau propre et bien réglé.*

* **Inserts et post-traitement** — [Insérer une pause dans l’impression](https://help.prusa3d.com/article/insert-pause-or-custom-g-code-at-layer_120490) · [Revêtement époxy](https://www.smooth-on.com/Epoxy-Coatings-XTC/c1397_1429/index.html) · [Lissage par repassage — Prusa](https://help.prusa3d.com/article/ironing_177488)  
  *Une pièce imprimée peut recevoir des écrous, des aimants ou des inserts. Le post-traitement améliore l’aspect, mais ajoute du temps et peut modifier les dimensions.*

## Procédés et pistes pour demain

* **Stéréolithographie — SLA** — [Formlabs Form 4](https://formlabs.com/3d-printers/form-4/) · [Elegoo Saturn](https://www.elegoo.com/collections/saturn-series) · [Nanoscribe](https://www.nanoscribe.com/en/)  
  *La SLA solidifie une résine avec de la lumière. Elle offre des détails fins, mais impose des gants, du nettoyage et une post-cuisson.*

* **Dépôt de filament — FDM / FFF** — [Technologie FDM — Stratasys](https://www.stratasys.com/en/guide-to-3d-printing/technologies-and-materials/fdm-technology) · [Arbre généalogique RepRap](https://reprap.org/wiki/RepRap_Family_Tree) · [Prusa](https://www.prusa3d.com) · [Bambu Lab](https://bambulab.com)  
  *C’est le procédé utilisé pendant le cours : accessible, visible et adapté au prototypage. Les lignes déposées expliquent sa simplicité et ses limites mécaniques.*

* **Argile, grande échelle et construction** — [Impression d’argile — WASP](https://www.3dwasp.com/en/clay-3d-printer-delta-wasp-2040-clay) · [Construction imprimée — Crane WASP](https://www.3dwasp.com/en/3d-printer-house-crane-wasp) · [Hangprinter](https://hangprinter.org/)  
  *Le dépôt par couches ne se limite pas au plastique : on peut extruder de l’argile ou du béton et changer complètement l’échelle de fabrication.*

* **Recycler localement le plastique** — [Precious Plastic](https://preciousplastic.com) · [Filastruder](https://www.filastruder.com)  
  *Recycler un plastique en filament est possible, mais la matière doit être triée, propre et régulière. C’est un bon lien avec l’économie circulaire.*

* **Bio-impression et assemblage robotique** — [Panorama de la bio-impression](https://www.aniwaa.com/buyers-guide/3d-printers/3d-bioprinting-3d-bioprinters/) · [Robots assembleurs — MIT](https://news.mit.edu/2022/assembler-robots-structures-voxels-1122)  
  *Ces pistes montrent que la fabrication additive dépasse l’objet plastique : tissus biologiques, matériaux programmables et grandes structures assemblées par des robots.*

## Du modèle au fichier imprimable

* **Formats 3MF et STEP** — [Consortium 3MF](https://3mf.io/) · [Format STEP — NIST](https://www.nist.gov/ctl/smart-connected-systems-division/smart-connected-manufacturing-systems-group/step-nist)  
  *Le STEP conserve une géométrie CAO exploitable. Le 3MF transporte un projet d’impression avec unités et réglages. Ils sont souvent préférables au vieux STL.*

* **Préparer l’impression dans Bambu Studio** — [Télécharger Bambu Studio](https://bambulab.com/en/download/studio) · [Documentation Bambu Studio](https://wiki.bambulab.com/en/software/bambu-studio)  
  *Le slicer découpe le modèle en couches et calcule les mouvements. Avant d’imprimer, on vérifie l’orientation, le temps, la matière et l’aperçu couche par couche.*

* **Partager et trouver des modèles** — [Printables](https://www.printables.com) · [Thingiverse](https://www.thingiverse.com/) · [Sketchfab](https://sketchfab.com/)  
  *Télécharger un modèle fait gagner du temps, mais il faut vérifier sa licence, ses dimensions et s’il a vraiment été conçu pour être imprimé.*

## Onshape et prise de mesure

* **Ressources Onshape pour les étudiants** — [Parcours étudiants Onshape](https://www.onshape.com/en/education/student-resources) · [Créer un compte Éducation](https://www.onshape.com/en/education/sign-up)  
  *Onshape fonctionne dans le navigateur et enregistre automatiquement. Premier objectif : une esquisse contrainte, une extrusion, puis une modification de cote.*

* **Exporter depuis Onshape** — [Aide officielle : exporter des fichiers](https://cad.onshape.com/help/Content/exporting-files.htm)  
  *On conserve le document Onshape comme source modifiable, puis on exporte une copie pour le slicer. Toujours vérifier les unités et le format.*

* **Mesurer avec un pied à coulisse** — [Tutoriel vidéo en français](https://www.youtube.com/watch?v=KWOM6_AJVSA)  
  *Nettoyer les surfaces, fermer doucement, vérifier le zéro et mesurer plusieurs fois. La cote utile doit aussi répondre à une fonction dans l’assemblage.*

## Source

* [3D Scanning and Printing — Neil Gershenfeld, MIT Center for Bits and Atoms](https://academy.cba.mit.edu/classes/scanning_printing/index.html)  
  *Liste adaptée au niveau première année et au projet de VU-mètre.*
