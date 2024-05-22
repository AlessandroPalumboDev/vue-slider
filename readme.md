Descrizione:
Partendo dal markup della versione svolta in js plain, rifare lo slider ma questa volta usando Vue.
Sorpresa: Vi lascio un markup html bello pronto da utilizzare, se volete potete partire da questo.

- Bonus:
- 1- al click su una thumb, visualizzare in grande l'immagine corrispondente

- 2- applicare l'autoplay allo slider: ogni 3 secondi, cambia immagine automaticamente

- 3- quando il mouse va in hover sullo slider, bloccare l'autoplay e farlo riprendere quando esce


- Ricreo lo slider base usando Vue e i file html e css forniti
    - Creo variabile dell app che ritorna l'array di oggeti e un contatore dell'indice
    - Uso v-for per selezionare solo l'elemento dell'array che mi serve sfruttando il contatore dell indice 
    - Uso v-bind per l'indirizzo dell'immagine e alt 
    - Uso @click sui tasti per evento al click usando la stessa logica del vecchio esercizio

- BONUS 1
    - Riutilizzo lo stesso v-for per la visualizzazione delle immagini dello slider per le thumb creando un nuovo method pe l'evento al click

- BONUS 2
    - Sfruttando il ciclo di vita dell'app uso un setInterval di tre secondi che usa la funzione di freccia avanti

- BONUS 3
    - aggiungo eventi al passaggio del mouse sullo slider @mouseenter @mouseleave che sfruttano le funzioni che gestiscono l'autoplay
    - nei data aggiungo una chiave al return nulla
    - creo la funzione di autoplay tra i methods che modifica la chiave nulla e la richiamo in mounted
    - creo la funzione di stop con clearInterval