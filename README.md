# WordPress Perfect .htaccess

🛡️ **The ultimate, production-ready GNU GPLv3 `.htaccess` configuration optimized for WordPress speed, security, and performance (Updated 2026).**

---

## English 🇬🇧

`WordPress Perfect .htaccess` is a highly optimized, bulletproof configuration file designed specifically for WordPress websites running on Apache 2.4+ servers. 

Following a strict 2026 security audit, this version goes beyond basic rules to offer modern web optimizations (HTTP/2 & HTTP/3 readiness) and an advanced security layout aimed at achieving an **A+ score** on tools like *securityheaders.com*.

### ✨ Features & 2026 Audit Fixes
* **Security Headers (A+ Grade):** Implements a robust Content Security Policy (CSP) pre-configured for WordPress core, Gutenberg, and major tools (Google Analytics, Stripe, PayPal, YouTube). Includes modern COOP, COEP, and CORP headers.
* **WooCommerce Native Support:** Dynamically blocks transactional pages (`/cart`, `/checkout`, `/my-account`) from being cached to prevent private data leaks.
* **Performance Optimization:** Highly tuned Gzip/Deflate compression (including text-based SVG) and far-future expires headers with `immutable` caching parameters.
* **8G Firewall Integrated:** Embedded with the reliable 8G Firewall matrix to filter malicious query strings, request URIs, and bad user-agents.
* **WordPress & Gutenberg Friendly:** Restores compatibility with the block editor by safely delegating User REST API endpoints to PHP rather than blindly blocking them via Apache.

### 🚀 Quick Start
1.  **Backup:** Always back up your existing `.htaccess` file before replacing it.
2.  **Copy & Paste:** Copy the contents of the `.htaccess` file from this repository into your WordPress root directory.
3.  **Tailor:** Look at the `Content-Security-Policy` block. If you use page builders like Elementor or Divi, leave `'unsafe-eval'` active; otherwise, you can remove it for extra tightening.

### 📄 License
This project is licensed under the **GNU GPLv3 License** - see the comment block inside the file or the [LICENSE](LICENSE) file for details.

---

## Français 🇫🇷

`WordPress Perfect .htaccess` est un fichier de configuration hautement optimisé et sécurisé, conçu spécifiquement pour les sites WordPress propulsés par un serveur Apache 2.4+.

Suite à un audit de sécurité rigoureux en 2026, cette version dépasse les simples règles de réécriture pour offrir des optimisations adaptées au web moderne (HTTP/2 & HTTP/3) et une architecture de sécurité conçue pour cibler la **note maximale A+** sur des outils comme *securityheaders.com*.

### ✨ Fonctionnalités & Corrections de l'Audit 2026
* **En-têtes de sécurité (Score A+) :** Implémentation d'une Content Security Policy (CSP) robuste, pré-configurée pour le cœur de WP, Gutenberg, et les scripts tiers courants (Analytics, Stripe, PayPal, YouTube). Intègre les en-têtes modernes COOP, COEP et CORP.
* **Compatibilité native WooCommerce :** Blocage dynamique de la mise en cache des pages transactionnelles (`/cart`, `/checkout`, etc.) pour éviter toute fuite de données privées entre clients.
* **Performances maximales :** Compression Gzip/Deflate optimisée (incluant les fichiers SVG textuels) et gestion agressive du cache du navigateur avec la directive `immutable`.
* **Pare-feu 8G intégré :** Intégration transparente de la matrice 8G Firewall pour intercepter les requêtes injectées, les mauvais User-Agents et les scripts malveillants.
* **Gutenberg & API REST :** Correction des règles d'analyse d'auteurs pour ne plus bloquer l'éditeur de blocs natif de WordPress, tout en protégeant le site contre l'énumération brute.

### 🚀 Démarrage rapide
1.  **Sauvegarde :** Sauvegardez impérativement votre fichier `.htaccess` actuel avant toute modification.
2.  **Copier/Coller :** Copiez le contenu du fichier `.htaccess` de ce dépôt et collez-le à la racine
