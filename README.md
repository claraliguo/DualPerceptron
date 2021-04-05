# DualPerceptron
Progetto AI

L'algoritmo di apprendimento supervisionato del perceptron è uno dei più utilizzati per la classificazione in quanto semplice ed interpretabile.

Lo scopo di questo progetto  è sperimentare opportuni valori di gamma, analizzando il validation error. 
Il progetto si divide in due parti:
  - nella prima si chiede di implementare l'algoritmo di Perceptron Duale descritto in Cristianini & Shawe-Taylor 2002 utilizzando come Kernel l'RBF kernel, descritto nel dettaglio nella relazione allegata.
  - nella seconda si chiede di applicare l'algoritmo al dataset MNIST, il quale porterà a trovarsi dinanzi al problema di classificazione multiclasse, poichè le cifre scritte a mano del dataset vanno da 0 a 9.

Il primo file perceptronduale1.py è da eseguire modificando per 3 volte il valore del parametro gamma della funzione rbf_kernel che ritorna il valore del kernel nell'addestramento del Perceptron Duale.
  - Il primo valore di gamma è 0.1 e il validation error ottenuto è 11.25%
  - Il secondo valore di gamma è 0.02 e il validation error ottenuto è 12.50%
  - Il terzo valore di gamma è 0.05 e il validation error ottenuto è 28.75%

Il secondo file perceptronduale2.py è anch'essa da eseguire modificando il valore del parametro gamma della funzione rbf_kernel.

Le osservazioni sui vari risultati ottenuti cambiando i valori per gamma sono argomentate nella relazione allegata.
