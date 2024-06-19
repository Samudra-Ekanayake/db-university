Selezionare tutti gli studenti nati nel 1990 (160)
SELECT * FROM `students` WHERE YEAR (date_of_birth) = 1990;  risultato = 160


Selezionare tutti i corsi che valgono più di 10 crediti (479)
SELECT * FROM `courses` WHERE `cfu` > 10; risultato = 479


Selezionare tutti gli studenti che ad OGGI hanno almeno 30 anni compiuti (3725)
SELECT * FROM students WHERE date_of_birth <= DATE_SUB(CURDATE(), INTERVAL 30 YEAR); risultato = 3725


Selezionare tutti i corsi del primo semestre del primo anno di un qualsiasi corso di laurea (286)
SELECT * FROM `courses` WHERE `period` = `I semestre`  AND `year`= 1; risultato = non funziona


Da quanti dipartimenti è composta l'università? (12)
SELECT * FROM `departments` WHERE `id`; risultato = 12


Quanti sono gli insegnanti che non hanno un numero di telefono? (50)
SELECT * FROM `teachers` WHERE `phone` IS NULL; risultato = 50





Selezionare tutti gli appelli d'esame che avvengono nel pomeriggio (dopo le 14) del 20/06/2020 (21)
Selezionare tutti i corsi di laurea magistrale (38)
Inserire nella tabella degli studenti un nuovo record con i propri dati (per il campo degree_id, inserire un valore casuale)
Cambiare il numero dell’ufficio del professor Pietro Rizzo in 126
Eliminare dalla tabella studenti il record creato precedentemente al punto 9

