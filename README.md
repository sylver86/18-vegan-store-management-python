# VeganShop — Gestionale CLI per Negozio Vegano in Python

![Python](https://img.shields.io/badge/Python-3.8+-3776AB?logo=python&logoColor=white)
![OOP](https://img.shields.io/badge/Design-OOP-blue)
![JSON](https://img.shields.io/badge/Persistence-JSON-lightgrey)
![CLI](https://img.shields.io/badge/Interface-CLI-green)

## Panoramica

Applicazione CLI per la gestione di un negozio di prodotti vegani: catalogo prodotti, registrazione vendite, controllo scorte e calcolo margini (lordo e netto). Progettata con focus su organizzazione del codice, persistenza dei dati e validazione robusta dell'input — dimostrando solidi principi Python in un contesto CRUD reale.

Dimostra competenze applicabili allo sviluppo di tool interni enterprise, script di gestione e qualsiasi applicativo Python che richieda persistenza, validazione e logica di business.

## Valore Enterprise

| Settore / Azienda | Rilevanza |
|-------------------|-----------|
| Engineering Informatica | OOP Python, persistenza JSON, logica gestionale |
| IT Consulting (NTT Data, Accenture) | Python scripting per tool interni enterprise |
| Retail & E-commerce | Pattern CRUD applicabile a sistemi di inventario |
| Qualsiasi settore | Architettura CLI riutilizzabile per script di gestione |

## Funzionalità

| Feature | Descrizione |
|---------|-------------|
| Registrazione prodotto | Nome, quantità, prezzo acquisto, prezzo vendita |
| Listino prodotti | Vista completa catalogo con livelli di stock correnti |
| Registrazione vendita | Log transazione, aggiornamento automatico stock |
| Validazione stock | Alert se quantità richiesta supera disponibilità |
| Rifornimento stock | Aggiunta quantità a prodotto esistente senza reinserire prezzi |
| Profitto lordo | Calcolo ricavo totale vendite |
| Profitto netto | Ricavo meno costo acquisto della merce venduta |
| Persistenza dati | Stato salvato in `db.json` tra sessioni |
| Validazione input | Check numerici con recovery errore su tutti gli input |

## Utilizzo

```bash
git clone https://github.com/sylver86/18-vegan-store-management-python.git
cd 18-vegan-store-management-python
python main.py
```

**Menu interattivo:**
```
=== VEGAN STORE MANAGEMENT ===
1. Aggiungi prodotto
2. Lista prodotti
3. Registra vendita
4. Profitto lordo
5. Profitto netto
0. Esci
```

## Struttura Repository

```
18-vegan-store-management-python/
├── main.py        # Entry point — menu CLI e loop principale
├── README.md
```

**Design highlights:**
- Funzioni con responsabilità singola (gestione prodotti, vendite, reporting)
- Struttura dati in-memory: dizionari + liste per il catalogo
- Serializzazione JSON per persistenza cross-sessione
- Try/except su tutti gli input numerici con messaggi di errore user-friendly

## Stack Tecnologico

`Python 3.8+` · `JSON` · `OOP` · `CLI`

---

---

# VeganShop — Python CLI Store Management Application 🇬🇧

![Python](https://img.shields.io/badge/Python-3.8+-3776AB?logo=python&logoColor=white)
![JSON](https://img.shields.io/badge/Persistence-JSON-lightgrey)

## Overview

CLI application for managing a vegan product store: product catalogue, sales recording, stock control, and profit reporting (gross and net). Designed with clean code organisation, data persistence, and robust input validation — demonstrating solid Python fundamentals in a real-world CRUD context.

## Features

| Feature | Description |
|---------|-------------|
| Product registration | Name, quantity, purchase price, sell price |
| Product listing | Full catalogue with current stock levels |
| Sales recording | Log transactions, auto-update stock |
| Stock validation | Alert if quantity requested exceeds available stock |
| Stock replenishment | Add stock without re-entering prices |
| Gross profit | Total sales revenue calculation |
| Net profit | Revenue minus purchase cost of sold goods |
| Data persistence | State saved to `db.json` between sessions |
| Input validation | Numeric checks with error recovery on all inputs |

## Usage

```bash
git clone https://github.com/sylver86/18-vegan-store-management-python.git
cd 18-vegan-store-management-python
python main.py
```

## Design Highlights

- Single-responsibility functions (product management, sales, reporting)
- In-memory catalogue with dict + list data structures
- JSON serialisation for cross-session persistence
- Try/except on all numeric inputs with user-friendly error messages

## Technologies

`Python 3.8+` · `JSON` · `OOP` · `CLI`
