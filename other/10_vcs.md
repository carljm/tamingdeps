<!SLIDE small nobullets>

# but what about VCS support?!? #

* `-e git://github.com/carljm/django-model-utils@8c6c1cf8#egg=django-model-utils`

<!SLIDE>

## it's excellent ##

<!SLIDE incremental>

    @@@ comment
    - testing if the tip version fixes a bug, developing a reusable app...

## use it in development ##

<!SLIDE incremental>

    @@@ comment
    - anytime you have to install something new on your server just to support
      your deployment process, you might be doing something wrong

## not for production deploys ##

* more moving parts in every deploy
* have to install VCSes on every server
* VCS clones / checkouts are slow
* every VCS host is another point of failure
* internal releases are easy to make (`setup.py sdist`)
