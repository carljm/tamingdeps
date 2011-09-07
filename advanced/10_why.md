<!SLIDE incremental nobullets>

## sure, PyPI mirrors are nice ##

* but
* `Some Project` host their own downloads
* and now their site's down and I can't deploy

<!SLIDE incremental>

    @@@ comment
    Ultimately, you've got to control your own dependency source if you want
    reliable deployments. I'll go over three ways pip can help you do that.

## if you want it done right, do it yourself ##

* 1. `--index-url`
* 2. `--find-links`
* 3. `vendor/`
