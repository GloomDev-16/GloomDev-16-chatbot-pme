# Chatbot PME – Assistant Professionnel Multicanal

## 🇫🇷 Présentation

**Chatbot PME** est une solution complète pour les petites et moyennes entreprises (PME) : assistant conversationnel intelligent, disponible sur Web, WhatsApp et Telegram. Il répond à vos questions métier, automatise la relation client, et facilite l’accès à l’information.

### Fonctionnalités principales
- Réponses professionnelles instantanées (GPT-4/Mistral)
- Interface graphique moderne (Tkinter)
- Intégrations WhatsApp & Telegram
- Système de clés d’accès sécurisé pour chaque client
- Tableau de bord analytique (bientôt)

### Sécurité & Accès
Chaque utilisateur doit s’inscrire via WhatsApp pour recevoir sa **clé d’accès personnelle**. Cette clé est requise pour utiliser le bot sur tous les canaux.

---

## 🚀 Installation & Lancement

### 1. Prérequis
- Python 3.8+
- Compte OpenAI (ou Mistral)
- Compte Twilio (WhatsApp)
- Bot Telegram (token)

### 2. Installation
```bash
git clone <votre-repo>
cd chatbot-pme
pip install -r requirements.txt
```

### 3. Configuration
Créez un fichier `.env` à la racine :
```
OPENAI_API_KEY=sk-...
TWILIO_SID=...
TWILIO_TOKEN=...
TELEGRAM_BOT_TOKEN=...
```

---

### 4. Lancement
- **Backend API** :  
  `uvicorn backend.api:app --host 0.0.0.0 --port 8000`
- **Interface graphique** :  
  `python frontend/main.py`
- **Bot Telegram** :  
  `python run_telegram_bot.py`

---

## 🟢 Utilisation

### Inscription (obligatoire)
1. Envoyez « INSCRIPTION » au numéro WhatsApp du bot.
2. Recevez une clé d’accès unique.
3. Utilisez cette clé dans l’interface ou l’API.

### Exemple de requête API
```json
{
  "content": "Bonjour",
  "channel": "web",
  "user_id": "demo",
  "access_key": "PME-XXXX-YYYY"
}
```

---

## 🇬🇧 English – Quick Start

**Chatbot PME** is a complete, secure, multi-channel assistant for SMEs. It answers business questions, automates customer support, and provides information instantly on Web, WhatsApp, and Telegram.

### Key Features
- Instant professional answers (GPT-4/Mistral)
- Modern GUI (Tkinter)
- WhatsApp & Telegram integrations
- Secure access key system for each client
- Analytics dashboard (coming soon)

### Security & Access
Each user must register via WhatsApp to receive a **personal access key**. This key is required for all bot usage.

---

### 1. Requirements
- Python 3.8+
- OpenAI (or Mistral) account
- Twilio account (WhatsApp)
- Telegram bot token

### 2. Installation
```bash
git clone <your-repo>
cd chatbot-pme
pip install -r requirements.txt
```

### 3. Configuration
Create a `.env` file at the project root:
```
OPENAI_API_KEY=sk-...
TWILIO_SID=...
TWILIO_TOKEN=...
TELEGRAM_BOT_TOKEN=...
```

### 4. Launch
- **Backend API**:
  `uvicorn backend.api:app --host 0.0.0.0 --port 8000`
- **GUI**:
  `python frontend/main.py`
- **Telegram bot**:
  `python run_telegram_bot.py`

---

## 🟢 Usage

### Registration (required)
1. Send "INSCRIPTION" to the WhatsApp bot number.
2. Receive your unique access key.
3. Use this key in the interface or API.

### Example API request
```json
{
  "content": "Hello",
  "channel": "web",
  "user_id": "demo",
  "access_key": "PME-XXXX-YYYY"
}
```

---

## 📞 Support
Pour toute question ou personnalisation, contactez l’éditeur du bot.

For support or customization, contact the bot provider.
