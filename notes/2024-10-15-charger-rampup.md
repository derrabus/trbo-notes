# 2024-10-25 Charger Codebase

* Production system is an ancient Hetzner root server with PHP 5.6
    * Afraid of upgrading the host OS
    * Apparently no ops/admin maintaining the server regularly
    * Devs work on PHP 8.1 locally, possibly with a different set of dependencies

* MySQL 5.7 is used
    * Upgrade blocker: Usage of `PASSWORD()` function

* Plans to migrate to GCP are stalling
    * "No one gave us the ticket for that yet"

* Framework: Self-invented based on Slim/Pimple/Twig
    * Heavily inspired by ZF

* No CI for PHP
    * No tests
    * No static code analysis
    * No enforced code-style

* A lot of dead code
    * Code is commented out instead of removed
    * A lot of code that will break when executed, du to missing imports of global classes

* Implicitly declared properties make it hard to navigate through the codebase.

* The whole project resides in document root

* Frontend is being migrated from Angular to React

* Security Issues
    * API keys are MD5 hashes derived from Shop ID and Client ID
    * API Keys cannot be changed or regenerated
    * Passwords are hashed with MySQL's deprecated `PASSWORD()` function