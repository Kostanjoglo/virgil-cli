NAME
====

**card-search-private** -- search for a Private Virgil Card\[s\] from
the Virgil Keys Service

SYNOPSIS
========

        virgil card-search-private  [-o <arg>] -d <arg> -t <arg> [-u] [-V] [--]
                            [--version] [-h]

DESCRIPTION
===========

Search for a Private Virgil Card from the Virgil Keys Service

OPTIONS
=======

        -o <arg>,  --out <arg>
         Folder in which will be saved a Virgil Cards

        -d <arg>,  --identity <arg>
         (required)  Identity value

        -t <arg>,  --identity-type <arg>
         (required)  Identity type

        -u,  --unconfirmed
         Search Cards include unconfirmed identity

        -V,  --VERBOSE
         Show detailed information

        --,  --ignore_rest
         Ignores the rest of the labeled arguments following this flag.

        --version
         Displays version information and exits.

        -h,  --help
         Displays usage information and exits.

EXAMPLES
========

1.  Search for Private Virgil Cards with a confirmed Identity:

        virgil card-search-private -d alice@gmail.com -t email -o alice/

2.  Search for Cards with a confirmed Identity and
    uncorfirmaed Identity.

        virgil card-search-private -d alice@gmail.com -t email -o alice-with-unconfirmed-identity/ -u

SEE ALSO
========

virgil(1)  
card-create-private(1)  
card-get(1)