# Portfolio Professionale | Architettura SASS e Sviluppo Front-End

Questo repository contiene il codice sorgente del portfolio di Pasquale Lucarelli. Il progetto è concepito come un esercizio di rigore tecnico, mirando a bilanciare un'estetica di **low cognitive load** con una fondazione di codice estremamente modulare e scalabile.

La documentazione e l'architettura interna sono state curate per facilitare l'analisi del codice, la manutenibilità a lungo termine e l'eventuale contribuzione in un contesto di lavoro in team.

---

## 🏗️ Filosofia e Struttura Architetturale

La struttura del progetto riflette l'adesione ai principi di **Separazione delle Preoccupazioni (SoC)** e l'uso di SASS come strumento primario di *Design System* management.

### Punti Chiave dell'Architettura

*   **SASS-Centric Design System:** L'intera gestione degli stili si basa su un'architettura SCSS modulare. Variabili globali (*design tokens*), *mixins* e *functions* sono centralizzati, garantendo un controllo capillare sul tema e una rapida iterazione stilistica.
*   **Gestione di Bootstrap 5:** Il framework Bootstrap 5 è stato integrato e **destrutturato** tramite SASS. Questo approccio ha permesso di eliminare il *bloat* e utilizzare solo le utility necessarie, ottimizzando il peso finale del CSS.
*   **Layout Asimmetrico (CSS Grid):** Il layout è costruito prevalentemente utilizzando **CSS Grid**, una scelta che massimizza l'efficienza nella gestione di strutture complesse e supporta il design asimmetrico voluto.

## 🛠️ Stack Tecnologico

| Tecnologia | Descrizione di Ruolo |
| **HTML5** | Fondazione semantica e strutturale del contenuto. |
| **SCSS / SASS** | Architettura, variabili tematiche e compilazione modulare degli stili. |
| **Bootstrap 5** | Framework di base, utilizzato solo nella sua forma essenziale (destrutturata). |
| **JavaScript** | Utilizzo mirato per micro-interazioni e miglioramenti UX non invasivi. |

## ⚙️ Guida all'Esecuzione Locale

Per configurare e visualizzare il progetto in locale, è necessario che l'ambiente supporti la compilazione SASS (tramite Node.js).

1. **Clonazione del Repository:**
    ```bash
    git clone []
    cd portfolio
    ```

2. **Avvio del Watcher SASS:**
    Il CSS è generato dinamicamente. Questo comando è fondamentale per monitorare le modifiche ai file SCSS e compilarli automaticamente nell'output CSS.

    ```bash
    sass --watch assets/scss:assets/css
    ```
    *Si raccomanda di mantenere attivo il watcher SASS durante lo sviluppo.*

3. **Visualizzazione Locale:**
    Aprire il file `index.html` direttamente nel browser o tramite un server di sviluppo locale (es. Live Server) per visualizzare il risultato.

## 📂 Struttura per la Manutenzione e Contribuzione

La seguente struttura è stata ottimizzata per una navigazione intuitiva da parte di contributori esterni:

*   **File HTML Principali:** `index.html`, `curriculum.html`, `projects.html`
*   **Assets SCSS (Architettura Stili):** `/assets/scss/`
    *   `_variables.scss`: File centrale per tutti i *design tokens* (colori, font, breakpoint).
    *   `_mixins.scss`: Collezione di utility SASS custom per la generazione di stili dinamici.

## 🔗 Distribuzione Online

Il progetto è attualmente ospitato su piattaforma GitHub Pages, garantendo un *deployment* rapido e una accessibilità immediata.
**Accesso al Portfolio Live:**
[https://palale858-create.github.io/portfolio/](https://palale858-create.github.io/portfolio/)
