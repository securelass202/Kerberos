# 🌐 TCP vs UDP - Comparaison des Protocoles de Transport

## 🔍 Introduction

TCP (Transmission Control Protocol) et UDP (User Datagram Protocol) sont deux **protocoles de couche transport** utilisés pour transmettre des données sur Internet. Bien qu’ils partagent certains buts, ils sont **radicalement différents en termes de fonctionnement, fiabilité et cas d’usage**.

---

## 🧠 Principales Différences

| 🧩 Critère                | 🧷 TCP                                         | 🧷 UDP                                |
|--------------------------|-----------------------------------------------|--------------------------------------|
| **Connexion**            | Orienté connexion (négo. via handshake)       | Sans connexion                       |
| **Fiabilité**            | Assure la livraison (ACK, retransmission)     | Pas de garantie de livraison         |
| **Ordre des données**    | Garanti                                       | Non garanti                          |
| **Contrôle de flux**     | Oui                                           | Non                                  |
| **Taille de l’en-tête**  | 20 octets (plus lourd)                        | 8 octets (léger)                     |
| **Vitesse**              | Moins rapide (plus de contrôle)               | Très rapide                          |
| **Transmission**         | Flux continu (stream)                         | Datagrams indépendants               |

---

## 💼 Cas d’utilisation

### ✅ TCP est utilisé pour :
- HTTP / HTTPS (web)
- SSH (connexion sécurisée)
- FTP (transfert de fichiers)
- SMTP (envoi d’e-mails)

### ✅ UDP est utilisé pour :
- DNS (résolution de noms)
- DHCP (attribution d’adresse IP)
- VoIP (voix sur IP)
- Streaming (audio / vidéo)
- Jeux en ligne (latence faible)

---

## 🧪 Exemple illustratif

- **TCP** : comme une conversation téléphonique — on s’assure que l’autre a bien entendu avant de continuer.
- **UDP** : comme envoyer des SMS — pas de confirmation, pas de garantie que l’autre les lit dans l’ordre.

---

## 🔐 Résumé Sécurité

| Protocole | Avantage Sécurité | Inconvénient Sécurité        |
|-----------|-------------------|------------------------------|
| TCP       | Meilleure gestion des erreurs | Plus de surface d’attaque (ex : SYN Flood) |
| UDP       | Moins de contrôle = moins d’attaques ciblées sur le protocole | Spoofing facile, pas de vérification |

---

## 🧾 Conclusion

- **TCP** = Fiabilité, ordre, lenteur → Pour données sensibles ou structurées
- **UDP** = Rapidité, légèreté, incertitude → Pour temps réel ou volume élevé

> 🎯 Choisissez **TCP** pour la précision. Choisissez **UDP** pour la rapidité.


![Image](https://github.com/user-attachments/assets/d0956443-91b4-4253-948c-64df8fb0a47e)
