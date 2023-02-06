# Biblioteca 🛴

Scrivere un programma che permetta di gestire una Biblioteca semplificata, in grado di gestire un array
di indici (interi) dei libri che contiene. La Biblioteca viene costruita a partire da un array di 
indici di libri.
In particolare, implementare i seguenti metodi:
- `esisteLibro`: prende un indice e restituisce true se esiste il libro con questo indice, false altrimenti
- `getIndiciLibriOrdinati`: ritorna la lista degli indici di libri presenti nella biblioteca, in ordine ascendente

Potete utilizzare il seguente codice come test:

```java
public class Main {
    public static void main(String[] args) {
        int[] values = new int[7];
        values[0] = 123;
        values[1] = 4;
        values[2] = 98;
        values[3] = 33;
        values[4] = 76;
        values[5] = 2;
        values[6] = 235;
        Biblioteca biblioteca = new Biblioteca(values);
        System.out.println(biblioteca.esisteLibro(76));
        int[] libriOrdinati = biblioteca.getIndiciLibriOrdinati();
        System.out.println(libriOrdinati[0] == 2);
        System.out.println(libriOrdinati[1] == 4);
        System.out.println(libriOrdinati[2] == 33);
        System.out.println(libriOrdinati[3] == 76);
        System.out.println(libriOrdinati[4] == 98);
        System.out.println(libriOrdinati[5] == 123);
        System.out.println(libriOrdinati[6] == 235);
    }
}
```

Suggerimento: riutilizzate il codice dei precedenti esercizi

## Biblioteca2

Rendere la biblioteca funzionante con dei libri veri e propri invece che con solo i loro indici.
Creare quindi una classe Libro con delle proprie caratteristiche, tra cui l'indice che usavamo prima,
ad esempio nome, autore, categoria, ecc, e modificare di conseguenza la classe Biblioteca ed il main di test.


