# MediConnect — Sécurisation de l'infrastructure réseau

Projet du module **Sécurité des réseaux** — Efrei Paris (Cybersécurité et Cloud), octobre 2026.

Conception, mise en œuvre et test de l'infrastructure réseau d'une plateforme
de prise de rendez-vous médicaux, sur une maquette VirtualBox avec deux
pare-feux **Stormshield SNS 4.8.14**.

## Points clés
- 2 sites, 6 zones de sécurité au siège (ADMIN, SRV, LAN, DMZ-PROD, DMZ-DEMO, OUT)
- VPN IPsec IKEv2 site à site (AES-256, PFS) et VPN SSL OpenVPN pour les nomades
- Annuaire LDAP, 7 groupes, règles de filtrage basées sur l'identité
- MFA TOTP pour les médecins via portail captif
- IPS, filtrage d'URL, blocage par service web, protection anti-DoS
- Administration via zone dédiée et bastion SSH
- Journalisation nominative et 44 tests positifs/négatifs documentés

## Rapport
📄 [Lire le rapport complet (PDF)](Rapport_MediConnect_BOUDACHE.pdf)

## Auteur
Zakari BOUDACHE
