# 🛠️ Suite d'Outils d'Exploitation & Automatisation OT/IT

Bienvenue sur l'espace regroupant les applications et utilitaires d'administration, de sauvegarde, de supervision et de sécurité dédiés aux environnements industriels (**OT / Télégestion / Supervision**).

> 🔒 *Les dépôts de code sont privés ; les liens ci-dessous sont accessibles aux comptes autorisés.*

---

## 📦 Catalogue des projets

**10 projets** regroupés par domaine d’exploitation.

### 📲 Portail d'Alarmes & Télégestion

| Projet | Version | Socle technique | Rôle principal |
| :--- | :---: | :--- | :--- |
| [**KiTools**](https://github.com/A2ICoder/KiTools) | `v0.16.1` | `.NET 10` · `ASP.NET Core` · `SQLite` | Portail web temps réel de réception, qualification et acquittement des alarmes SMS de télégestion, avec supervision du modem et fonctionnement hors ligne. |

### 📡 Écosystème S4-Manager / Stations S4 & S4W

| Projet | Version | Socle technique | Rôle principal |
| :--- | :---: | :--- | :--- |
| [**S4-Keeper**](https://github.com/A2ICoder/S4-Keeper) | `v1.0.0` | `PowerShell 7` · `SHA-256` · `SMTP` | Sauvegarde automatisée des configurations S4-Manager, publication vérifiée, rétention multi-paliers et rapport hebdomadaire HTML/CSV. |
| [**S4W-CertScope**](https://github.com/A2ICoder/S4W-CertScope) | `v1.0.0` | `PowerShell 5.1+` · `TLS/X.509` | Audit parallèle planifié des certificats HTTPS du parc S4W et alerte automatique sur les autorités non conformes. |
| [**S4-FleetOps**](https://github.com/A2ICoder/S4-FleetOps) | `v1.0.0` | `PowerShell 7 / 5.1` · `CSV` | Outil à la demande : export des utilisateurs, export du diagnostic des stations et rafraîchissement groupé contrôlé. |

### 🌐 Continuité de Service WebServ / Topkapi

| Projet | Version | Socle technique | Rôle principal |
| :--- | :---: | :--- | :--- |
| [**WebServ-Sentinel**](https://github.com/A2ICoder/WebServ-Sentinel) | `v1.0.0` | `PowerShell 5.1` · `IIS` | Surveillance applicative multi-sites (équipement + portail HTTPS) et recyclage contrôlé des pools IIS après panne confirmée. |
| [**WebServ-Rebound**](https://github.com/A2ICoder/WebServ-Rebound) | `v1.0.0` | `PowerShell 5.1` · `Services Windows` | Surveillance locale WebServ / Topkapi et redémarrage gradué des services Windows avec escalade bornée et quotas glissants. |

### 💾 Sauvegarde Patrimoine OT & Équipements Réseau

| Projet | Version | Socle technique | Rôle principal |
| :--- | :---: | :--- | :--- |
| [**A2I Vault**](https://github.com/A2ICoder/A2IVault) | `v0.4.33` | `.NET 10` · `ASP.NET Core` · `SQLite` · `agents Windows` | Plateforme centrale de sauvegarde et de supervision du patrimoine industriel, avec console web, agents Windows, contrôles SHA-256 et rétention. |
| [**ARA-Vault**](https://github.com/A2ICoder/ARA-Vault) | `v1.0.0` | `PowerShell 5.1 / 7` · `RoboCopy` · `7-Zip` | Sauvegarde automatisée, contrôle d'intégrité `SHA-256`, purge encadrée et rapport hebdomadaire du patrimoine industriel (API, supervisions, partages OT). |
| [**PLC Backup Station**](https://github.com/A2ICoder/PLC-Backup-Station) | `v0.1.0` · expérimental | `C#` · `.NET Framework 4.8` · `Modbus/TCP / UMAS` | CLI autonome de sauvegarde APPLICATION/DATA d’automates Schneider avec mot de passe applicatif connu. Validé sur simulateur ; qualification matérielle restante. |
| [**NPort-RebootGuard**](https://github.com/A2ICoder/NPort-RebootGuard) | `v1.0.0` | `PowerShell 5.1` · `HTTP / CDP` | Enchaînement séquentiel `Save/Restart` des serveurs série Moxa NPort et validation automatique du retour en service. |

---

## 🧭 Conventions communes à tous les dépôts

- **Zéro donnée sensible dans Git** : adresses IP, URL internes, partages NAS et destinataires résident exclusivement dans des fichiers de configuration locaux non versionnés (`*.local.psd1`, `*.Site.psd1`, `config.json`), accompagnés d'un modèle `*.example.*` versionné.
- **Identité visuelle normalisée** : logos, bannières et icônes rangés dans `assets/brand/`, avec leur documentation de marque associée.
- **Hygiène multi-outils** : `.gitattributes` adapté à chaque projet et mémoire technique locale `AGENTS.md` hors dépôt.
