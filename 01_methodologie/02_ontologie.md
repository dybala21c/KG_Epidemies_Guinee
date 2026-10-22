# Ontologie du KG Épidémies Guinée

**Version** : 1.0
**Date** : 2026-10-22
**Auteur** : Mamady Lamine Condé
**Statut** : Document fondateur de la Phase 2

---

## 1. Vue d'ensemble

L'ontologie définit **ce qui peut exister** dans le KG et **comment les entités sont reliées**. Sans ontologie, le KG serait un ensemble de triplets sans structure, difficile à interroger et à réutiliser.

L'ontologie du KG Épidémies Guinée est **volontairement simple** : elle compte **10 types d'entités** et **8 familles de relations**. Cette simplicité est un choix : elle garantit que le KG reste lisible par des non-spécialistes (chercheurs, décideurs, ONG).

---

## 2. Types d'entités

Le KG reconnaît **10 types d'entités**. Chaque entité est identifiée par un **identifiant unique** (en snake_case, sans accents).

### 2.1 `epidemie`
Une épidémie documentée.

**Exemples** :
- `epidemie_Ebola_2014_Guinee`
- `epidemie_COVID-19_Guinee`
- `epidemie_Lassa_2021_Guinee`
- `epidemie_Mpox_2025_Guinee`

**Attributs typiques** : date de début, date de fin, nombre de cas, nombre de décès, taux de létalité, localisation.

### 2.2 `maladie`
Une maladie infectieuse.

**Exemples** :
- `Ebola`
- `COVID-19`
- `Lassa`
- `Marburg`
- `Mpox`
- `Diphterie`
- `Rougeole`
- `Rubeole`
- `Meningite`
- `Rage`

### 2.3 `acteur`
Un acteur institutionnel ou organisationnel.

**Exemples** :
- `OMS`
- `MSF`
- `CDC`
- `UNICEF`
- `ANSS`
- `Croix_Rouge_francaise`
- `ALIMA`
- `USAID_OFDA`
- `Banque_Mondiale`

### 2.4 `institution`
Une institution guinéenne.

**Exemples** :
- `ANSS` (Agence Nationale de Sécurité Sanitaire)
- `MoH_Guinee` (Ministère de la Santé)
- `Cellule_nationale_lutte_contre_Ebola`
- `CNRD`
- `Conseil_scientifique_riposte_coronavirus`
- `INSP`
- `One_Health_Platform_Guinee`

### 2.5 `lieu`
Un lieu géographique.

**Exemples** :
- `Guinee`
- `Conakry`
- `Gueckedou`
- `Macenta`
- `Nzerekore`
- `Kankan`
- `Faranah`
- `Lola`
- `Forecariah`
- `Boke`

### 2.6 `ETC`
Un Ebola Treatment Centre (ou CT-Epi, ou structure de soins).

**Exemples** :
- `ETC_Donka`
- `ETC_Gueckedou`
- `ETC_Nongo_Conakry`
- `ETC_Kailahun`
- `ETC_Bo`
- `ETC_ELWA3_Monrovia`
- `CT_Epi_Siguiri`

### 2.7 `date`
Une date ou période.

**Exemples** :
- `decembre_2013`
- `mars_2014`
- `17_mars_2016`
- `4_juillet_2016`
- `12_mars_2020`
- `14_fevrier_2021`

### 2.8 `indicateur`
Un indicateur quantitatif (chiffre, pourcentage, taux).

**Exemples** :
- `2543` (nombre de décès Ebola)
- `51_pourcent` (mortalité moyenne ETC MSF)
- `75_pourcent` (taux de létalité Lassa)
- `1126` (nombre de triplets)

### 2.9 `lecon`
Une leçon apprise.

**Exemples** :
- `lecon_Ebola_2014`
- `lecon_MSF_Ebola`
- `lecon_transversale_S6`
- `lecon_CBS_S6`

### 2.10 `recommandation`
Une recommandation formulée.

**Exemples** :
- `recommandation_MSF`
- `recommandation_respondants`
- `recommandation_chercheurs`
- `recommandation_transversale_S6`

---

## 3. Types de relations

Le KG reconnaît **8 familles de relations**. Chaque relation est nommée en snake_case et commence par un verbe.

### 3.1 Famille `a_pour_*` — Attribution
Relie une entité à un attribut ou une valeur.

**Exemples** :
- `a_pour_nombre_cas` → 3811
- `a_pour_nombre_deces` → 2543
- `a_pour_taux_letalite` → 67_pourcent
- `a_pour_periode_debut` → fin_2013
- `a_pour_date_premier_cas_confirme` → mars_2014

### 3.2 Famille `a_impacte_*` — Impact
Relie une épidémie à ses conséquences.

**Exemples** :
- `a_impacte` → services_sante
- `a_impacte_cesariennes` → -75%
- `a_impacte_vaccination` → campagnes_annulees
- `a_impacte_polio` → echantillons_non_transportes

### 3.3 Famille `a_conduit_a_*` — Causalité
Relie un fait à sa conséquence directe.

**Exemples** :
- `a_conduit_a_retrait` → armee_de_la_reponse
- `a_conduit_a_implication` → anthropologues
- `a_conduit_a_creation` → ANSS
- `a_conduit_a` → nouveau_systeme_surveillance_DHIS2

### 3.4 Famille `a_ete_*` — État
Relie une entité à un état ou un statut.

**Exemples** :
- `a_ete` → urgence_sanitaire_la_plus_memorabe
- `a_ete_cible_de` → jets_de_pierres
- `a_ete_accuse_de` → propager_Ebola_pour_argent
- `a_ete_contenue_dans` → 1_district_4_mois

### 3.5 Famille `a_pour_*` (opérateurs) — Opérateurs
Relie une épidémie à ses opérateurs.

**Exemples** :
- `a_pour_operateur_ETU` → MSF
- `a_pour_financeur_ETU` → USAID_OFDA
- `a_pour_pilier_soins` → MSF
- `a_pour_coordination_nationale` → cellules_nationales_Ebola

### 3.6 Famille `inclut_*` / `comprenait_*` — Composition
Relie une entité à ses composants.

**Exemples** :
- `inclut` → maintien_mesures_IPC
- `inclut` → messages_education_sante_publique_plus_forts
- `comprenaient` → symptomatique_support_rehydratation
- `comprenait` → ETC_mobilisation_communautaire_HP_kits

### 3.7 Famille `correspond_a_*` — Correspondance
Relie deux entités équivalentes ou parallèles.

**Exemples** :
- `correspond_a` → declaration_epidemie_Guinee_mars_avril_2014
- `correspond_a` → propagation_pays_voisins_mai_juillet_2014
- `correspond_a` → pic_cas_aout_octobre_2014

### 3.8 Famille `est_*` — Définition
Relie une entité à sa définition ou sa nature.

**Exemples** :
- `est` → isolement_et_soins_supportifs
- `est` → enterrements_securises
- `est` → creation_ANSS
- `est` → manque_appropriation_concept_LHS
- `est_un_evenement_rare` → oui

---

## 4. Contraintes

### 4.1 Contraintes de cardinalité
- Une `epidemie` peut avoir **plusieurs** `a_pour_nombre_cas` (si plusieurs sources).
- Une `epidemie` a **un seul** `a_pour_periode_debut` (la première date connue).
- Un `ETC` a **un seul** `a_pour_localisation`.
- Une `lecon` peut avoir **plusieurs** `inclut`.

### 4.2 Contraintes de cohérence
- Un triplet `a_pour_nombre_deces` doit être **numérique** (pas de texte).
- Un triplet `a_pour_periode_debut` doit être une **date** (pas un événement).
- Un triplet `a_impacte` doit relier une **épidémie** à un **service** ou **indicateur**.

### 4.3 Contraintes de traçabilité
- Chaque triplet doit avoir **une source** (S1 à S10).
- Chaque triplet doit avoir **une page**.
- Chaque triplet doit avoir **une citation exacte**.

### 4.4 Contraintes de nommage
- Les identifiants sont en **snake_case** (ex. `epidemie_Ebola_2014_Guinee`).
- Les identifiants sont **sans accents** (ex. `Gueckedou` et non `Guéckédou`).
- Les identifiants sont **en français** (ex. `a_pour_nombre_deces` et non `has_number_of_deaths`).

---

## 5. Exemples de triplets valides

Voici **5 exemples** de triplets valides, avec leur type d'entité et de relation :

| Head | Type Head | Relation | Type Relation | Tail | Type Tail |
|---|---|---|---|---|---|
| `epidemie_Ebola_2014_Guinee` | epidemie | `a_pour_nombre_deces` | attribution | `2543` | indicateur |
| `epidemie_Ebola_2014_Guinee` | epidemie | `a_impacte` | impact | `services_sante` | indicateur |
| `ANSS` | institution | `creee_le` | attribution | `4_juillet_2016` | date |
| `ETC_Donka` | ETC | `a_recu_IV_fluides_pour` | attribution | `76_pourcent_patients_mars_avril_2014` | indicateur |
| `lecon_MSF_Ebola` | lecon | `investissement_precoce_dans` | recommandation | `acceptabilite_communautaire_changement_comportement` | indicateur |

---

## 6. Conclusion

L'ontologie du KG Épidémies Guinée est **simple mais rigoureuse** : 10 types d'entités, 8 familles de relations, 4 contraintes. Elle garantit que le KG est :
- **Lisible** : chaque entité a un type clair
- **Interrogeable** : chaque relation suit une logique
- **Extensible** : on peut ajouter de nouveaux types si nécessaire
- **Réutilisable** : d'autres chercheurs peuvent comprendre la structure

---

**Prochaine étape** : Documentation de la justification des relations (Phase 2, Chantier 3).
