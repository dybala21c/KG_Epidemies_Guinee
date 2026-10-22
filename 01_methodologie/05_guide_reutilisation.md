# Guide de réutilisation — KG Épidémies Guinée

**Version** : 1.0
**Date** : 2026-10-22
**Auteur** : Mamady Lamine Condé
**Statut** : Document fondateur de la Phase 2

---

## 1. À qui s'adresse ce guide

Le KG Épidémies Guinée est destiné à **4 publics** :

### 1.1 Chercheurs
Épidémiologistes, historiens, sociologues, politistes qui étudient les épidémies en Guinée.

**Ce qu'ils peuvent faire** : analyser les données, comparer les épidémies, tester des hypothèses.

### 1.2 Décideurs
Responsables politiques, autorités sanitaires, gestionnaires de crise.

**Ce qu'ils peuvent faire** : comprendre les leçons apprises, anticiper les crises, planifier les ripostes.

### 1.3 ONG et organisations internationales
MSF, OMS, UNICEF, Croix-Rouge, etc.

**Ce qu'elles peuvent faire** : cibler leurs interventions, coordonner leurs actions, évaluer leurs impacts.

### 1.4 Grand public
Journalistes, étudiants, citoyens intéressés.

**Ce qu'ils peuvent faire** : comprendre les épidémies, vérifier des faits, s'informer.

---

## 2. Comment interroger le KG

Le KG est stocké dans deux fichiers :
- `kg_epidemies_v1_2026-10-18.tsv` (3 colonnes : Head, Relation, Tail)
- `kg_sources.md` (7 colonnes : #, Head, Relation, Tail, Source, Page, Citation)

### 2.1 Requêtes simples (par entité)
Pour trouver tous les triplets liés à une entité, cherche son nom dans le TSV :

```bash
grep "epidemie_Ebola_2014_Guinee" kg_epidemies_v1_2026-10-18.tsv
Résultat : tous les triplets qui concernent l'épidémie Ebola 2014 en Guinée.


### 2.2 Requêtes par relation
Pour trouver tous les triplets qui utilisent une relation donnée :

```bash
grep "a_pour_nombre_deces" kg_epidemies_v1_2026-10-18.tsv
Résultat : Tous les triplets qui attribuent un nombre de décès (ex. epidemie_Ebola_2014_Guinee a_pour_nombre_deces 2543, epidemie_Ebola_Guinee_2014_2016 a_pour_nombre_deces 2544, etc.).
