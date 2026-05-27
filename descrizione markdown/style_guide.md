# Overline — Brand & Website Style Guide

Questo documento analizza in dettaglio le scelte stilistiche, l'architettura visiva e le interazioni del sito web **Overline**, delineandone l'identità visiva e tecnica.

## 1. Identità e "Vibe"
Il sito trasmette una sensazione di estrema **robustezza, precisione industriale e qualità premium**. Il design è brutale ma raffinato, perfettamente in linea con il prodotto: attrezzatura professionale e massiccia per il braccio di ferro.
*   **Parole Chiave:** Industriale, Brutalista, Tecnico, Premium, Inarrestabile, Preciso.
*   **Filosofia:** "Niente Superfluo" - Il design elimina le distrazioni per concentrarsi sulla solidità dei materiali e della meccanica.

## 2. Palette Cromatica (Dark Theme)
L'interfaccia si basa su un tema scuro profondo (Dark Mode nativo) con un singolo colore d'accento molto forte, che richiama l'aggressività e l'energia agonistica.

| Ruolo | Colore (HEX) | Descrizione |
| :--- | :--- | :--- |
| **Background Base** | `#030303` | Un nero quasi assoluto, crea profondità e contrasto infinito. |
| **Superfici / Card** | `#0d0d0d` | Grigio scurissimo utilizzato per elevare leggermente i contenitori dal fondo. |
| **Testo Principale** | `#F0F0F0` | Bianco sporco per garantire un'alta leggibilità senza affaticare la vista. |
| **Testo Secondario** | `#888888` | Grigio medio per descrizioni, note e testi di supporto (Muted). |
| **Accento** | `#E60000` | Un rosso intenso e vibrante. Usato per dettagli chiave, linee di demarcazione, bottoni e indicatori di progresso. |
| **Bordi / Outline** | `#2A2A2A` | Grigio scuro per delineare delicatamente le sezioni e i contenitori. |

## 3. Tipografia
Il sistema tipografico gioca su forti contrasti, mescolando l'impatto visivo di font display con la precisione tecnica dei font monospazio.

*   **Display Font (`Anton`)**: 
    *   *Uso:* Titoli giganti (`<h1>`, `<h2>`), claim principali.
    *   *Stile:* Tutto maiuscolo, condensato, massiccio. Comunica forza bruta e imponenza (es. "NIENTE SUPERFLUO").
*   **Mono Font (`JetBrains Mono`)**: 
    *   *Uso:* Etichette, specifiche tecniche, numerazioni di sezione, piccoli sottotitoli.
    *   *Stile:* Tecnico, preciso, ingegneristico. Aumenta la percezione di un prodotto "calibrato" e meccanico. Spesso usato con un ampio `letter-spacing` (0.1em - 0.2em) e in maiuscolo.
*   **Body Font (`Hanken Grotesk`)**: 
    *   *Uso:* Paragrafi descrittivi, testi lunghi.
    *   *Stile:* Sans-serif moderno, pulito e altamente leggibile.

## 4. Elementi Visivi e Layout
Il layout respira grazie a un ampio utilizzo di spazio negativo (margin-h: 64px, section-gap: 160px), conferendo un'aura di lusso industriale.

*   **Glassmorphism (Effetto Vetro):** Navbar e card testuali utilizzano sfondi semi-trasparenti neri (`rgba(3,3,3,0.75)`) combinati con filtri di sfocatura (`backdrop-filter: blur(12px-20px)`). Questo permette alle immagini di sfondo di trasparire elegantemente, creando profondità.
*   **Vignettatura e Gradienti:** Le immagini di sfondo non sono mai piatte. Sono sempre trattate con gradienti radiali (vignette) o lineari scuri ai bordi per fondersi perfettamente con le transizioni tra le sezioni (fade in entrata e in uscita) e per far risaltare i testi bianchi in sovrimpressione.
*   **Linee e Geometrie Rigide:** Uso frequente di bordi netti (spesso a sinistra, colorati di rosso accento) per delimitare paragrafi o card. Questo rafforza l'estetica "squadrata" e meccanica.
*   **Dettagli Tecnici (Micro-UI):** Presenza di elementi come indicatori di progresso lineari (`#progress`), piccoli "dot" pulsanti accanto alle etichette (`.label-tag .dot`) e watermarks giganti in semitrasparenza (nel footer).

## 5. Dinamismo e Animazioni (Motion Design)
Il sito è fortemente interattivo e basato sullo scroll, utilizzando tecnologie all'avanguardia come **GSAP (ScrollTrigger)** e **Lenis (Smooth Scroll)** per un'esperienza fluida e cinematografica.

> [!TIP]
> Le animazioni non sono puramente estetiche, ma guidano l'occhio dell'utente esaltando l'impatto dei prodotti e la "pesantezza" dei materiali.

*   **Smooth Scrolling:** Movimento della pagina fluido e ammortizzato, essenziale per far percepire il sito come un'app premium.
*   **Text Reveal:** I titoli principali non compaiono semplicemente, ma emergono dal basso (mascherati) riga per riga, simulando la solidità che si "svela".
*   **Parallasse (Parallax):** Le immagini di sfondo in tutte le sezioni e nell'hero banner si muovono a velocità diversa rispetto allo scroll, creando una profonda tridimensionalità. Nell'hero è presente anche un lento effetto "Ken Burns" in loop (scale up continuo).
*   **Scroll-Jacking / Pinning (Sezione 4 e 5):** 
    *   *Titoli Pinned:* Elementi che si bloccano al centro dello schermo mentre scalano di dimensione allo scroll.
    *   *Pannelli Sequenziali:* La sezione "Precisione" blocca lo schermo diviso a metà, cambiando le descrizioni di testo sulla destra (S5 Dual Panel) in base alla percentuale di scroll dell'utente, accompagnato da una barra di progresso verticale.
*   **Ease Pesanti:** Le transizioni utilizzano curve di easing specifiche (come `expo.out` o `power4.out`), che danno un senso di inerzia e peso agli elementi che entrano nello schermo.
