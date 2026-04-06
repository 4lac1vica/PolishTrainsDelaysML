# Polish Train Delays
ML project which aims to predict the delays for Polish Railways. 

**Tools:** Anaconda Interpreter, PyCharm IDE, Jupyter Notebook.

**Language:** Python 3.11.

**Dataset:** https://www.kaggle.com/datasets/bartek358/train-delays
 

**Note:** The project is still in progress.



## ENGLISH


## ROMANIAN

Acest proiect analizeaza intarzierile trenurilor de pe reteaua feroviara poloneza, folosind tehnici de Exploratory Data
Analysis (EDA).


Scopul este de a intelege : 
    
- distributia intarzierilor 
- rutele cu cele mai mari intarzieri
- garile care au cele mai multe plecari/sosiri

**Dataset**

Datasetul contine informatii despre trenuri. Coloanele principale sunt:

- datetime - data la care datele trenului au fost colectate 
- id - numarul trenului 
- carrier - operatorul trenului (ex. PKP Intercity)
- connection - ruta pe care opereaza trenul (ex. Varsovia - Cracovia)
- arrival - ora de sosire fara adunarea intarzierii
- delay - intarzierea trenului 
- name - numele garii unde a fost monitorizat 

**Preprocesare Date**

- conversia coloanei 'delay' din text ('x min') in numeric
- tratarea valorilor lipsa 
- extractia garii de plecare din coloana 'connection'

**Analiza EDA**

1) Distributia intarzierilor 
    - reprezentare in histograma 
    - identificarea valorilor extreme


2) Cele mai frecvente rute 
    - rutele care sunt cele mai folosite 


3) Rutele cu cele mai mari intarzieri 
    - calculul intarzierii medii pe ruta 


4) Garile cu cele mai multe plecari 
   - identificarile hub-urilor principale

    
**Vizualizare**

Datele sunt reprezentate folosind histograme si barcharts

**Concluzie**

Majoritatea intarzierilor sunt mici, de pana in 30 de minute. Dar exista si valori extreme. 
Varsovia, Cracovia si Gdansk au cele mai aglomerate gari, din punctul de vedere al plecarilor si sosirilor.
Cea mai frecventa ruta este Pruszkow - Otwock. Cel mai frecvent operator este PKP Intercity. 

**Cum sa rulezi**

- creeaza un env folosind conda
````
conda create -n train_env python=3.11
conda activate train_env
````
- instaleaza dependentele 

````
  pip install pandas matplotlib seaborn scikit-learn
````

- ruleaza notebook-ul 

````
jupyter notebook
````




    
