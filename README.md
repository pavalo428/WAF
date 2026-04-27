[READ ME.txt](https://github.com/user-attachments/files/27111605/READ.ME.txt)
1. INSTALLER LES DÉPENDANCES :

   pip install flask pandas scikit-learn joblib


2. LANCER LE SERVEUR

   python app.py


3. OUVRIR LE LIEN DE L'APPLICATION :

   http://127.0.0.1:5000


4. SAISIR DANS LE NAVIGATEUR LES REQUETES SUIVANTES :
 
 
    http://127.0.0.1:5000/login?user=test               (REQUETE NORMALE QUI RETOURNE UN `OK`)
    
    http://127.0.0.1:5000/login?user=admin' OR 1=1--         (REQUETE SQL QUI RETOURNE `BLOCKED`)

    http://127.0.0.1:5000/search?q=<script>alert(1)</script>      (REQUETE XSS QUI RETOURNE ÉGALEMENT `BLOCKED`)
