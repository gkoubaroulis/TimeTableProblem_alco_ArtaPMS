# Εργασία μαθήματος "Προχωρημένοι αλγόριθμοι και Δομές Δεδομένων" 2020-2021

## 1. Εργασία μαθήματος "Προχωρημένοι αλγόριθμοι και Δομές Δεδομένων"
Πολλές φορές στην καθημερινότητα παρουσιάζονται προβλήματα που οι λύσεις τους είναι πολύπλοκές, ονομάζονται προβλήματα συνδυαστικής βελτιστοποίησης. Οι λύσεις των προβλημάτων συνδυαστικής βελτιστοποίησης, έχοντας ένα σύνολο περιορισμών,  είναι αυτές που επιτυγχάνουν το καλύτερο δυνατό αποτέλεσμα με συγκεκριμένα δεδομένα, σε αυτή την κατηγορία προβλημάτων μπορούμε να εντάξουμε το πρόβλημα δημιουργίας προγράμματος εξετάσεων στα πανεπιστημιακά ιδρύματα. Στο τέλος κάθε εξαμήνου πρέπει να οργανωθούν εξετάσεις το πρόγραμμα που θα βγει πρέπει να ικανοποιεί συγκεκριμένους περιορισμούς. Το πρόβλημα δεν είναι καινούργιο, το έχουν προσεγγίσει ερευνητές σε όλο το κόσμο προσπαθώντας να βρουν αποδοτικές λύσεις. Μια απλοποιημένη μορφή του προβλήματος έχει προταθεί από τους Carter, Laporte και Lee το 1996 δίνοντας μαζί και 13 στιγμιότυπα προβλημάτων από κάποια εκπαιδευτικά ιδρύματα του Καναδά, Αμερικής, Ηνωμένου Βασιλείου και Μέσης Ανατολής συνολικά είναι γνωστό ως “Toronto Benchmark Data”. Η βέλτιστη λύση των προβλημάτων αυτών δεν παράγεται σε πολυωνυμικό χρόνο  αλλά ενδεχομένως να απαιτείται εκθετικός. Η παρούσα εργασία αποσκοπεί στη κατασκευή υπολογιστικής εφαρμογής τέτοια ώστε να παράγει λύσεις σε αυτό το πρόβλημα με τα συγκεκριμένα στιγμιότυπα. Εφαρμόστηκε αλγόριθμος άπληστης μεθόδου για την παραγωγή λύσης, τα αποτελέσματα των προβλημάτων ποίκιλαν βάσει της μορφολογίας κάθε στιγμιότυπο δεδομένων.

## 2. Χρωματισμός Γραφήματος 
Στη θεωρία γραφημάτων , χρωματισμού γραφήματος είναι μια ειδική περίπτωση της επισήμανσης γράφημα. Είναι μια διαδικασία εκχώρησης ετικετών, που παραδοσιακά ονομάζονται "χρώματα", σε στοιχεία ενός γραφήματος που υπόκεινται σε ορισμένους περιορισμούς. Στην απλούστερη μορφή του, είναι ένας τρόπος χρωματισμού των κορυφών ενός γραφήματος έτσι ώστε καμία γειτονική κορυφή να έχει το ίδιο χρώμα. αυτό ονομάζεται χρωματισμός κορυφής . Παρομοίως, ένας χρωματισμός άκρου εκχωρεί ένα χρώμα σε κάθε άκρη, έτσι ώστε δεν υπάρχουν δύο γειτονικές άκρες του ίδιου χρώματος, και ένας χρωματισμός προσώπου ενός επίπεδου γραφήματος εκχωρεί ένα χρώμα σε κάθε πρόσωπο ή περιοχή, έτσι ώστε δεν υπάρχουν δύο όψεις που μοιράζονται ένα όριο ίδιο χρώμα.

![](https://www.codeproject.com/KB/recipes/graph_coloring_using_RLF/gcq_3.png)

## 3. Επίλυση προβλήματος "Χρονοπρογραμματισμού Εξετάσεων Πανεπιστημίου"

### Περιγραφή προβλήματος

Το πρόβλημα χρονοπρογραμματισμού εξετάσεων σε πανεπιστημιακό ίδρυμα αφορά 1ον  τα εξεταζόμενα μαθήματα της εξεταστικής, 2ον τους σπουδαστές που έχουν δηλώσει τα μαθήματα που θα εξεταστούν και 3ον τον αριθμό περιόδων εξετάσεων σε κάθε μια από τις οποίες μπορούν να εξεταστούν ένα ή περισσότερα μαθήματα(εξετάσεις). Το κάθε μάθημα το παρακολουθούν ένα σύνολο από σπουδαστές και κάθε σπουδαστής είναι εγγεγραμμένος σε ένα ή περισσότερα μαθήματα. Ζητούμενο είναι η δημιουργία προγράμματος εξέτασης μαθημάτων τέτοιο ώστε σε κάθε εξεταστική περίοδο να εξεταστούν μαθήματα ένα ή περισσότερα σε κάθε φορά με τον αυστηρό περιορισμό μαθήματα που είναι στην ίδια περίοδο να μην έχουν  ίδιους  εγγεγραμμένους σπουδαστές, σε περίπτωση παρουσίασης του φαινομένου αυτού θα έχουμε σύγκρουση και θα πρέπει να κάνουμε περαιτέρω αναζήτηση λύσης καθώς είναι πιθανό να υπάρχουν εναλλακτικά προγράμματα που ικανοποιούν τον παραπάνω περιορισμό που τέθηκε στην αρχή του προβλήματος.

Τα Δεδομένα δοκιμών γνωστά και ως "Benchmark Data sets in Exam Timetableling" μπορούμε να τα αναζητήσουμε στο παρακάτω site: 
* [Benchmark Data Sets in Exam Timetabling](http://www.asap.cs.nott.ac.uk/external/resources/)

## 4. Κώδικας εφαρμογής.

* [start.cpp](/src2/start.cpp): Στο αρχείο αυτό βρίσκεται το αρχικό μενού όπου από εκεί καλούνται όλες οι συναρτήσεις  επίλυσης του προβλήματος.

* [menuFun.cpp](/src2/menuFun.cpp): Στο αρχείο βρίσκονται συναρτήσεις  σχετικές με τα μενού που εμφανίζονται στην οθόνη.

* [graph.cpp](/src2/graph.cpp): Στο αρχείο αυτό υπάρχει ο αλγόριθμος επίλυσης του προβλήματος, επιστρέφει στο κυρίως αρχείο ένα πίνακα με τους χρωματισμούς των κορυφών.

* [dataFun.cpp](/src2/dataFun.cpp): Στο αρχείο αυτό βρίσκονται συναρτήσεις διαχείρισης δεδομένων και αποθήκευσης των λύσεων.

* [../datasets/car-f-92(3.71).stu](/datasets/car-f-92(3.71).stu): Ενδεικτικά είναι ένα αρχείο με δεδομένα προβλήματος, κάθε γραμμή του προβλήματος αντιστοιχεί σε ένα φοιτητή, τα περιεχόμενα τις κάθε γραμμής αντιστοιχούν στους κωδικούς των μαθημάτων που ο φοιτητής είναι εγγεγραμμένος.

## 5 Οδηγίες εγκατάστασης
Η εφαρμογή έχει γραφεί σε γλώσσα προγραμματισμού c++. Τα δεδομένα και ο κώδικας είναι σε δυο φακέλους , ο ένας φάκελος “datasets” περιέχει τα αρχεία δεδομένων των προβλημάτων και ο άλλος “src2” περιέχει τα αρχεία κώδικα και το εκτελέσιμο της εφαρμογής. Αφού ανοιχτούν τα αρχεία κώδικα, με επέκταση .cpp, μπορούμε να δούμε τον κώδικα. Για την μεταγλώττιση θα πρέπει να εγκαταστήσουμε τον compiler της c++, μπορούμε να τον κατεβάσουμε δωρεάν από το link https://sourceforge.net/projects/mingw/. Για την μεταγλώττιση της εφαρμογής θα τρέχουμε την εντολή

g++ -o start start.cpp

Η εντολή της μεταγλώττισης θα παράξει το εκτελέσιμο αρχείο start.exe


## 6 Οδηγίες εκτέλεσης

Για να τρέξουμε την εφαρμογή θα πάμε στο φάκελο “src2” και με διπλό κλικ στο αρχείο “start.exe” η εφαρμογή θα ανοίξει σε περιβάλλον command mode. Επίσης, μπορούμε να εκκινήσουμε την εφαρμογή αν  σε  command mode γράψουμε start.exe και πατήσουμε enter . Στο φάκελο που είναι το εκτελέσιμο αρχείο της εφαρμογής θα πρέπει να βρίσκεται και το αρχείο  “filenames.txt”, στο αρχείο αυτό βρίσκονται τα ονόματα των αρχείων με τα δεδομένα των εγγραφών των φοιτητών. Σε ένα επίπεδο φακέλων πίσω πρέπει να βρίσκεται ο φάκελος με τα δεδομένα “datasets”. Με την εκτέλεση της εφαρμογής παράγεται ένα αρχείο με επέκταση ".msol" που έχει λύση του κάθε προβλήματος.


  