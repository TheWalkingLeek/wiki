DelayedJobs sollen grosse Tasks von der restlichen Applikation in den Hintergrund abkapseln.

* Alle aktiven Jobs sind in der delayed_jobs Tabelle gespeichert
* Jobs sind eigene Instanzierungen einer jeweiligen Job Klasse
* Die Job Klasse benötigt eine perform Methode, diese wird dann ausgeführt
* Jobs können eine Prioritisierung besitzen
* Jobs benötigen eine run_at value 
* Jobs werden neu gestartet sollten sie failen
* Es gibt eine MAX_ATTEMPTS Variable (default 25)
* Es gibt eine MAX_RUN_TIME Variable (default 4.hours)
* Jobs werden nach failen (oder auch bei successfull jobs) gelöscht
* rake jobs:work beginnt, alle Jobs abzuarbeiten
* rake jobs:clear löscht alle Jobs in der Queue

https://github.com/tobi/delayed_job