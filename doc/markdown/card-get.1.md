NAME
====

**card-get** -- return Card(s)

SYNOPSIS
========

**virgil card-get** \[-o *arg*\] -a *arg* \[-e *arg*\] \[-k *file*\]
\[--\] \[--version\] \[-h\]

DESCRIPTION
===========

Return a Card by card-id or a group of Cards connected with
public-key-id

OPTIONS
=======

    -o *arg*,  --out *arg*
     Folder where Virgil Cards will be saved

    -a *arg*,  --card-id *arg*
     (required)  Virgil Card identifier

    -e *arg*,  --public-key-id *arg*
     Public Key identifier


    -k *file*,  --key *file*
     Private key

    --,  --ignore_rest
     Ignores the rest of the labeled arguments following this flag

    --version
     Displays version information and exits

    -h,  --help
     Displays usage information and exits

EXAMPLES
========

1.  Return a Card by card-id:

        virgil card-get -a *card_id*

2.  Return a group of Cards connected with public-key-id, card-id
    belongs to one of the Cards:

        virgil card-get -a *card_id* -e *public_key_id* -k private.key

SEE ALSO
========

[`virgil(1)`](../markdown/virgil.1.md),  
[`card-create(1)`](../markdown/card-create.1.md),  
[`card-search(1)`](../markdown/card-search.1.md),  
[`card-search-app(1)`](../markdown/card-search-app.1.md)