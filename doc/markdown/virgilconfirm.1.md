NAME
====

**confirm** -- send confirmation code to the Virgil Public Keys service.

SYNOPSIS
========

**virgil confirm** --user-id *arg* --code *arg*

DESCRIPTION
===========

Send confirmation code to the Virgil Public Keys service. Confirmation
code is sent to the user's identifier (email, phone, etc) after public
key registration.

OPTIONS
=======

-i *arg*, --user-id *arg*  
(required) User's identifer. Format:

    [email|phone|domain]:<value>

where:

-   if `email`, then *value* - user's email;
-   if `phone`, then *value* - user's phone;
-   if `domain`, then *value* - user's domain.

-c *arg*, --code *arg*  
(required) Confirmation code.

SEE ALSO
========

`virgil(1)`, `virgilkeyreg(1)`