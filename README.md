# Modello_di_diffusione_quantistico_per_la_simulazione_di_immagini_galattiche
Codice Python per un modello di diffusione quantistico per la generazione di immagini di galassie

Il file QDM_dissertazione è una dissertazione teorica sul modello di diffusione quantistico implementato.

Nel file QDM_Definitivo_GitHub.ipynb è presente il codice per la generazione delle immagini galattiche. 
In particolare nel file è presente sia il codice necessario per addestrare da zero autoencoder e circuito quantistico
sia il codice necessario per caricare i parametri dei modelli pre-addestrati utilizzati per la dissertazione. 
Porre attenzione alla modalità di caricamento dei dati, selezionare la corretta cartella in cui sono stati salvati i parametri prima di eseguire la cella corrispondente.

Nei file autoencoder.pth e Circuiti_parametrici.zip sono disponibili i parametri dei modelli pre-addestrati che possono essere caricati nel codice per la generazione delle immagini.
Nella cartella Circuiti_parametrici sono contenuti i paramtri di tutti i 15 circuiti. vanno eseguiti in ordine considerando la seguente notazione: circuito_t+1_t.pth svolge il denoising dal passo t+1 a t.

Nel file Decoder_esterno.ipynb è presente il codice per l'addestramento del decoder necessario per aumentare la risoluzione delle immagini generate fino a 256x256
Nel file Decoder_esterno.pth sono presenti i parametri del decoder pre-addestrato per l'aumento della risoluzione

Nel file encodend_images.zip è presente una copia del fil autoencoder.pth oltre che tutte le immagini del dataset compresse (8x8) dall'encoder di autoencoder.pth
Questo file è particolarmente pesante e si può evitare di scaricarlo qualora si usino i circuiti quantistici già addestrati o in alternativa si esegua la relativa cella per il
salvataggio sul drive dei vettori dello spazio latente direttamente dal codice QDM_Definitivo_GitHub.ipynb
