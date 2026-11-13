# StudiaInsieme

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)
[![Next.js](https://img.shields.io/badge/Next.js-14-black)](https://nextjs.org/)
[![TypeScript](https://img.shields.io/badge/TypeScript-5-blue)](https://www.typescriptlang.org/)
[![Supabase](https://img.shields.io/badge/Supabase-PostgreSQL-green)](https://supabase.com/)

Social network verticale per la condivisione di appunti tra studenti delle scuole superiori e dell'università.

**Tag line:** Segui chi sa, condividi ciò che impari.

---

## Indice

- [Panoramica](#panoramica)
- [Funzionalità](#funzionalità)
- [Stack](#stack)
- [Installazione](#installazione)
- [Struttura del progetto](#struttura-del-progetto)
- [Roadmap](#roadmap)
- [Contribuire](#contribuire)
- [Licenza](#licenza)

---

## Panoramica

Gli appunti circolano oggi in modo frammentato: PDF su gruppi WhatsApp, foto in chat, file non organizzati. StudiaInsieme centralizza la condivisione in un'esperienza sociale: feed personalizzato per materia e istituto, profili con follower, like, salvataggi e un sistema di reputazione che fa emergere i contributori migliori.

Il progetto nasce con un approccio pilot: lancio iniziale su un singolo istituto per validare il modello prima di scalare.

---

## Funzionalità

**Account**
- Registrazione e login con email o Google
- Profilo con foto, bio, istituto, classe/anno, materie preferite
- Statistiche personali e badge
- Impostazioni privacy

**Feed e scoperta**
- Feed personalizzato per materie e studenti seguiti
- Ricerca per materia, istituto, autore, parola chiave
- Feed stile TikTok (v2)

**Appunti**
- Upload di PDF, foto e testo con metadati (materia, istituto, classe, tag)
- Anteprima in bozza prima della pubblicazione
- Gestione dei propri appunti (modifica, eliminazione)
- Cartelle personalizzate per gli appunti salvati

**Interazione social**
- Like, follow, commenti
- Salvataggio in cartelle
- Notifiche
- Messaggi diretti (v2)

**Moderazione**
- Pannello admin (rimozione contenuti, ban)
- Segnalazione copyright
- Gestione dati GDPR

---

## Stack

| Livello | Tecnologia |
|---------|-----------|
| Frontend | Next.js 14 (App Router), React, Tailwind CSS |
| Backend / DB | Supabase (PostgreSQL, Auth, Storage) |
| Ricerca | Meilisearch |
| Hosting | Vercel + Supabase |
| Linguaggio | TypeScript |

---

## Installazione

**Prerequisiti:** Node.js 18+, npm, account Supabase.

```bash
git clone https://github.com/tuo-username/studioinsieme.git
cd studioinsieme
npm install
cp .env.example .env.local
