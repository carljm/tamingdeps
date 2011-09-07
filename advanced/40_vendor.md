<!SLIDE>

# option 3 #

<!SLIDE incremental>

## commit deps (unpacked) in a vendor/ directory ##

* ``pip install --install-option="--home=`pwd`/vendor/" ...``
* ``export PYTHONPATH=`pwd`/vendor/lib/python``
* commit `vendor/` with the rest of your code

<!SLIDE commandline incremental>

    $ tree -L 4
    .
    `-- vendor
        |-- bin
        |   `-- django-admin.py
        `-- lib
            `-- python
                |-- django
                |-- Django-1.3-py2.6.egg-info
                |-- django_floppyforms-0.4.7-py2.6.egg-info
                `-- floppyforms

<!SLIDE incremental>

## vendor/ ##

* fastest, simplest deployment story (no moving parts)
* platform/path issues with compiled extensions
* requires path hackery (PYTHONPATH or runtime sys.path mods)
* temptation to patch stuff directly in `vendor/`
