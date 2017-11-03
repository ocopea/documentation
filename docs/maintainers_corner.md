# Maintainers' Corner

---

**Managing Project and Tools**

Since maintainers are responsible for the acceptance of pull requests and other
tool-related operations, here are some guidelines that support consistency and
other requirements of this project.

## Tool Inventory

The Ocopea project makes use of these toolsets:

* [Github](maintainers_corner.md#github)
* [Bintray](maintainers_corner.md#bintray)
* [Docker Hub](maintainers_corner.md#docker-hub)
* [Travis CI](maintainers_corner.md#travis-ci)
* [ReadTheDocs](maintainers_corner.md#readthedocs)

## Github

Links to sections below

* [File modification](maintainers_corner.md#checklist-for-modifications-to-existing-files)
* [New file](maintainers_corner.md#checklist-for-new-files)
* [New repository](maintainers_corner.md#checklist-for-new-repository)

### Checklist for modifications to existing files

Pull Requests involving code modifications will be accepted after maintainers have ensured the following:

* Code (source and test) follows best practices outlined in [Ocopea Project Guidelines](guidelines.md)

### Checklist for new files

In addition to the above requirements, there are additional steps needed before a PR can be accepted.
Examples of new files could include, for example, source code or an Open Source (vendor) dependency.

#### New source code modules

Non-Dell EMC authors:

* See the Dell EMC {code} [Contributor Agreement](https://github.com/codedellemc/codedellemc.github.io/wiki/Contributor-Agreement).

Dell EMC authors:

* New files have the Dell EMC Copyright statement applied in a comment to the
top of the source code file(s).

    ```Copyright (c) 2017 Dell Inc. or its subsidiaries. All Rights Reserved.```

#### New vendor dependencies

These additions require some coordination across Ocopea repositories:

* Have been reviewed according to Dell Technologies formal process
[https://inside.dell.com/docs/DOC-106365](https://inside.dell.com/docs/DOC-106365)
* Maintainers will ensure the
[Third_party_license](https://github.com/ocopea/documentation/blob/master/Third_party_license)
file is updated to include copyright information for added dependencies

### Checklist for new repository

New repositories will likely have both new code and new dependencies.  The
above relevant sections apply.  In addition, maintainers will ensure projects have
the following before approving:

#### Files

* README.md
* LICENSE (points to [Ocopea LICENSE](https://github.com/ocopea/documentation/blob/master/LICENSE))
* OWNERS
* COPYRIGHT (points to [Ocopea COPYRIGHT](https://github.com/ocopea/documentation/blob/master/COPYRIGHT))

#### Settings

Compare to existing repositories (such as
[pcf-fs-crb](https://github.com/ocopea/pcf-fs-crb/settings)) for the full set
of github project settings.

Some of the changes from default include:

* Options
    * Enable "Allow rebase merging"
    * Others options are disabled
* Branches
    * Default branch is master
    * Protected branch includes master

## Bintray


## Docker Hub


## Travis CI


## ReadTheDocs

The documentation project has a webhook enabled for
[ReadTheDocs](http://ocopea-documentation.readthedocs.io/en/latest).  This
webhook initiates the rebuild of documentation there on every push to master.

The webhook is created from an authorized account on ReadTheDocs, which on
project import redirects to github sign-on to create a trusted link.  Authorized
members for ReadTheDocs project is managed on that site, and ReadTheDocs member
accounts can be added or removed.

The webhook can be viewed and managed from
[github](https://github.com/ocopea/documentation/settings/hooks/17174029),
including temporary or permanent deactivation.  The set of events that trigger
the webhook can be refined there as needed.

---

## Managing Memberships

When a Maintainer is added to a project, use the following checklist:

* Individual's account has 2FA enabled
* Set individual as owner of the project
* Update OWNERS file in the project to include the new individual

