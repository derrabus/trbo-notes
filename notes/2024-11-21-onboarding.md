# Onboarding Layer-Editor 2.0

* Kunde bindet Plugin-Code ein
    * Bootstrapping-Code
    * Uralt-jQuery
    * Cache des Codes auf GCP-Bucket (30min.) als CDN

* `r.php`
    * „Die API“
    * „Wurst-Code“

* Data-Layer:
    * Key/Value-Daten, die der Kunde für Regeln verwenden kann.

* Plugin-Code zieht alle Layer, die eingebunden werden sollen
    * Viele Duplikate
    * Hohe AUsführungszeit wegen entpacken/eval von JS

* Aktuell: Jeder Layer === ein use-case
    * Sammlung von Workarounds
    * HTML-Layer zur Positionierung

* TODO: Layer Settings

* TODO: Close

* TODO: Tracking