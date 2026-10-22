# Index des entités et relations — KG Épidémies Guinée

**Version** : 1.0
**Date** : 2026-10-22
**Auteur** : Mamady Lamine Condé
**Statut** : Document fondateur de la Phase 2

---

## 1. Vue d'ensemble

Ce document recense **toutes les entités** et **toutes les relations** utilisées dans le KG Épidémies Guinée. Il sert de **répertoire** pour les utilisateurs qui souhaitent savoir :
- Quelles entités existent dans le KG
- Quelles relations sont utilisées
- Combien de fois chaque entité/relation apparaît

---

## 2. Index des entités (par type)

### 2.1 Épidémies
| Entité | Nombre d'occurrences |
|---|---|
| `epidemie_Ebola_2014_Guinee` | ~70 |
| `epidemie_Ebola_2013_2014_Guinee` | ~10 |
| `epidemie_Ebola_2014_2016_Guinee` | ~20 |
| `epidemie_Ebola_2021_Guinee` | ~15 |
| `epidemie_COVID-19_Guinee` | ~40 |
| `epidemie_Lassa_2021_Guinee` | ~5 |
| `epidemie_Marburg_2021_Guinee` | ~10 |
| `epidemie_Mpox_Guinee_2025` | ~12 |
| `epidemie_Mpox_Guinee_2026` | ~5 |

### 2.2 Institutions
| Entité | Nombre d'occurrences |
|---|---|
| `ANSS` | ~30 |
| `MoH_Guinee` | ~10 |
| `Cellule_nationale_lutte_contre_Ebola` | ~8 |
| `CNRD` | ~1 |
| `Conseil_scientifique_riposte_coronavirus` | ~2 |
| `INSP` | ~2 |
| `One_Health_Platform_Guinee` | ~2 |

### 2.3 Acteurs
| Entité | Nombre d'occurrences |
|---|---|
| `MSF` | ~40 |
| `OMS` | ~25 |
| `CDC` | ~20 |
| `UNICEF` | ~15 |
| `Croix_Rouge_francaise` | ~5 |
| `ALIMA` | ~3 |
| `USAID_OFDA` | ~2 |
| `Banque_Mondiale` | ~1 |

### 2.4 Lieux
| Entité | Nombre d'occurrences |
|---|---|
| `Guinee` | ~20 |
| `Conakry` | ~15 |
| `Gueckedou` | ~10 |
| `Macenta` | ~5 |
| `Nzerekore` | ~8 |
| `Kankan` | ~3 |
| `Faranah` | ~3 |
| `Lola` | ~2 |
| `Forecariah` | ~2 |
| `Boke` | ~2 |

### 2.5 ETC
| Entité | Nombre d'occurrences |
|---|---|
| `ETC_Donka` | ~10 |
| `ETC_Gueckedou` | ~8 |
| `ETC_Nongo_Conakry` | ~5 |
| `ETC_Kailahun` | ~5 |
| `ETC_Bo` | ~3 |
| `ETC_ELWA3_Monrovia` | ~3 |
| `CT_Epi_Siguiri` | ~2 |

### 2.6 Leçons
| Entité | Nombre d'occurrences |
|---|---|
| `lecon_Ebola_2014` | ~4 |
| `lecon_MSF_Ebola` | ~10 |
| `lecon_transversale_S6` | ~3 |
| `lecon_CBS_S6` | ~4 |

### 2.7 Recommandations
| Entité | Nombre d'occurrences |
|---|---|
| `recommandation_MSF` | ~10 |
| `recommandation_respondants` | ~15 |
| `recommandation_chercheurs` | ~14 |
| `recommandation_transversale_S6` | ~4 |

---

## 3. Index des relations (par famille)

### 3.1 Famille `a_pour_*` (Attribution)
| Relation | Nombre d'occurrences |
|---|---|
| `a_pour_nombre_cas` | ~10 |
| `a_pour_nombre_deces` | ~10 |
| `a_pour_taux_letalite` | ~8 |
| `a_pour_periode_debut` | ~5 |
| `a_pour_periode_fin` | ~2 |
| `a_pour_date_premier_cas_confirme` | ~3 |
| `a_pour_operateur_ETU` | ~5 |
| `a_pour_financeur_ETU` | ~2 |
| `a_pour_pilier_soins` | ~1 |

### 3.2 Famille `a_impacte_*` (Impact)
| Relation | Nombre d'occurrences |
|---|---|
| `a_impacte` | ~2 |
| `a_impacte_cesariennes` | ~1 |
| `a_impacte_vaccination` | ~1 |
| `a_impacte_polio` | ~1 |

### 3.3 Famille `a_conduit_a_*` (Causalité)
| Relation | Nombre d'occurrences |
|---|---|
| `a_conduit_a` | ~5 |
| `a_conduit_a_creation` | ~2 |
| `a_conduit_a_retrait` | ~1 |
| `a_conduit_a_implication` | ~1 |

### 3.4 Famille `a_ete_*` (État)
| Relation | Nombre d'occurrences |
|---|---|
| `a_ete` | ~1 |
| `a_ete_cible_de` | ~1 |
| `a_ete_accuse_de` | ~1 |
| `a_ete_contenue_dans` | ~2 |

### 3.5 Famille `inclut_*` / `comprenait_*` (Composition)
| Relation | Nombre d'occurrences |
|---|---|
| `inclut` | ~8 |
| `comprenaient` | ~2 |
| `comprenait` | ~1 |

### 3.6 Famille `correspond_a_*` (Correspondance)
| Relation | Nombre d'occurrences |
|---|---|
| `correspond_a` | ~5 |

### 3.7 Famille `est_*` (Définition)
| Relation | Nombre d'occurrences |
|---|---|
| `est` | ~20 |
| `est_un_evenement_rare` | ~1 |

---

## 4. Conclusion

Le KG Épidémies Guinée contient :
- **~9 épidémies** documentées
- **~7 institutions** guinéennes
- **~8 acteurs** internationaux
- **~10 lieux** géographiques
- **~7 ETC** (centres de traitement)
- **~4 leçons** principales
- **~4 ensembles de recommandations**

Les relations les plus utilisées sont :
- `a_pour_*` (attribution) : ~50 occurrences
- `est_*` (définition) : ~21 occurrences
- `inclut_*` (composition) : ~11 occurrences

Cet index permet de **naviguer** dans le KG et de **comprendre** sa structure.

---

**Prochaine étape** : Synthèse finale de la Phase 2 (bilan et validation).