<!SLIDE>

# option 1 #

<!SLIDE incremental>

## host your own index ##

* pip lets us replace the default PyPI index URL (or add more index URLs)
* directory per project, with links to sdists
* automate with `chishop` (or `EggBasket`, `ClueReleaseManager`, `basketweaver`...)
* can also accept `setup.py upload` like PyPI
* just use `--index-url` option with base URL
* or `--extra-index-url` if you want PyPI too
* can go in reqs file (applies to whole file)

<!SLIDE commandline incremental>

`--index-url http://myindex.example.com/`

    $ tree
    .
    |-- Django
    |   `-- Django-1.3.tar.gz
    `-- django-floppyforms
        `-- django-floppyforms-0.4.2.tar.gz

<!SLIDE incremental>

## your own index ##

* easy to upload internal packages with `setup.py upload`
* higher maintenance
* separate from project but needs to be kept in sync
