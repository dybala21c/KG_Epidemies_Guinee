# Justification des relations — KG Épidémies Guinée

**Version** : 1.0
**Date** : 2026-10-22
**Auteur** : Mamady Lamine Condé
**Statut** : Document fondateur de la Phase 2

---

## 1. Vue d'ensemble

Ce document justifie **chaque famille de relations** utilisée dans le KG Épidémies Guinée. Pour chaque famille, il précise :
- Sa **définition**
- Son **usage** dans le KG
- Un **exemple concret** (avec source et page)
- Son **niveau de confiance** (certain, probable, à vérifier)

Le niveau de confiance est défini ainsi :
- **Certain** : le fait est explicitement écrit dans la source, avec citation exacte.
- **Probable** : le fait est déduit d'une combinaison de sources, sans citation unique.
- **À vérifier** : le fait est rapporté par une source unique, non corroborée.

---

## 2. Famille `a_pour_*` — Attribution

**Définition** : Relie une entité à un **attribut** ou une **valeur** (chiffre, date, lieu, acteur).

**Usage** : C'est la famille la plus utilisée dans le KG. Elle permet de stocker les **caractéristiques** d'une entité.

**Exemples** :
- `epidemie_Ebola_2014_Guinee` → `a_pour_nombre_cas` → `3811` (S1, p.4)
- `epidemie_Ebola_2014_Guinee` → `a_pour_nombre_deces` → `2543` (S1, p.4)
- `epidemie_Ebola_2014_Guinee` → `a_pour_periode_debut` → `fin_2013` (S1, p.1)

**Niveau de confiance** : **Certain** (chaque triplet a une citation exacte).

---

## 3. Famille `a_impacte_*` — Impact

**Définition** : Relie une **épidémie** à ses **conséquences** sur les services de santé, l'économie, la société.

**Usage** : Cette famille permet de documenter les **effets indirects** des épidémies.

**Exemples** :
- `epidemie_Ebola_2014_Guinee` → `a_impacte` → `services_sante` (S1, p.7)
- `epidemie_Ebola_2014_Guinee` → `a_impacte_cesariennes` → `-75%` (S1, p.7)
- `epidemie_Ebola_2014_Guinee` → `a_impacte_vaccination` → `campagnes_annulees` (S1, p.7)

**Niveau de confiance** : **Certain** (chaque triplet a une citation exacte).

---

## 4. Famille `a_conduit_a_*` — Causalité

**Définition** : Relie un **fait** à sa **conséquence directe** ou à son **résultat**.

**Usage** : Cette famille permet de documenter les **chaînes causales** (ex. « la crise a conduit à la création de l'ANSS »).

**Exemples** :
- `Ebola_2014_2016_Guinee` → `a_conduit_a_creation` → `ANSS` (S5, p.5)
- `double_loop_learning_Guinee` → `a_conduit_a` → `creation_ANSS` (S5, p.17)
- `triple_loop_learning_Ebola_2014_2016` → `a_conduit_a` → `nouveau_systeme_surveillance_DHIS2` (S5, p.10)

**Niveau de confiance** : **Certain** (chaque triplet a une citation exacte).

---

## 5. Famille `a_ete_*` — État

**Définition** : Relie une entité à un **état** ou un **statut**.

**Usage** : Cette famille permet de documenter les **qualifications** (ex. « a été considéré comme », « a été accusé de »).

**Exemples** :
- `epidemie_Ebola_Guinee_2014_2016` → `a_ete` → `urgence_sanitaire_la_plus_memorabe` (S9, p.2)
- `hopital_Guinee_pendant_Ebola` → `a_ete_cible_de` → `jets_de_pierres` (S4, p.12)
- `personnel_sante_Guinee_pendant_Ebola` → `a_ete_accuse_de` → `propager_Ebola_pour_argent` (S4, p.12)

**Niveau de confiance** : **Certain** (chaque triplet a une citation exacte).

---

## 6. Famille `a_pour_*` (opérateurs) — Opérateurs

**Définition** : Relie une **épidémie** à ses **opérateurs** (acteurs, financeurs, piliers).

**Usage** : Cette famille permet de documenter **qui fait quoi** dans la riposte.

**Exemples** :
- `epidemie_Ebola_2014_Guinee` → `a_pour_operateur_ETU` → `MSF` (S1, p.4)
- `epidemie_Ebola_2014_Guinee` → `a_pour_financeur_ETU` → `USAID_OFDA` (S1, p.4)
- `epidemie_Ebola_2014_Guinee` → `a_pour_pilier_soins` → `MSF` (S1, p.4)

**Niveau de confiance** : **Certain** (chaque triplet a une citation exacte).

---

## 7. Famille `inclut_*` / `comprenait_*` — Composition

**Définition** : Relie une entité à ses **composants** (éléments, sous-parties).

**Usage** : Cette famille permet de documenter la **structure** d'une entité.

**Exemples** :
- `besoins_prioritaires_soignants_Guinee_pendant_Ebola` → `incluent` → `maintien_mesures_IPC` (S4, p.13)
- `soins_cliniques_MSF` → `comprenaient` → `symptomatique_support_rehydratation_antibio_antipaludique_nutrition_psychosocial` (S2, p.25)
- `intervention_Monrovia` → `comprenait` → `ETC_mobilisation_communautaire_HP_kits` (S2, p.17)

**Niveau de confiance** : **Certain** (chaque triplet a une citation exacte).

---

## 8. Famille `correspond_a_*` — Correspondance

**Définition** : Relie deux entités **équivalentes** ou **parallèles**.

**Usage** : Cette famille permet de documenter les **phases**, les **périodes** ou les **équivalences**.

**Exemples** :
- `phase_1` → `correspond_a` → `declaration_epidemie_Guinee_mars_avril_2014` (S2, p.9)
- `phase_2` → `correspond_a` → `propagation_pays_voisins_mai_juillet_2014` (S2, p.9)
- `phase_3` → `correspond_a` → `pic_cas_aout_octobre_2014` (S2, p.10)

**Niveau de confiance** : **Certain** (chaque triplet a une citation exacte).

---

## 9. Famille `est_*` — Définition

**Définition** : Relie une entité à sa **définition** ou à sa **nature**.

**Usage** : Cette famille permet de documenter les **définitions** (ex. « le pilier 1 est l'isolement »).

**Exemples** :
- `pilier_1` → `est` → `isolement_et_soins_supportifs` (S2, p.14)
- `pilier_2` → `est` → `enterrements_securises` (S2, p.14)
- `enabler_LHS_Guinee` → `est` → `creation_ANSS` (S5, p.11)

**Niveau de confiance** : **Certain** (chaque triplet a une citation exacte).

---

## 10. Conclusion

Les **8 familles de relations** du KG Épidémies Guinée sont toutes justifiées par :
- Une **définition** claire
- Un **usage** documenté
- Des **exemples** concrets (avec source et page)
- Un **niveau de confiance** explicite

Cette justification garantit que le KG est **explicable** : chaque relation peut être comprise, auditée et réutilisée.

---

**Prochaine étape** : Documentation des limites (Phase 2, Chantier 4).