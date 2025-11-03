# Laboratory of Statistical and Mathematical 

- Website https://devangelista2.github.io/statistical-mathematical-methods/2025-26
- Data sets for learning: https://www.kaggle.com
- suggest to work: on virtual environment

## Create Virtual Environment
- apri anaconda primpt da terminale
- conda create --name SMM2526
- conda activate SMM2526
- select kernel environament inside VS in the ipynb

note: environment position ->  C:\Users\richy\anaconda3\envs\SMM2526

## Required libraries
- numpy
- scipy
- pandas
- matplot
...

## Estension
.ipynb -> i python note book

## Rules
- derivatives must be done by hand and not with libraries
- A,B,C are Matrix, v,w,x are vectors, a,b,c are scalars

### Notes
matrix moltiplication: (m,k) * (k,n) -> (m,n)


### Tutor
francesco.pivi2@unibo.it


## Questions 1
Ho capito che lo scopo dell'algoritmo è quello di modulare in maniera adattiva il learning rate. E che lo fa attravero una condizione che controlla che:

Loss_function_allo_step_K+1 

sia minore di:

Loss_function_allo_step_K - (arminijo_constant) * learning_rate * norma_2_gradiente

Immagino anche che il ciclo while serva per diminuire il learning rate affinchè non si "superi" (overshoot) il minimo

la cosa che non mi è chiara è propriò la dimostrazione della formula appena citata. Perchè essa è sufficente per definire un learning rate della giusta dimensione? Ho provato a cercare la risposte su internet però le dimostrazioni non mi sono chiarissime.

## Questions 2
nel algoritmo SDG che abbiamo fatto ad ogni step viene comunque calcolata la loss function per ogni valore di  X, Y. 
avevo letto che SDG dovrebbe prendere solo 1 valore randomico da ogni Batch e computare il gradiente con quello. e Non computare tutti i valori nel batch.
Ho inteso male o esiste anche una versione di SDG come ho descrito io