About r-waterml
===============

Home: https://github.com/jirikadlec2/waterml

Package license: MIT

Feedstock license: BSD 3-Clause

Summary: Lets you connect to any of the Consortium of Universities for the Advancement of Hydrologic Sciences, Inc. ('CUAHSI') Water Data Center 'WaterOneFlow' web services and read any 'WaterML' hydrological time series data file. To see list of available web services, see <http://hiscentral.cuahsi.org>. All versions of 'WaterML' (1.0, 1.1 and 2.0) and both types of the web service protocol ('SOAP' and 'REST') are supported. The package has six data download functions: GetServices(): show all public web services from the HIS Central Catalog. HISCentral_GetSites() and HISCentral_GetSeriesCatalog(): search for sites or time series from the HIS Central catalog based on geographic bounding box, server, or keyword. GetVariables(): Show a data.frame with all variables on the server. GetSites(): Show a data.frame with all sites on the server. GetSiteInfo(): Show what variables, methods and quality control levels are available at the specific site. GetValues(): Given a site code, variable code, start time and end time, fetch a data.frame of all the observation time series data values. The GetValues() function can also parse 'WaterML' data from a custom URL or from a local file. The package also has five data upload functions: AddSites(), AddVariables(), AddMethods(), AddSources(), and AddValues(). These functions can be used for uploading data to a 'HydroServer Lite' Observations Data Model ('ODM') database via the 'JSON' data upload web service interface.



Current build status
====================


<table><tr><td>All platforms:</td>
    <td>
      <a href="https://dev.azure.com/conda-forge/feedstock-builds/_build/latest?definitionId=1787&branchName=master">
        <img src="https://dev.azure.com/conda-forge/feedstock-builds/_apis/build/status/r-waterml-feedstock?branchName=master">
      </a>
    </td>
  </tr>
</table>

Current release info
====================

| Name | Downloads | Version | Platforms |
| --- | --- | --- | --- |
| [![Conda Recipe](https://img.shields.io/badge/recipe-r--waterml-green.svg)](https://anaconda.org/conda-forge/r-waterml) | [![Conda Downloads](https://img.shields.io/conda/dn/conda-forge/r-waterml.svg)](https://anaconda.org/conda-forge/r-waterml) | [![Conda Version](https://img.shields.io/conda/vn/conda-forge/r-waterml.svg)](https://anaconda.org/conda-forge/r-waterml) | [![Conda Platforms](https://img.shields.io/conda/pn/conda-forge/r-waterml.svg)](https://anaconda.org/conda-forge/r-waterml) |

Installing r-waterml
====================

Installing `r-waterml` from the `conda-forge` channel can be achieved by adding `conda-forge` to your channels with:

```
conda config --add channels conda-forge
```

Once the `conda-forge` channel has been enabled, `r-waterml` can be installed with:

```
conda install r-waterml
```

It is possible to list all of the versions of `r-waterml` available on your platform with:

```
conda search r-waterml --channel conda-forge
```


About conda-forge
=================

[![Powered by NumFOCUS](https://img.shields.io/badge/powered%20by-NumFOCUS-orange.svg?style=flat&colorA=E1523D&colorB=007D8A)](http://numfocus.org)

conda-forge is a community-led conda channel of installable packages.
In order to provide high-quality builds, the process has been automated into the
conda-forge GitHub organization. The conda-forge organization contains one repository
for each of the installable packages. Such a repository is known as a *feedstock*.

A feedstock is made up of a conda recipe (the instructions on what and how to build
the package) and the necessary configurations for automatic building using freely
available continuous integration services. Thanks to the awesome service provided by
[CircleCI](https://circleci.com/), [AppVeyor](https://www.appveyor.com/)
and [TravisCI](https://travis-ci.com/) it is possible to build and upload installable
packages to the [conda-forge](https://anaconda.org/conda-forge)
[Anaconda-Cloud](https://anaconda.org/) channel for Linux, Windows and OSX respectively.

To manage the continuous integration and simplify feedstock maintenance
[conda-smithy](https://github.com/conda-forge/conda-smithy) has been developed.
Using the ``conda-forge.yml`` within this repository, it is possible to re-render all of
this feedstock's supporting files (e.g. the CI configuration files) with ``conda smithy rerender``.

For more information please check the [conda-forge documentation](https://conda-forge.org/docs/).

Terminology
===========

**feedstock** - the conda recipe (raw material), supporting scripts and CI configuration.

**conda-smithy** - the tool which helps orchestrate the feedstock.
                   Its primary use is in the construction of the CI ``.yml`` files
                   and simplify the management of *many* feedstocks.

**conda-forge** - the place where the feedstock and smithy live and work to
                  produce the finished article (built conda distributions)


Updating r-waterml-feedstock
============================

If you would like to improve the r-waterml recipe or build a new
package version, please fork this repository and submit a PR. Upon submission,
your changes will be run on the appropriate platforms to give the reviewer an
opportunity to confirm that the changes result in a successful build. Once
merged, the recipe will be re-built and uploaded automatically to the
`conda-forge` channel, whereupon the built conda packages will be available for
everybody to install and use from the `conda-forge` channel.
Note that all branches in the conda-forge/r-waterml-feedstock are
immediately built and any created packages are uploaded, so PRs should be based
on branches in forks and branches in the main repository should only be used to
build distinct package versions.

In order to produce a uniquely identifiable distribution:
 * If the version of a package **is not** being increased, please add or increase
   the [``build/number``](https://conda.io/docs/user-guide/tasks/build-packages/define-metadata.html#build-number-and-string).
 * If the version of a package **is** being increased, please remember to return
   the [``build/number``](https://conda.io/docs/user-guide/tasks/build-packages/define-metadata.html#build-number-and-string)
   back to 0.

Feedstock Maintainers
=====================

* [@bgruening](https://github.com/bgruening/)
* [@cbrueffer](https://github.com/cbrueffer/)
* [@conda-forge/r](https://github.com/conda-forge/r/)
* [@daler](https://github.com/daler/)
* [@dbast](https://github.com/dbast/)
* [@jdblischak](https://github.com/jdblischak/)
* [@johanneskoester](https://github.com/johanneskoester/)
* [@ocefpaf](https://github.com/ocefpaf/)

