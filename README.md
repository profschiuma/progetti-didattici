# DoodlePop 🍿

> **AI Motion & Audio Puppeteer Studio**
> Anima i disegni e le illustrazioni dei bambini in tempo reale attraverso l'intelligenza artificiale, il tracciamento corporeo e la voce.

---

## 📖 Descrizione

**DoodlePop** è un'applicazione web interattiva progettata per la didattica digitale, l'animazione e la narrazione visiva nella scuola dell'infanzia e primaria.

L'app trasforma qualsiasi disegno statico realizzato su carta in una marionetta digitale animata (avatar 2D):

1. **Motion Capture via Webcam:** Attraverso modelli di Computer Vision (*MediaPipe Pose*), il corpo dell'alunno controlla in tempo reale braccia, gambe, tronco e inclinazione della testa del personaggio.
2. **Animazione Vocale:** Il microfono rileva il parlato o il canto, animando dinamicamente la bocca del burattino in sincronia con la voce.
3. **Regia e Spostamento Scenico:** L'utente può muovere il personaggio nello spazio dello sfondo tramite tocco (iPad/Tablet), mouse o frecce della tastiera.
4. **Registrazione Video:** Permette di registrare l'intera recitazione ed esportare il filmato in formato video `.mp4` o `.webm`.

L'applicazione è **100% standalone** (un singolo file HTML senza dipendenze server o cartelle esterne) ed è eseguibile direttamente via browser su PC, Mac, iPad e Chromebook.

---

## ✨ Caratteristiche Principali

* **🪄 Scontorno Automatico del Foglio:** Algoritmo integrato di rimozione del fondo bianco cartaceo con slider di tolleranza regolabile.
* **🦴 Setup Scheletro (Rigging a Doppia Modalità):**
* *Modalità Stickman:* Allineamento rapido dei nodi articolari direttamente sul disegno, con aggancio automatico testa-collo senza fessure (*Zero Gap*).
* *Modalità Lazo:* Ritaglio a mano libera dei singoli arti per personaggi asimmetrici o disegni non convenzionali.


* **🪞 Modalità Specchio Bambini (1:1):** Rispecchiamento intuitivo dei movimenti (muovendo il braccio destro risponde il braccio sul lato destro dello schermo).
* **🎯 Stabilizzatore di Movimento (Anti-Jitter):** Filtro esponenziale (EMA) per eliminare i tremolii della webcam e garantire movimenti corporei fluidi.
* **🕹️ Interazione Spaziale:** Possibilità di trascinare il personaggio sullo sfondo con il dito (iPad) o le frecce della tastiera mentre recita.
* **🎙️ Bocca Dinamica Vettoriale:** Apertura e articolazione labiale reattiva al volume della voce.
* **📹 Registrazione Nativa MP4/WebM:** Acquisizione sincrona di video, audio e movimenti con blocco di sicurezza anti-interruzione.
* **🌍 Interfaccia Multilingua:** Supporto completo in 5 lingue (Italiano, Inglese, Spagnolo, Francese, Tedesco).

---

## 🚀 Guida all'Uso

### 1. Preparazione del Personaggio (Consigli per il disegno)

* **Posa a Stella (T-Pose):** Disegnare il personaggio con braccia e gambe ben aperte e staccate dal tronco.
* **Collo Visibile:** Lasciare un po' di spazio tra la testa e la maglia per facilitare il punto di rotazione.
* **Foglio Bianco:** Disegnare su carta bianca ben illuminata, evitando ombre scure o elementi di sfondo.

### 2. Caricamento e Rigging

1. Cliccare su **`🖼️ Sfondo`** per caricare l'ambientazione scenica (bosco, spazio, castello, ecc.).
2. Cliccare su **`🧍 Personaggio`** per caricare la foto del disegno del bambino.
3. Regolare la **Tolleranza Scontorno Foglio** per rendere trasparente la carta bianca.
4. Nella vista **Stickman**, trascinare i nodi colorati sulle articolazioni del disegno (spalle, gomiti, polsi, bacino, ginocchia e caviglie).
5. Posizionare il nodo **Collo** esattamente alla base della testa/colletto.

### 3. Animazione e Registrazione

1. Cliccare su **`▶️ Avvia Tracking Webcam`** e posizionarsi davanti alla telecamera.
2. Attivare il **`🎙️ Microfono`** per abilitare l'animazione della bocca.
3. **Muoversi e Recitare:** Spostare il personaggio sullo sfondo trascinandolo con il dito (iPad) o usando le frecce della tastiera da PC.
4. Cliccare su **`⏺️ Registra Video MP4`** per avviare la registrazione dello spettacolo.
5. Cliccare su **`⏹️ Ferma & Salva Video`** per scaricare automaticamente il file video finito.

---

## 🛠️ Tecnologie Utilizzate

* **HTML5 Canvas & JavaScript ES6+** (Rendering a 30 FPS client-side)
* **Google MediaPipe Pose** (Modello di stima scheletrica e pose detection)
* **Web Audio API** (Analisi spettrale e modulazione labiale)
* **MediaRecorder API** (Cattura video Canvas + Audio Stream combinato)

---

## ⚖️ Licenza e Attribuzioni

**DoodlePop** è un software educativo ideato e sviluppato da **Giuseppe Schiuma** (2026).

Distribuito sotto licenza **MIT License**.

### Librerie Open Source di Terze Parti

* **Google MediaPipe Pose** – Copyright (c) The MediaPipe Authors.
Distribuito sotto licenza [Apache License 2.0](http://www.apache.org/licenses/LICENSE-2.0).
