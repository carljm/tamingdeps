<!SLIDE>

## dependencies are painful ##

<!SLIDE>

## even Django hates them ##

    @@@ comment
    As evidence, I present this cute little obscenity.

<!SLIDE>

    @@@ python
    from django.utils import unittest

<!SLIDE>

## but you don't have to! ##

<!SLIDE incremental>

    @@@ comment
    libraries
        - harder, because less control over how and where used
        - might discuss at the end if I have time
    end-user programs
        - really really hard, less control and used by non-programmers
        - Django's situation, due to wanting easy ramp-up for beginners
        - not going to discuss; not pip's focus either

## scope ##

* a web project
* not a library
* not an end-user program

<!SLIDE incremental>

## deployment desiderata ##

    @@@ comment
    - not going to talk about all aspects of a deployment system, just
      dependency management. these might be obvious, but:
    - repeatable: if you haven't changed anything intentionally, deploying the
      same project twice should have exactly the same results
    - reliable: not reliant on servers outside your control that might be down,
      minimize moving parts that could break
    - fast: you want to be able to deploy often and casually and with minimum
      downtime; speed matters

* repeatable
* reliable
* fast
