# Rapport de Projet – Ethical Hacking

> Projet académique réalisé dans le cadre du module **Ethical Hacking** à l'EFREI Paris (Promotion 2028).

## ⚠️ Avertissement éthique et légal

Ce dépôt documente un **scénario pédagogique fictif**. Aucune action offensive décrite n'a été menée contre un système réel sans autorisation. L'entreprise ciblée, les collaborateurs et les comptes mentionnés dans le rapport sont **anonymisés / fictifs** ; toute ressemblance avec des personnes ou organisations réelles serait fortuite.

Les techniques présentées (OSINT, ingénierie sociale, phishing, macro malveillante, deepfake vocal, persistance) relèvent d'un exercice encadré de sensibilisation à la cybersécurité. Elles ne doivent en aucun cas être reproduites contre un système ou une personne sans consentement explicite et cadre légal (test d'intrusion contractualisé, CTF, etc.).

## 🎯 Scénario

Une reconnaissance passive est menée à partir d'une simple publication LinkedIn annonçant l'arrivée d'une nouvelle collaboratrice dans une entreprise fictive. Ce point d'entrée anodin permet de reconstituer progressivement son identité, son parcours, son réseau professionnel, sa localisation probable et son exposition aux fuites de données — avant d'exploiter ces informations pour un scénario d'ingénierie sociale menant à un accès initial, une élévation de privilèges et l'effacement des traces.

## 🔍 Phases couvertes

1. **Contexte et scénario** – présentation de l'entreprise cible et du point de départ
2. **Phase de reconnaissance (OSINT)** – identité, parcours, réseau professionnel, informations juridiques, localisation, emails, fuites de données
3. **Synthèse et niveau de fiabilité** – croisement et hiérarchisation des sources
4. **Chaîne d'attaque** – enchaînement des vecteurs exploitables
5. **Phase 3 – Gaining Access** – ingénierie sociale par message vocal (voix clonée) et macro malveillante
6. **Phase 4 – Maintaining Access & élévation de privilèges**
7. **Phase 5 – Covering Tracks** – effacement des traces d'intrusion
8. **Conclusion**

## 🛠️ Outils et sources utilisés

- **OSINT** : Sherlock, LinkedIn, Epieos, Geneanet, Google Maps
- **Fuites de données** : Have I Been Pwned (HIBP)
- **Registres d'entreprises** : RNE, INSEE, Guichet unique
- **Ingénierie sociale** : Deepfake  (clonage vocal Voicebox)
- **Exploitation / post-exploitation** : macro VBA, Kali Linux
