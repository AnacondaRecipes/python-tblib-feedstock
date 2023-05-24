# About python-tblib
===========================

**Feedstock license:** [BSD-3-Clause](https://github.com/AnacondaRecipes/python-tblib/blob/main/LICENSE)

**Home:** https://github.com/hoodmane/python-tblib/

**Package license:** BSD 2-Clause

**Summary:** Serialization library for Exceptions and Tracebacks.
  
**Description:** It allows you to:
* Pickle tracebacks and raise exceptions with pickled tracebacks in different processes. This allows better error handling when running code over multiple processes (imagine multiprocessing, billiard, futures, celery etc).
* Create traceback objects from strings (the from_string method). No pickling is used.
* Serialize tracebacks to/from plain dicts (the from_dict and to_dict methods). No pickling is used.
* Raise the tracebacks created from the aforementioned sources.
* Pickle an Exception together with its traceback and exception chain (raise ... from ...) (Python 3 only)
Again, note that using the pickle support is completely optional. You are solely responsible for security problems should you decide to use the pickle support.

Installing python-tblib
================

`python-tblib` can be installed with:

```
conda install python-tblib
```

Terminology
===========

**feedstock** - the conda recipe (raw material), supporting scripts and CI configuration.

**conda-smithy** - the tool which helps orchestrate the feedstock.
                   Its primary use is in the construction of the CI ``.yml`` files
                   and simplify the management of *many* feedstocks.

**conda-forge** - the place where the feedstock and smithy live and work to
                  produce the finished article (built conda distributions)


Updating python-tblib-feedstock
========================

If you would like to improve the python-tblib recipe or build a new
package version, please fork this repository and submit a PR. Upon submission,
your changes will be run on the appropriate platforms to give the reviewer an
opportunity to confirm that the changes result in a successful build.

In order to produce a uniquely identifiable distribution:
 * If the version of a package **is not** being increased, please add or increase
   the [``build/number``](https://docs.conda.io/projects/conda-build/en/latest/resources/define-metadata.html#build-number-and-string).
 * If the version of a package **is** being increased, please remember to return
   the [``build/number``](https://docs.conda.io/projects/conda-build/en/latest/resources/define-metadata.html#build-number-and-string)
   back to 0.

Feedstock Maintainers
=====================

* [@katietz](https://github.com/katietz/)
* [@Jrice1317](https://github.com/Jrice1317/)
