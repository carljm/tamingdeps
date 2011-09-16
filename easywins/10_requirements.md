<!SLIDE>

## the pip requirements file ##

    @@@
    Django==1.3

    South==0.7.3
    django-compressor==0.9.2
    BeautifulSoup==3.2.0
    slimmer==0.1.30
    django-floppyforms==0.4.2
    django-classy-tags==0.3.0
    ...

<!SLIDE incremental>

## habits for highly effective requirements files ##

* pin everything
* (even deps of deps)
* pin exactly
* `Django==1.2.5`, not `Django>=1.2,<1.3`
* test regularly in a clean venv

<!SLIDE incremental nobullets>

## how it works ##

* `Django==1.3`
* default "index url": `http://pypi.python.org/simple/`
* `http://pypi.python.org/simple/Django/1.3`
* `http://pypi.python.org/simple/Django/`
* link scraping, wheee!
* `rel=[homepage,download]` or links that look like PyPI home/download links
* archive files (zip/tar) named like `Django-1.3.tar.gz` - "sdists"
* picks highest found version that fits criterion
* use `pip install -vv ...` to debug
