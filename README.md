# DualPerceptron
Progetto AI

L'algoritmo di apprendimento supervisionato del perceptron è uno dei più utilizzati per la classificazione in quanto semplice ed interpretabile.

Lo scopo di questo progetto  è sperimentare opportuni valori di gamma, analizzando il validation error. 
Il progetto si divide in due parti:
  - nella prima si chiede di implementare l'algoritmo di Perceptron Duale descritto in Cristianini & Shawe-Taylor 2002 utilizzando come Kernel l'RBF kernel, descritto nel dettaglio nella relazione allegata.
  - nella seconda si chiede di applicare l'algoritmo al dataset MNIST, il quale porterà a trovarsi dinanzi al problema di classificazione multiclasse, poichè le cifre scritte a mano del dataset vanno da 0 a 9.

Il primo file perceptronduale1.py è da eseguire modificando per 3 volte il valore del parametro gamma della funzione rbf_kernel che ritorna il valore del kernel nell'addestramento del Perceptron Duale. L'algoritmo di apprendimento di questa prima parte è stato applicato sul dataset load_breast_cancer, per la classificazione binaria.

  - Il primo valore di gamma è 0.1 e il validation error ottenuto è 11.25%
  - Il secondo valore di gamma è 0.02 e il validation error ottenuto è 12.50%
  - Il terzo valore di gamma è 0.05 e il validation error ottenuto è 28.75%


Il secondo file perceptronduale2.py è anch'essa da eseguire modificando il valore del parametro gamma della funzione rbf_kernel, però sul dataset MNIST, per la classificazione multiclasse, considerando due classi a scelta. Per procedere con quest'ultimo passaggio, è possibile codificare le 10 classi del MNIST con la codifica Unary (one-hot) coding, scegliendo le due classi e considerando, per ogni nuova istanza che deve essere classificata, entrambe le funzioni assegnando il punto alla classe corrispondente secondo una condizione, meglio argomentata nella relazione allegata:

    y_train = np_utils.to_categorical(y_train)
    y_test = np_utils.to_categorical(y_test)
    num_classi = y_train.shape

(np_utils.to_categorical è importata da Keras)

Le osservazioni sui vari risultati ottenuti cambiando i valori per gamma sono argomentate nella relazione allegata.
