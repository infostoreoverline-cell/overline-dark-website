# Overline — Brand & Website Style Guide (Comprehensive)

Questo documento rappresenta la **Bibbia di stile** per il brand e il sito web **Overline**. Definisce in maniera rigorosa e completa l'identità visiva, l'architettura dei componenti, le scelte tipografiche e le linee guida di interazione (motion design) per garantire un'esperienza utente coerente, premium e d'impatto.

---

## 1. Identità e Anima del Brand (The "Vibe")

Overline non è solo attrezzatura, è una dichiarazione di intenti. Il sito deve trasmettere immediatamente una sensazione di **estrema robustezza, precisione industriale e qualità premium ineguagliabile**. Il design è brutale, scuro e spietato, ma ingegneristicamente raffinato. È l'incarnazione digitale dell'acciaio lavorato dal pieno.

*   **L'Anima di Overline:** Nata per il braccio di ferro ai massimi livelli (Armwrestling). È per chi non accetta compromessi, per chi cerca il limite e ha bisogno di attrezzatura che non ceda mai prima di lui. L'atmosfera generale deve ricordare un'officina meccanica d'élite: sudore, magnesite, precisione assoluta e determinazione.
*   **Target Audience:** Atleti professionisti di Armwrestling, proprietari di palestre hardcore (powerlifting, strongman, armwrestling) e appassionati che pretendono il non plus ultra dell'attrezzatura.
*   **Tone of Voice (Copywriting):** Autorevole, diretto, tecnico e privo di fronzoli ("Zero Bullshit"). Le frasi devono essere brevi, incisive e trasmettere potenza. Si usano termini ingegneristici e legati alla performance pura (es. "Tolleranza zero", "Acciaio dal pieno", "Niente superfluo").
*   **Parole Chiave Visive ed Emotive:** Industriale, Brutalista, Tecnico, Premium, Inarrestabile, Preciso, Pesante, Aggressivo ma Calibrato.
*   **Filosofia "Niente Superfluo":** Il design elimina ogni distrazione per concentrarsi sull'essenziale: la solidità dei materiali e la perfezione della meccanica. Solo funzione che diventa estetica dominante.

---

## 2. Struttura Narrativa e User Journey (Scroll Storytelling)

L'intera architettura del sito Overline **non è concepita come un semplice catalogo**, ma come un vero e proprio **viaggio narrativo (Storytelling Journey)** guidato dallo scroll dell'utente.

*   **Lo Scroll come Motore Narrativo:** Lo scroll non serve solo a navigare, ma a svelare la storia. Il sito alterna momenti di ampio respiro (tanto spazio negativo, claim giganti) a momenti di densità tecnica.
*   **L'Hook (Hero Section):** Il primo impatto non deve spiegare ogni dettaglio, ma creare un senso di soggezione e potenza. È un manifesto visivo brutale che stabilisce subito il livello (premium/hardcore) del brand.
*   **Esplorazione e Smontaggio Visivo:** Le informazioni non vengono presentate tutte insieme. Man mano che l'utente scende nella pagina, il prodotto viene "vivisezionato". Le sezioni guidano l'occhio dalla visione d'insieme ai dettagli macro (es. la zigrinatura, i cuscinetti), simulando lo smontaggio ingegneristico di una macchina perfetta.
*   **Scroll-Jacking Strategico:** Invece di far scorrere via l'utente, il sito blocca la visuale (Pinning) in punti focali della narrazione. Questo forza l'utente a fermarsi, assorbire l'importanza di una feature o l'atmosfera di un video in background, prima di permettergli di proseguire.
*   **Il Climax (Risoluzione):** La narrazione costruisce tensione e desiderio e culmina sempre con una "Call to Action" inequivocabile. Solo dopo aver dimostrato la superiorità ingegneristica totale, l'utente viene invitato all'acquisto o al contatto.

---

## 3. Sistema Cromatico (Dark Theme System)

L'interfaccia si basa su un tema scuro profondo con un singolo colore d'accento molto forte. Non esistono "Light Mode", poiché la luce abbacinante non si sposa con l'atmosfera "hardcore" del brand.

| Ruolo | Colore (HEX) | Utilizzo Specifico e Regole |
| :--- | :--- | :--- |
| **Background Base** | `#030303` | Sfondo principale del tag `<body>`. Un nero quasi assoluto, crea profondità e contrasto infinito per le fotografie. |
| **Superfici / Card** | `#0D0D0D` | Sfondo per le card, i form, i modali e i menu a tendina. Serve a creare gerarchia elevando leggermente i contenitori. |
| **Testo Principale** | `#F0F0F0` | Titoli e testo dei paragrafi. Non è un bianco puro (`#FFFFFF`) per evitare l'abbagliamento e ridurre l'affaticamento visivo. |
| **Testo Secondario** | `#888888` | Testi di supporto, didascalie, placeholder dei form e icone disattivate. |
| **Brand Accent (Rosso)** | `#E60000` | Pulsanti primari (Call to Action), hover states, linee di delimitazione tecniche, indicatori di progresso e alert di errore. |
| **Accent Hover** | `#FF1A1A` | Variante più chiara del rosso per gli stati `:hover` e `:active` dei pulsanti interattivi. |
| **Bordi / Outline** | `#2A2A2A` | Linee di divisione (`<hr>`), bordi delle card e contorni degli input form. Crea struttura senza appesantire. |
| **Success State** | `#00E676` | (Opzionale) Usato solo se strettamente necessario, ad es. per i messaggi di "Acquisto Completato" o form inviati. |

### Gradienti
I gradienti sono usati con parsimonia, unicamente per scurire i bordi delle immagini e favorire la leggibilità del testo sovrastante (Vignettatura).
*   **Gradient Overlay:** `linear-gradient(to top, rgba(3,3,3,1) 0%, rgba(3,3,3,0) 50%)`

---

## 4. Tipografia (Typography System)

Il sistema tipografico gioca su forti contrasti, mescolando l'impatto visivo di font display massicci con la precisione tecnica dei font monospazio ingegneristici.

*   **Display Font (`Anton`)** 
    *   *Stile:* Tutto maiuscolo (`text-transform: uppercase`), condensato, massiccio. Comunica forza bruta.
    *   *H1 (Hero):* `8rem` (Desktop) / `4rem` (Mobile) — `line-height: 1.0`
    *   *H2 (Sezioni):* `5rem` (Desktop) / `3rem` (Mobile) — `line-height: 1.1`
*   **Mono Font (`JetBrains Mono`)**
    *   *Stile:* Tecnico, preciso, per specifiche ed etichette. Peso `400` o `700`. Maiuscolo.
    *   *Labels / Tags:* `0.85rem` — `letter-spacing: 0.15em`
    *   *Specifiche Tecniche:* `1rem` — `letter-spacing: 0.05em`
*   **Body Font (`Hanken Grotesk`)**
    *   *Stile:* Sans-serif moderno e pulito per la massima leggibilità.
    *   *Paragrafi (P):* `1.125rem` (18px) — `line-height: 1.6` — `font-weight: 400`
    *   *Testi Piccoli:* `0.875rem` (14px) — `line-height: 1.5`

---

## 5. UI Components e Architettura Visiva

Ogni componente dell'interfaccia deve sembrare "costruito" e solido come l'attrezzatura stessa. Niente angoli arrotondati morbidi (no border-radius eccessivi).

### Pulsanti (Buttons)
I pulsanti devono essere grandi, facilmente cliccabili e con interazioni fisiche (micro-animazioni di scale).
*   **Primary Button:** Background `#E60000`, Testo `#F0F0F0` (JetBrains Mono, Uppercase). Nessun bordo. Al passaggio del mouse (`:hover`) scala a `1.05` e il colore passa a `#FF1A1A`.
*   **Secondary/Outline Button:** Sfondo trasparente, Bordo `2px solid #2A2A2A`. Testo `#F0F0F0`. Al `:hover` il bordo diventa `#E60000`.
*   **Border Radius:** Rigorosamente `0px` (squadrati) o massimo `2px` per togliere l'eccessiva spigolosità dei pixel.

### Form e Input
L'estetica dei form di login, registrazione e contatto richiama interfacce terminale / cruscotti meccanici.
*   **Input Field:** Background `#0D0D0D`, Bordo `1px solid #2A2A2A`, Padding `16px 24px`.
*   **Focus State:** Il bordo diventa rosso (`#E60000`) e il placeholder scompare o si rimpicciolisce. Nessun glow (box-shadow diffusa).

### Cards e Contenitori (Glassmorphism)
*   **Pannelli in Sovrimpressione (es. Navbar, Info box):** Sfondo `rgba(3, 3, 3, 0.75)` con `backdrop-filter: blur(16px)`. Questo crea una vetrata tecnica e premium, permettendo alle immagini di sfondo di mantenere la loro profondità.
*   **Bordi Decorativi:** Spesso i contenitori hanno un bordo spesso solo su un lato (es. `border-left: 4px solid #E60000`) per ancorarli visivamente e spezzare la monotonia.

---

## 6. Layout e Spaziature (Grid System)

Il layout "respira" grazie a un uso massiccio dello spazio negativo (vuoto). Questo è il segreto per far percepire un prodotto come lussuoso e non economico.

*   **Sistema a Multipli di 8:** Tutte le spaziature (margin, padding, gap) devono essere multipli di 8px (es. 8, 16, 24, 32, 64, 128).
*   **Section Gap (Distanza tra le sezioni):** Minimo `160px` su desktop per creare pause drammatiche durante lo scroll.
*   **Contenitore Massimo (Max-Width):** `1440px`. Oltre questa larghezza, i contenuti restano centrati ma non si allargano ulteriormente per mantenere proporzioni cinematografiche. Le immagini di sfondo possono andare in "full-bleed" (`100vw`).
*   **Padding Orizzontale Globale:** `24px` su Mobile, `64px` su Desktop.

---

## 7. Fotografia e Storytelling Visivo

Le immagini sono il cuore dell'esperienza Overline. Devono sostituire la componente tattile che manca in uno schermo, facendo percepire il "freddo" dell'acciaio, l'odore del ferro e la ruvidità delle superfici. Nessuna foto stock generica è ammessa.

### Tipologia di Scatti e Inquadrature
*   **Macro sui Materiali (Close-ups):** Inquadrature ravvicinate estreme sulle lavorazioni meccaniche. L'utente deve poter percepire visivamente i solchi della zigrinatura (knurling), ammirare la perfezione del taglio laser, la profondità delle incisioni CNC e il massiccio spessore delle piastre in acciaio.
*   **Product Shot Monolitici:** L'attrezzatura intera (es. tavoli da armwrestling, pulegge) deve essere fotografata come se fosse un monumento. L'uso di angolazioni dal basso verso l'alto (low-angle) è caldamente consigliato per conferire imponenza, stabilità e dominanza al prodotto.
*   **Action Shots (Umani):** Quando sono presenti atleti, il focus non è mai sui volti o sulle espressioni, ma sull'interazione violenta con l'attrezzo. Mani spaccate intrise di magnesite bianca che stringono grip neri, avambracci in trazione massima, sudore sul metallo. L'atleta è solo l'esecutore, la macchina (Overline) è la vera protagonista.

### Illuminazione e Grading (Stile)
*   **Chiaroscuro Drammatico (High Contrast):** L'illuminazione deve essere cinematografica ("Moody Lighting"). Luce dura e direzionale (spesso laterale o in controluce) per incidere i volumi, le forme spigolose e far "uscire" le texture, lasciando ampie zone del prodotto e dello sfondo inghiottite nell'oscurità totale (Deep Shadows).
*   **Color Grading:** Estremamente desaturato e freddo. Le foto devono essere quasi monocromatiche, tendenti ai toni dell'acciaio e della grafite. Si può lasciare spiccare (con moderazione) solo eventuali dettagli in rosso per richiamare il colore d'accento del brand.
*   **Sfondi (Backgrounds):** Gli sfondi devono fondersi con il tema del sito. Sfondi nero assoluto, asfalto bagnato, o cemento industriale sfocato nel buio. Niente colori saturi, niente ambienti diurni luminosi o palestre commerciali affollate. L'atmosfera deve essere isolata e focalizzata.
*   **Vignettatura Naturale:** Gli angoli delle foto fotografate (o editate) dovrebbero sempre sfumare verso il nero scuro (`#030303`) per permettere una transizione pulita e senza stacchi netti (invisible seam) tra l'immagine e lo sfondo della pagina web.

### Regole CSS per Uniformità Fotografica
Nel caso si debbano gestire gallerie dinamiche, per garantire che tutte le immagini mantengano questo rigore "dark and moody", applicare i seguenti filtri:
*   **Stato Base:** `filter: grayscale(25%) contrast(1.15) brightness(0.9);`
*   **Stato Hover (se interattiva):** Restituisce la grinta originale `filter: grayscale(0) contrast(1.1) brightness(1); transition: filter 0.6s power2.out;`

---

## 8. Dinamismo e Animazioni (Motion Design)

L'interazione è il livello che trasforma il sito in un "software premium".
Il sito utilizza pesantemente **GSAP (ScrollTrigger)** e **Lenis (Smooth Scroll)**.

> [!TIP]
> Le animazioni in Overline non devono mai sembrare "giocose" o "leggere" (bounce/spring). Devono simulare il peso fisico e l'inerzia meccanica.

*   **Smooth Scrolling:** Essenziale. Rallenta lo scroll nativo rendendolo vellutato e inerziale.
*   **Reveal dei Testi (Stagger):** I titoli giganti (Anton) appaiono divincolandosi da una maschera sottostante riga per riga, dal basso verso l'alto.
*   **Parallasse Pesante:** Backgrounds che si muovono a `y: "20%"` rispetto alla direzione dello scroll, conferendo profondità.
*   **Scroll-Jacking / Pinned Sections:** Alcune sezioni fondamentali bloccano l'utente (pinning), costringendolo ad osservare un'animazione sequenziale (es. esploso tecnico di un prodotto) prima di farlo proseguire.
*   **Curve di Easing:** Non usare mai `ease-in-out` generici. Usare `expo.out` o `power4.out` con durate lunghe (`1.2s` - `1.5s`). Il movimento deve partire velocissimo e frenare molto lentamente (Attrito).
*   **Magnetic Elements:** I pulsanti e i dot principali sono magnetici: quando il cursore del mouse si avvicina, il bottone si "stacca" leggermente dalla sua posizione verso il cursore.

---

## 9. Iconografia

*   **Stile:** Minimalista, lineare (Stroke), geometrico e affilato.
*   **Specifiche:** Stroke width costante (`1.5px` o `2px`). Nessun riempimento (Fill), tranne in rari casi per indicare l'attivazione.
*   **Libreria Consigliata:** Lucide Icons o un set SVG personalizzato costruito su griglia 24x24px.

---

## 10. Best Practices per lo Sviluppo

*   **Semantica HTML:** Utilizzare `<article>`, `<section>`, `<main>`, `<aside>` per favorire l'accessibilità e la struttura logica (fondamentale per screen reader).
*   **Variabili CSS:** Utilizzare ampiamente `:root` per definire i "Design Tokens" (colori, font-size, spaziature) in modo da poter scalare facilmente eventuali modifiche. Esempio: `var(--color-accent)`.
*   **Performance:** Le immagini ad altissima risoluzione devono essere convertite in formato `.webp` e servite con attributo `loading="lazy"`, ad eccezione dell'hero banner che deve caricare istantaneamente.
