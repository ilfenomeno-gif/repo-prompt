# 📚 SCHEDA D’USO COMPLETA – TUTTI I PROMPT STRATEGICI PER AI

## Indice rapido

| Zona | Prompt |
|------|--------|
| **Generali** | 1. Framework Prompt Universale<br>2. Agente Autonomo & Cooperativo<br>3. Game Design Analyzer<br>4. Problem Solver a 4 Fasi<br>5. AI Prompt Enhancer<br>6. DUSU – Master Prompt Architect |
| **Specialistici** | 7. DeepReasoner<br>8. AI Fundamentals Coach<br>9. Honesty Extractor<br>10. Prompt Ingegnere Software<br>11. (già incluso DUSU come #6) |

> In realtà i file sono 11, ma DUSU è già al punto 6. Tutti coperti.

---

## 1. Framework Prompt Universale

| Specifica | Dettaglio |
|-----------|-----------|
| **A cosa serve** | Dare all’AI una struttura rigida (ruolo, task, contesto, formato, avvertenze, valutazione) per ottenere risposte oggettive, verificabili e migliorabili. |
| **Tipo di IA** | ChatGPT, Claude, Gemini, Copilot (qualsiasi LLM testuale) |
| **Lunghezza risposta** | 500‑2000 parole (dipende dal task) |
| **Flusso operativo** | 1. Copia l’intero prompt fino a “Ora, dimmi il tuo compito”.<br>2. Incollalo all’inizio della chat.<br>3. Sostituisci `[descrivi qui...]` con il tuo task reale.<br>4. L’AI risponderà con: ruolo, obiettivo, task, contesto, formato, RADAR, sintesi, prossimo passo. |
| **❌ Come NON usarlo** | Non omettere la sezione “Ora, dimmi il tuo compito”. Se non sostituisci il segnaposto, l’AI chiederà il task (funziona comunque, ma perde tempo). |
| **Verifica funzionamento** | La risposta deve contenere le sezioni: `## [TITOLO RISPOSTA]`, `Livello attivato`, `✅ VERITÀ TRACCIABILE (RADAR)`, `⚠️ AVVERTENZE`, `📋 SINTESI ESECUTIVA`, `🔄 PROSSIMO PASSO`. |
| **💡 Chicca** | Puoi forzare il livello di complessità scrivendo `[LIVELLO: Rapido]` nel task. Il prompt supporta tre livelli (Rapido, Standard, Approfondito). |

---

## 2. Agente Autonomo & Cooperativo

| Specifica | Dettaglio |
|-----------|-----------|
| **A cosa serve** | Far eseguire all’AI compiti complessi in autonomia (senza chiedere conferme intermedie) e, se presenti altri agenti nello stesso workspace, delegare loro sotto‑task. |
| **Tipo di IA** | Microsoft Copilot (modalità Agente), ChatGPT con plugin di tool calling, Claude con computer use. Su ChatGPT standard funziona solo la parte autonoma (non la delega). |
| **Lunghezza risposta** | 300‑1000 parole + azioni/esecuzioni |
| **Flusso operativo** | 1. Incolla il prompt in Copilot.<br>2. Specifica obiettivo e, se presenti, elenca gli altri agenti con nome e competenze.<br>3. L’AI scompone il task, esegue autonomamente o delega.<br>4. Alla fine produce un riepilogo azioni. |
| **❌ Come NON usarlo** | Dichiarare agenti che non esistono → l’AI proverà a delegare e fallirà. Meglio non menzionarli se non presenti. |
| **Verifica funzionamento** | La risposta deve includere “Esecuzione autonoma” o “Delega effettuata”. |
| **💡 Chicca** | Prima di delegare, l’AI risponde mentalmente a 3 domande (agenti presenti? competenze adatte? contesto compatibile?). Se una risposta è “no”, esegue tutto da solo. |

---

## 3. Game Design Analyzer

| Specifica | Dettaglio |
|-----------|-----------|
| **A cosa serve** | Analizzare e sviluppare idee per giochi (videogiochi, da tavolo, MUD) seguendo una pipeline in 4 fasi: Discovery, Strategia, Allineamento, Azione. |
| **Tipo di IA** | ChatGPT, Claude, Gemini (finestra di contesto lunga) |
| **Lunghezza risposta** | Fase 1: domande brevi. Fasi 2‑4: 1000‑3000 parole. |
| **Flusso operativo** | 1. Copia e incolla il prompt.<br>2. Sostituisci `[INSERIRE IDEA/CONTESTO]` con la tua idea.<br>3. Aggiungi “Inizia dalla Fase 1.”<br>4. Rispondi alle domande della Fase 1.<br>5. L’AI procede automaticamente alla Fase 2, 3, 4. |
| **❌ Come NON usarlo** | Non rispondere a tutte le domande della Fase 1 → l’AI resta in attesa. Non chiedere di saltare fasi → il framework si rompe. |
| **Verifica funzionamento** | La risposta deve iniziare con “Fase 1: Discovery” e domande chiare. Alla fine della Fase 4, produce executive summary, roadmap, rischi. |
| **💡 Chicca** | Nella Fase 4 chiede esplicitamente di valutare “feature creep” (troppe funzioni inutili) – già integrato nel framework. |

---

## 4. Problem Solver a 4 Fasi

| Specifica | Dettaglio |
|-----------|-----------|
| **A cosa serve** | Affrontare qualsiasi problema complesso (business, personale, tecnico) senza risposte affrettate. Obbliga l’AI a: 1) chiarimenti, 2) proposta approccio, 3) revisione, 4) piano finale. |
| **Tipo di IA** | Qualsiasi LLM |
| **Lunghezza risposta** | Fase 1: domande brevi. Fase 2: 200‑500 parole. Fase 3: 100‑300. Fase 4: 500‑1500. |
| **Flusso operativo** | 1. Incolla il prompt.<br>2. Descrivi il problema (anche vago).<br>3. L’AI risponde con “Fase 1: Chiarimenti”.<br>4. Rispondi punto per punto.<br>5. L’AI passa alla Fase 2 e poi aspetta il tuo consenso per la Fase 3 (“procedi alla Fase 3”). |
| **❌ Come NON usarlo** | Dare il consenso esplicito solo quando sei sicuro. Se non dai consenso, l’AI resta in attesa. |
| **Verifica funzionamento** | La risposta deve menzionare “Fase 1”, “Fase 2”, ecc. Se l’AI dà subito soluzione senza domande, il prompt non è stato applicato. |
| **💡 Chicca** | Se l’utente salta una fase, il prompt dice: *“Per garantire un piano corretto, questa fase non può essere saltata.”* È uno dei pochi prompt che “si difende” da solo. |

---

## 5. AI Prompt Enhancer (6 Parti + 5 Hack)

| Specifica | Dettaglio |
|-----------|-----------|
| **A cosa serve** | Trasforma qualsiasi IA in un esperto di prompt engineering che applica automaticamente: rilevatore di verità, assistente prompt, loop di automiglioramento (3 round), “pensa passo dopo passo”, priming. |
| **Tipo di IA** | ChatGPT, Claude, Gemini, Copilot (meglio modelli recenti per il rilevatore di verità) |
| **Lunghezza risposta** | Variabile, sempre con percentuali di sicurezza e ragionamento step‑by‑step. |
| **Flusso operativo** | 1. Copia il prompt dalla prima riga “Agisci come un esperto...” fino a “Ora, dimmi il tuo compito”.<br>2. Incolla all’inizio della chat.<br>3. Scrivi il tuo compito (anche dopo).<br>4. L’AI applica automaticamente i 5 hack. |
| **❌ Come NON usarlo** | Non puoi disattivare il rilevatore di verità: è obbligatorio e restituirà sempre % di sicurezza. Se non vuoi questo, usa un altro prompt. |
| **Verifica funzionamento** | La risposta deve contenere almeno una percentuale (es. “95%+”) oppure la frase “Pensa passo dopo passo”. |
| **💡 Chicca** | Il loop di automiglioramento fa 3 round **invisibili** e ti mostra solo la versione finale. Puoi chiedere il confronto “prima/dopo” se vuoi vedere il progresso. |

---

## 6. DUSU – Master Prompt Architect (già “geratore prompt professionale”)

| Specifica | Dettaglio |
|-----------|-----------|
| **A cosa serve** | Il tuo prompt più avanzato. Progetta, analizza e migliora altri prompt. Usa 3 livelli di profondità (Rapido, Standard, Approfondito), 6 leggi IA inviolabili, loop di 3 round, RADAR, audit finale. |
| **Tipo di IA** | ChatGPT, Claude, Gemini, Copilot (consigliato GPT-4o o Claude 3.5+ per il livello Approfondito) |
| **Lunghezza risposta** | Da 300 parole (Rapido) a 3000+ (Approfondito) |
| **Flusso operativo** | 1. Incolla l’intero prompt DUSU.<br>2. Scrivi il tuo task (es. “Crea un prompt per un coach di vendite”).<br>3. DUSU esegue il doppio audit iniziale, sceglie il livello, applica F.U.G.P. e produce il prompt ottimale. |
| **❌ Come NON usarlo** | Non usare DUSU per domande semplici (es. “che ore sono?”) – sarebbe un uso sproporzionato. Usa invece il livello Rapido. |
| **Verifica funzionamento** | La risposta deve terminare con il blocco `[AUDIT DUSU]` a forma di riquadro. |
| **💡 Chicca** | DUSU **inietta automaticamente** le 6 Leggi IA e il formato di output in ogni prompt che genera. Non puoi dimenticartele. |

---

## 7. DeepReasoner (Ragionamento approfondito + XML)

| Specifica | Dettaglio |
|-----------|-----------|
| **A cosa serve** | Costringe l’AI a ragionare a lungo, autovalutarsi internamente con criteri e fornire risposte in XML (`<analisi>`, `<dettagli>`, `<raccomandazioni>`). Ideale per problemi strategici, analisi, coding complesso. |
| **Tipo di IA** | GPT‑4o, Claude 3.5+, Gemini 1.5+ (modelli con forte capacità di seguire istruzioni) |
| **Lunghezza risposta** | 300‑800 parole (modificabile cambiando il tag `<VERBOSITA>`) |
| **Flusso operativo** | 1. Copia tutto il prompt (da `[RUOLO]` alla fine).<br>2. Incolla nella chat.<br>3. Scrivi la tua domanda.<br>4. L’AI esegue l’autovalutazione interna (invisibile) e produce solo l’output XML finale. |
| **❌ Come NON usarlo** | Su GPT‑3.5 o modelli vecchi l’autovalutazione interna è inefficace. Non usare per domande banali (fa comunque tutto il processo). |
| **Verifica funzionamento** | La risposta deve contenere almeno due tag XML (`<analisi>`, `<dettagli>`, `<raccomandazioni>`). |
| **💡 Chicca** | Puoi cambiare la lunghezza modificando la frase in `<VERBOSITA>`: esempio “risposta molto breve, 100 parole” produce output compatto ma sempre strutturato. |

---

## 8. AI Fundamentals Coach (5 Fondamentali 2026)

| Specifica | Dettaglio |
|-----------|-----------|
| **A cosa serve** | Insegna i 5 fondamentali per usare l’IA in modo efficace: **COSTAR** (per prompt), classificazione dei 4 strumenti, agenti AI, integrazione dati personali, vibe coding. Non promuove tool specifici. |
| **Tipo di IA** | Qualsiasi LLM testuale |
| **Lunghezza risposta** | 200‑1500 parole, strutturata in elenchi o sezioni |
| **Flusso operativo** | 1. Incolla il prompt (da `[RUOLO]` a “Ora attendi la richiesta”).<br>2. Fai una domanda su un fondamentale (es. “Aiutami a scrivere un prompt per un reel”).<br>3. L’AI risponde applicando la regola corrispondente. |
| **❌ Come NON usarlo** | Non chiedere “parlami dell’IA” senza specificare – riceverai una risposta generica. Meglio essere precisi: “Spiegami il vibe coding con un esempio”. |
| **Verifica funzionamento** | La risposta deve menzionare almeno uno di: COSTAR, cervello generale, agente AI, dati personali, vibe coding. |
| **💡 Chicca** | Se chiedi “Quale strumento usare per X?”, l’AI classifica la risposta in una delle 4 categorie (cervello, ricerca, specialista, automazione) e segue la “regola d’uso” che hai scritto nel prompt. |

---

## 9. Honesty Extractor (Estrazione dati obiettiva)

| Specifica | Dettaglio |
|-----------|-----------|
| **A cosa serve** | Estrarre dati da documenti (contratti, PDF, email, Excel) **senza alcuna allucinazione**. L’AI deve lasciare vuoto qualsiasi campo non esplicitamente dichiarato, etichettare ogni dato come “estratto” o “inferito” e produrre un audit di affidabilità. |
| **Tipo di IA** | ChatGPT, Claude, Gemini (con supporto a file allegati) |
| **Lunghezza risposta** | Tabella + audit: da 10 righe a centinaia (dipende da campi e documento) |
| **Flusso operativo** | 1. Copia il prompt in una chat nuova.<br>2. Allega il documento (o incolla il testo).<br>3. Specifica i campi da estrarre (es. “nome cliente, data, importo”).<br>4. L’AI produce una tabella con colonne `Campo | Valore | Fonte | Evidenza | Motivo vuoto`.<br>5. Aggiunge la sezione Audit con livelli ALTO/MEDIO/BASSO. |
| **❌ Come NON usarlo** | Chiedere decine di campi in una volta → l’AI potrebbe perderne qualcuno. Meglio 5‑10 campi per richiesta. |
| **Verifica funzionamento** | La tabella deve contenere almeno un campo vuoto con “Motivo vuoto” compilato, o un campo “inferito” con “Evidenza”. Se tutta la tabella è “estratto” senza mai un vuoto, probabilmente l’AI ha inventato. |
| **💡 Chicca** | Il prompt incorpora la “penalità”: *“Una risposta SBAGLIATA è 3× peggiore di una risposta VUOTA.”* Questo cambia radicalmente il comportamento dell’AI, che diventa molto più conservativa. |

---

## 10. Prompt Ingegnere Software (Modalità Produzione)

| Specifica | Dettaglio |
|-----------|-----------|
| **A cosa serve** | Trasforma l’AI in un ingegnere del software obiettivo, deterministico e quantitativo. Struttura ogni risposta in: Analisi, Soluzione (con codice production‑ready, pattern, complessità O‑grande), Valutazione (tabella pro/contro con metriche), Alternative. Vieta opinioni e aggettivi vaghi. |
| **Tipo di IA** | ChatGPT, Claude, Gemini, Copilot (modelli con buona capacità di seguire strutture) |
| **Lunghezza risposta** | 300‑1500 parole (dipende dal codice) |
| **Flusso operativo** | 1. Incolla il prompt all’inizio della chat.<br>2. Scrivi la domanda tecnica **specificando il linguaggio** (es. “In Python, leggi CSV da 10 GB senza esaurire RAM”).<br>3. L’AI risponde con le 4 sezioni obbligatorie. |
| **❌ Come NON usarlo** | Non omettere il linguaggio di programmazione → l’AI chiederà chiarimenti (comportamento corretto, ma rallenta). Non chiedere opinioni (“secondo te è meglio X o Y?”) – l’AI rifiuterà e darà una tabella comparativa quantitativa. |
| **Verifica funzionamento** | La risposta deve avere le intestazioni `📐 Analisi (obiettiva)`, `⚙️ Soluzione ingegneristica`, `📊 Valutazione oggettiva`. La tabella Pro/Contro deve contenere metriche misurabili (es. “Spazio O(n)”, “latenza +20%”), non aggettivi. |
| **💡 Chicca** | Include un meccanismo di “incertezza”: se l’AI non è sicura sulla versione di una libreria o sull’OS, antepone `⚠️ [Condizione di incertezza]` e lista le assunzioni. |

---

## 🔗 COMBINAZIONI TRA PROMPT (le combo killer)

| Combo | Cosa fa | Flusso |
|-------|---------|--------|
| **Honesty Extractor + DUSU** | Estrai dati da un documento e poi fai generare a DUSU un prompt per usarli. | 1. Honesty Extractor su contratto → ottieni tabella pulita.<br>2. Incolla la tabella come contesto in DUSU e chiedi: “Crea un prompt per un agente che analizzi questi dati”. |
| **Problem Solver + DeepReasoner** | Risolvi problemi complessi con doppia profondità. | 1. Problem Solver produce il piano finale (Fase 4).<br>2. Per ogni fase del piano, chiedi a DeepReasoner: “Applica ragionamento approfondito a questo punto del piano”. |
| **AI Fundamentals Coach + Prompt Ingegnere Software** | Impara il fondamentale “vibe coding” e poi applica subito un prompt tecnico. | 1. Chiedi al Coach: “Spiegami il vibe coding con un esempio di calcolatrice”.<br>2. Poi usa Prompt Ingegnere Software: “Genera il codice per quella calcolatrice in React”. |
| **Framework Universale + Agente Autonomo** | Struttura un task complesso e poi lo esegue in autonomia. | 1. Framework Universale produce un piano dettagliato con livelli e RADAR.<br>2. Copia la sezione “Piano d’azione” e incollala in Agente Autonomo dicendo: “Esegui questo piano senza chiedere conferme”. |

---

## 💡 CHICCHE GENERALI (pratiche trasversali)

| | |
|---|---|
| 1 | Prima di usare un prompt, leggi sempre la sezione “Verifica funzionamento” – così sai subito se l’AI lo ha applicato correttamente. |
| 2 | Usa il livello “Rapido” di DUSU o del Framework Universale per domande semplici – non attivare mai l’Approfondito se non serve. |
| 3 | Salva i prompt migliori come “Prompt di sistema” nelle chat che usi spesso (es. Honesty Extractor per l’estrazione dati quotidiana). |
| 4 | Se un prompt produce una risposta troppo lunga o troppo corta, modifica il “Formato di output” direttamente nella copia che usi – aggiungi “max 300 parole” o “risposta in 5 punti”. |
| 5 | La combo più potente per report aziendali:<br>- Honesty Extractor → estrae i numeri reali da documenti.<br>- DeepReasoner → analizza i trend e le cause.<br>- DUSU → genera un prompt per automatizzare l’intero flusso la prossima volta. |
| 6 | Tutti i prompt che contengono le “Leggi IA” (DUSU, Framework Universale, Honesty Extractor) sono tra loro compatibili – puoi unirli tagliando e incollando le sezioni. Usa come base DUSU e innesta Honesty Extractor per l’estrazione. |

---

## ✅ RIEPILOGO – quale prompt usare per cosa?

| Se vuoi... | Usa... |
|------------|--------|
| Una risposta generica ma ben strutturata | Framework Universale (livello Standard) |
| Che l’AI esegua un task da sola senza romperti | Agente Autonomo & Cooperativo |
| Progettare un gioco dall’idea al documento | Game Design Analyzer |
| Risolvere un problema senza risposte affrettate | Problem Solver a 4 Fasi |
| Migliorare un prompt esistente o scriverne uno nuovo | AI Prompt Enhancer |
| Un prompt professionale che rispetta 6 leggi IA | DUSU – Master Prompt Architect |
| Un ragionamento profondissimo in formato XML | DeepReasoner |
| Imparare i 5 fondamentali dell’IA | AI Fundamentals Coach |
| Estrarre dati da un documento senza allucinazioni | Honesty Extractor |
| Codice production‑ready con metriche quantitative | Prompt Ingegnere Software |
