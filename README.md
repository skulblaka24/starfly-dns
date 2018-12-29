DNS
===

Ce role configure les bons dns sur la machine.

Requirements
------------

Le premier dns doit pointer sur la freebox qui pointe elle sur le dns interne du reseau.
Normalement ce dns porte un forwarder mais au cas où, on peut rajouter le dns de google.

Platform
--------

Debian ou RHEL

Role Variables
--------------

<pre><code>dns_search: "search starfly.ovh"
dns_nameserver:
  - "nameserver 192.168.1.254"
  - "nameserver 8.8.8.8"
</code></pre>

Dependencies
------------

Préconfiguration dns sur la freebox et dans l'environnement.

Ce role se télécharge automatiquement à partir du requirements.yml


Author Information
------------------

Starfly Env Team
