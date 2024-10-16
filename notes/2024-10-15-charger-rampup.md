# 2024-10-26 Charger Codebase

* Production system is an ancient Hetzner root server with PHP 5.6
    * Afraid of upgrading the host OS
    * Apparently no ops/admin maintaining the server regularly
    * Devs work on PHP 8.1 locally, possibly with a different set of dependencies

* Plans to migrate to GCP are stalling
    * "No one gave us the ticket for that yet"

* Framework: Self-invented based on Slim/Pimple/Twig

* No tests

* No static code analysis