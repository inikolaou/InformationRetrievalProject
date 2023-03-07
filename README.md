Η γλώσσα προγραμματισμού που χρησιμοποιήθηκε είναι η Python και συγκεκριμένα η έκδοση 3.10 μαζί με τις βιβλιοθήκες numpy, pandas, tensorflow, keras και elasticsearch (συγκεκριμένη έκδοση 7.10 κι επιλέχτηκε επειδή είναι η νεότερη έκδοση που ήταν ακόμα open source).
Η εγκατάσταση της Python είναι σχετικά απλή, πατώντας αυτό το σύνδεσμο οδηγούμαστε στη σελίδα για την εγκατάσταση της Python όπου διαλέγουμε το κατάλληλο link σύμφωνα με το λειτουργικό σύστημα που έχουμε.
Μαζί με την εγκατάσταση της Python έχουμε και τον package manager pip, οπότε μπορούμε να τρέξουμε την εντολή pip install -r requirements.txt ώστε να κατέβουν όλες οι απαραίτητες βιβλιοθήκες.
Επόμενο βήμα είναι να εγκαταστήσουμε την elasticsearch. Ο τρόπος που επιλέξαμε εμείς είναι μέσω του docker. Για να εγκαταστήσει κάποιος το docker ακολουθεί αυτό τον σύνδεσμο. Μαζί με το docker κατεβαίνει και το docker compose.
Στο φάκελο με τον κώδικα της εργασίας υπάρχει ένα αρχείο docker-compose.yml. Πρέπει να πάμε σ’ αυτό το φάκελο που βρίσκεται αυτό το αρχείο και στο terminal να τρέχουμε την εντολή docker-compose up -d. Με αυτή την εντολή θα δημιουργηθεί ένα container το οποίο περιέχει την elasticsearch και το kibana τα οποία μπορούμε να τα κάνουμε access από τις διευθύνσεις: http://localhost:9200/ - Elastic Search API και http://localhost:5601/ - Kibana Web UI interface. Κάθε φορά θα ανοίγουμε το docker desktop και θα ενεργοποιούμε τα services πατώντας το play κουμπί του elasticsearch container.
