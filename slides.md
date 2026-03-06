# Les Permissions Avancées dans Grist
Sécuriser et gérer finement l'accès à vos données

---

## 1. Les niveaux d'accès de base
Avant d'aller plus loin, Grist propose 3 niveaux d'accès standards [1] :
*   **Propriétaire (Owner)** : Contrôle le document et l'ajout de nouveaux utilisateurs [1].
*   **Éditeur (Editor)** : Peut modifier les données du document [1].
*   **Lecteur (Viewer)** : Peut uniquement lire et consulter les données [1].
*   Ces règles générales peuvent s'appliquer à chaque niveau de l'arborescence : l'espace d'équipe, le dossier ou le document [2].

---

## 2. La puissance des droits granulaires
Contrairement à un tableur classique, Grist permet une personnalisation des accès à une maille extrêmement fine [1] :
*   **Contrôle au niveau de la table** : Restreindre l'accès à une base de données entière.
*   **Contrôle au niveau de la colonne** : Masquer des informations spécifiques au sein d'un tableau [1, 3].
*   **Contrôle au niveau de la ligne** : N'afficher que les enregistrements pertinents pour la personne connectée [1, 3].

---

## 3. Le système C.R.U.D.
Pour paramétrer ces droits avancés, Grist s'appuie sur la norme technique C.R.U.D. qui permet de séparer chaque type d'action [1] :
*   **[C]reate (Créer)** : Droit d'ajouter de nouvelles données.
*   **[R]ead (Lire)** : Droit d'afficher et de consulter la donnée.
*   **[U]pdate (Mettre à jour)** : Droit de modifier une information existante.
*   **[D]elete (Supprimer)** : Droit de supprimer des données.

---

## 4. Cas d'usages concrets
Grâce aux règles avancées, vous pouvez créer des outils sur-mesure et sécurisés :
*   **Filtrage métier** : Paramétrer le document pour qu'un agent ne puisse voir (Read) et modifier (Update) que les projets qui sont liés à son propre département [4].
*   **Saisie isolée** : Permettre à un utilisateur de soumettre de nouvelles données via un formulaire (Create) sans avoir la permission de lire (Read) celles des autres [3, 5].
*   **Protection API** : Restreindre l'accès d'un compte de service (robot) en lui masquant les lignes pour lesquelles la colonne "à cacher aux robots" est cochée [6].
