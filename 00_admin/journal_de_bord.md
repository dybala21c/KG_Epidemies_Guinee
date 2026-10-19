## 2026-10-15 — Phase 1, Étape 1 : Sources téléchargées

### Actions
- Structure projet créée et validée
- 10 sources épidémies téléchargées (S1 à S10)
- Index des sources rempli
- Checklist des sources remplie

### Sources disponibles
- Ebola : S1 (CDC), S2 (MSF), S3 (PLOS)
- Leçons : S4 (BMJ), S5 (Maltais), S6 (Hemingway-Foday)
- Surveillance : S7 (ANSS bulletins), S10 (ANSS Mpox)
- Multi-épidémies : S8 (UNICEF), S9 (UN)

### Blocages
- Aucun

### Prochaine session
- Lire S1 (CDC) en priorité
- Extraire 10 premiers triplets Ebola
- Remplir kg_sources.md avec les traçabilités


## 2026-10-17 — Phase 1, Étape 1 : Noyau Ebola v1 extrait (70 triplets)

### Actions
- Lecture intégrale de S1 (CDC Ebola Response 2014-2016, 9 pages)
- Extraction de 70 triplets Guinée, tous tracés (page + citation exacte)
- Création de kg_epidemies_v1_2026-10-17.tsv (70 lignes)
- Création de kg_sources.md (70 lignes de traçabilité)

### Répartition des triplets
- Origine et chronologie : 6
- Chiffres clés (TABLE p.4) : 4
- Réponse internationale et piliers : 6
- Opérateurs ETU : 7
- Réticence et résistance communautaire : 6
- Stratégie Guinée : 8
- Approche cerclage : 8
- Fin de l'épidémie et résurgence : 4
- Impact sur les services de santé : 4
- Leçons apprises : 4
- Ressources humaines CDC : 4
- Dépistage et surveillance : 3
- Contexte global : 6

### Statut de validation
- 70 triplets confirmés (citation exacte + page)
- 0 triplet à vérifier
- 0 triplet faux
- Aucun triplet inventé

### Blocages
- Aucun

### Prochaine session
- Passer à S2 (MSF Ebola Review 2014-2015) pour enrichir le noyau
- Extraire les triplets MSF (opérations terrain, ETU, leçons)
- Fusionner avec le KG v1 Ebola
- Objectif : atteindre 100+ triplets Ebola avant l'automatisation LLM

### Commit Git
- feat(kg): noyau Ebola v1 — 70 triplets traces CDC


## 2026-10-18 — Phase 1, Étape 2 : Enrichissement S2 (OCB Ebola Review Part 1)

### Actions
- Lecture intégrale de S2 (OCB Ebola Review Part 1: Medico-operational, 78 pages)
- Analyse des tableaux et figures : Fig.1 (cas/semaine par pays), Fig.2 (timeline OCB), Fig.3 (Guinée), Fig.4 (Liberia), Fig.5 (Sierra Leone), Fig.6 (IV fluids Foya), Fig.7 (survie Foya), Fig.8 (CFR par mois/ETC), Tableau 1 (traitement Foya), Annexes V (timelines HP par site)
- Extraction de 218 triplets validés (S2-01 à S2-218), tous tracés (page + citation exacte)
- Application du cadrage : Priorité A (Guinée systématique) + Priorité B sélective (Liberia/SL si éclaire la Guinée) + Priorité C ignorée

### Répartition des triplets S2
- Executive Summary : 20
- Background / ToR / Méthodo : 21
- Stratégie MSF et Guinée : 27
- Liberia / Sierra Leone (comparatif) : 21
- Timeliness / Patient Care : 37
- HP / Outreach / Non-Ebola / Épidémio / Recherche : 44
- Conclusions / Recommandations : 48

### Statut de validation
- 218 triplets confirmés (citation exacte + page)
- 26 triplets rejetés du Bloc 1 initial (interprétations évaluatives, recommandations, génériques MSF sans ancrage Guinée)
- 0 triplet inventé

### Blocages
- Aucun

### Prochaine session
- Passer à S3 (PLOS Impact services de santé) pour enrichir le KG sur l'impact santé
- Objectif : atteindre 300+ triplets avant l'automatisation LLM

### Commit Git
- feat(kg): enrichissement S2 — 218 triplets traces OCB Ebola Review


## 2026-10-18 — Phase 1, Étape 3 : Enrichissement S3 (UNICEF Guinée 2021)

### Actions
- Lecture intégrale de S3 (UNICEF Guinea Humanitarian Situation Report No. 2, 9 pages)
- Analyse des tableaux et figures : Highlights p.1, Situation Overview p.2-3, Summary Analysis p.3-5, Annexes A (résultats) et B (funding) p.8-9
- Extraction de 151 triplets validés (S3-01 à S3-151), tous tracés (page + citation exacte)
- Application du cadrage : Priorité A (Guinée systématique) + Priorité B sélective (régional si éclaire le national) + Priorité C ignorée (partenaires, financeurs, médias, contacts)

### Répartition des triplets S3
- Highlights + Situation Overview : 52
- Santé + Nutrition : 25
- Protection / Éducation / WASH : 37
- C4D / RCCE / Coordination : 16
- Annexes A + B : 21

### Statut de validation
- 151 triplets confirmés (citation exacte + page)
- 0 triplet rejeté
- 0 triplet inventé

### Blocages
- Aucun

### Prochaine session
- Passer à S4 (PLOS Impact services de santé ou BMJ Millimouno 2023, selon choix)
- Objectif : atteindre 500+ triplets avant l'automatisation LLM

### Commit Git
- feat(kg): enrichissement S3 — 151 triplets traces UNICEF Guinee 2021


## 2026-10-18 — Phase 1, Étape 4 : Enrichissement S4 (PLOS Currents Outbreaks 2015)

### Actions
- Lecture intégrale de S4 (Barden-O'Fallon et al., Rapid Assessment of Ebola-Related Implications for RMNCH Service Delivery and Utilization in Guinea, 4 août 2015, 17 pages)
- Analyse des tableaux 1, 2, 3 et figures 1-4
- Extraction de 98 triplets validés (S4-01 à S4-98), tous tracés (page + citation exacte)
- Application du cadrage : Priorité A (Guinée systématique) + Priorité B sélective (Sierra Leone, Liberia, projections régionales) + Priorité C ignorée (financement, acknowledgements, références, liens)

### Répartition des triplets S4
- Contexte / Background : 22
- Table 1 (indicateurs significatifs) : 12
- Figs 1-4 + Stockouts : 11
- Table 2 (directeurs) : 17
- Table 3 (prestataires) : 12
- Verbatims + Conclusions + Priorité B : 24

### Statut de validation
- 98 triplets confirmés (citation exacte + page)
- 0 triplet rejeté
- 0 triplet inventé

### Blocages
- Aucun

### Prochaine session
- Passer à S5 (BMJ Millimouno 2023 ou Maltais 2022 Résilience, selon choix)
- Objectif : atteindre 600+ triplets avant l'automatisation LLM

### Commit Git
- feat(kg): enrichissement S4 — 98 triplets traces PLOS RMNCH Guinea 2015


## 2026-10-18 — Phase 1, Étape 5 : Enrichissement S5 (BMJ Global Health 2023, Millimouno)

### Actions
- Lecture intégrale de S5 (Millimouno et al., How has Guinea learnt from the response to outbreaks? A learning health system analysis. BMJ Global Health 2023;8:e010996, 22 pages)
- Analyse des Tableaux 1, 2, 3, 4, 5 et des figures 1-3
- Extraction de 188 triplets validés (S5-01 à S5-188), tous tracés (page + citation exacte)
- Application du cadrage : Priorité A (Guinée systématique) + Priorité B sélective (comparaisons internationales LHS si éclairent la Guinée) + Priorité C ignorée (références, acknowledgements, funding, méthodes détaillées, Box 4)

### Répartition des triplets S5
- Contexte / Setting : 22
- Ebola 2014-2016 + autres épidémies : 18
- EVD 2021 + Marburg 2021 : 24
- Table 1 (Leçons Ebola 2014-2016) : 26
- Table 2 (Incorporation) : 13
- Table 3 (Enablers/Barriers) : 35
- Tables 4 + 5 (Recommandations) : 29
- Discussion + Conclusion : 21

### Statut de validation
- 188 triplets confirmés (citation exacte + page)
- 0 triplet rejeté
- 0 triplet inventé

### Blocages
- Aucun

### Prochaine session
- Passer à S6 (Maltais 2022 Résilience ou Hemingway-Foday 2022 Surveillance, selon choix)
- Objectif : atteindre 800+ triplets avant l'automatisation LLM

### Commit Git
- feat(kg): enrichissement S5 — 188 triplets traces BMJ LHS Guinea 2023


## 2026-10-18 — Phase 1, Étape 6 : Enrichissement S6 (Hemingway-Foday 2022, surveillance post-Ebola)

### Actions
- Lecture intégrale de S6 (Hemingway-Foday et al., Lessons learned for surveillance system strengthening through capacity building and partnership engagement in post-Ebola Guinea, 2015–2019. Frontiers in Public Health 10:715356, 15 pages)
- Analyse des Tableaux 1 (activités stratégiques), 2 (maladies prioritaires IDSR), 3 (leçons/recommandations)
- Extraction de 144 triplets validés (S6-01 à S6-144), tous tracés (page + citation exacte)
- Application du cadrage : Priorité A (Guinée systématique) + Priorité B sélective (comparaisons régionales Sierra Leone, Liberia, Côte d'Ivoire, Guinée-Bissau, Sénégal) + Priorité C ignorée (funding, acknowledgments, références, author contributions, disclaimer)

### Répartition des triplets S6
- Introduction + Methods : 18
- CBS (Community-Based Surveillance) : 20
- Points of Entry (PoE) : 13
- IDSR strengthening : 21
- DHIS 2 / SurvEpi : 18
- Tables 2 + 3 : 39
- Discussion + Conclusion : 15

### Statut de validation
- 144 triplets confirmés (citation exacte + page)
- 0 triplet rejeté
- 0 triplet inventé

### Blocages
- Aucun

### Prochaine session
- Passer à S7 (Maltais 2022 Résilience post-Ebola et COVID-19)
- Objectif : atteindre 1000+ triplets avant l'automatisation LLM

### Commit Git
- feat(kg): enrichissement S6 — 144 triplets traces surveillance post-Ebola Guinea 2015-2019


## 2026-10-18 — Phase 1, Étape 7 : Enrichissement S7 (Maltais 2022, résilience post-Ebola)

### Actions
- Lecture intégrale de S7 (Maltais, Brière, Yaya, Comment la résilience post-Ebola en Guinée contribue à la gestion de la COVID-19 ? Santé Publique 2022/4 Vol. 34, p. 557-567, 11 pages)
- Analyse des Tableaux I (modèle Kruk), II (provenance gestionnaires), III (cadre d'analyse), IV (pointages), V (résilience par période)
- Extraction de 140 triplets validés (S7-01 à S7-140), tous tracés (page + citation exacte)
- Application du cadrage : Priorité A (Guinée systématique) + Priorité B sélective (comparaisons internationales Kruk) + Priorité C ignorée (références bibliographiques, conflits d'intérêts, remerciements, métadonnées Cairn)

### Répartition des triplets S7
- Introduction + Matériels et méthodes : 21
- Intégration + Diversité : 25
- Ressources humaines + Conscience + Autorégulation : 33
- Adaptabilité + Discussion : 28
- Tableau V (résilience par période) : 33

### Statut de validation
- 140 triplets confirmés (citation exacte + page)
- 0 triplet rejeté
- 0 triplet inventé

### Blocages
- Aucun

### Prochaine session
- Passer à S8 (ANSS Bulletins S27-S29)
- Objectif : consolider le noyau Lassa (2020-2026)

### Commit Git
- feat(kg): enrichissement S7 — 140 triplets traces resilience post-Ebola Guinea 2022


## 2026-10-18 — Phase 1, Étape 8 : Enrichissement S8 (ANSS Bulletins S27-S29, 2026)

### Actions
- Lecture intégrale des bulletins ANSS S27 (09/07/2026), S28 (16/07/2026) et S29 (23/07/2026)
- Analyse des tableaux, figures et cartes de surveillance épidémiologique
- Extraction de 73 triplets validés (S8-01 à S8-73), tous tracés (page + citation exacte)
- Application du cadrage : Priorité A (Guinée systématique) + Priorité C ignorée (logos, partenaires, photos)

### Répartition des triplets S8
- Vue d'ensemble des épidémies : 5
- Fièvre de Lassa : 8
- Diphtérie : 7
- Mpox : 11
- Rougeole/Rubéole : 6
- Autres MPE : 7
- COVID-19/Paludisme : 8
- Zoonoses (rage, morsures) : 11
- PoE/Événements : 10

### Statut de validation
- 73 triplets confirmés (citation exacte + page)
- 0 triplet rejeté
- 0 triplet inventé

### Blocages
- Aucun

### Prochaine session
- Passer à S9 (UN Guinée gestion urgences) ou S10 (ANSS Mpox 2025)
- Objectif : consolider le noyau COVID-19 et Mpox

### Commit Git
- feat(kg): enrichissement S8 — 73 triplets traces bulletins ANSS S27-S29 2026


## 2026-10-18 — Phase 1, Étape 9 : Enrichissement S9 (Nations Unies Guinée 2022)

### Actions
- Lecture intégrale de S9 (Nations Unies Guinée, "La Guinée s'appuie sur son expérience pour une gestion optimale des urgences sanitaires", 28 novembre 2022, 9 pages)
- Analyse des sections narratives et du témoignage officiel
- Extraction de 32 triplets validés (S9-01 à S9-32), tous tracés (page + citation exacte)
- Application du cadrage : Priorité A (Guinée systématique) + Priorité C ignorée (photos, logos, liens institutionnels)

### Répartition des triplets S9
- Contexte et institutionnalisation : 5
- Forum national : 2
- Témoignage survivants : 9
- Mesures et One Health : 6
- Résurgence Ebola et COVID-19 : 4
- Résultats et financement : 6

### Statut de validation
- 32 triplets confirmés (citation exacte + page)
- 0 triplet rejeté
- 0 triplet inventé

### Blocages
- Aucun

### Prochaine session
- Passer à S10 (ANSS Mpox 2025) pour finaliser la Phase 1
- Objectif : consolider le noyau Mpox et clôturer la Phase 1

### Commit Git
- feat(kg): enrichissement S9 — 32 triplets traces Nations Unies Guinee 2022


## 2026-10-18 — Phase 1, Étape 10 : Enrichissement S10 (Journal Horoya, Mpox 2025)

### Actions
- Lecture intégrale de S10 (Journal Horoya, "MPOX en Guinée : L'ANSS met en garde contre une recrudescence des cas", 22 juillet 2025)
- Analyse du communiqué officiel de l'ANSS (Bilan du 21 juillet 2025)
- Extraction de 12 triplets validés (S10-01 à S10-12), tous tracés (page + citation exacte)
- Application du cadrage : Priorité A (Guinée systématique) + Priorité C ignorée (publicités, navigation, autres articles de presse)

### Répartition des triplets S10
- Situation épidémiologique Mpox : 9
- Réponse et zones à haut risque : 3

### Statut de validation
- 12 triplets confirmés (citation exacte + page)
- 0 triplet rejeté
- 0 triplet inventé

### Blocages
- Aucun

### Prochaine session
- **Phase 1 terminée : 10/10 sources traitées.**
- Bilan final de la Phase 1 à produire.
- Passage à la **Phase 2 — Explicabilité avancée** (à planifier).

### Commit Git
- feat(kg): enrichissement S10 — 12 triplets traces Journal Horoya Mpox 2025