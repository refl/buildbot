Release Notes for Buildbot |version|
====================================

..
    Any change that adds a feature or fixes a bug should have an entry here.
    Most simply need an additional bulleted list item, but more significant
    changes can be given a subsection of their own.

The following are the release notes for Buildbot |version|.

Master
------

Features
~~~~~~~~

* A new :py:class:`FlattenList` Renderable has been added which can flatten nested lists.

* Builder configurations can now include a ``description``, which will appear in the web UI to help humans figure out what the builder does.

* The web UI now supports a PNG Status Resource that can be accessed publicly from for example README.md files or wikis or whatever other resource.
  This view produces an image in PNG format with information about the last build for the given builder name or whatever other build number if is passed as an argument to the view.

* The web hooks now include support for Bitbucket.

* The 'Rebuild' button on the web pages for builds features a dropdown to choose whether to 
  rebuild from exact revisions or from the same sourcestamps (ie, update branch references)

* The ``start``, ``restart``, and ``reconfig`` commands will now wait for longer than 10 seconds as long as the master continues producing log lines indicating that the configuration is progressing.

* Git source checkout step now supports reference repositories.

Deprecations, Removals, and Non-Compatible Changes
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Changes for Developers
~~~~~~~~~~~~~~~~~~~~~~

Slave
-----

Features
~~~~~~~~

Deprecations, Removals, and Non-Compatible Changes
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Details
-------

For a more detailed description of the changes made in this version, see the
git log itself::

   git log v0.8.8..master

Older Versions
--------------

Release notes for older versions of Buildbot are available in the :bb:src:`master/docs/relnotes/` directory of the source tree.
Newer versions are also available here:

.. toctree::
    :maxdepth: 1

    0.8.8
    0.8.7
    0.8.6
