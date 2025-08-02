Mechanic 2 server
=================

A [website][Mechanic 2 website] built with [Jekyll] and [hosted on GitHub].

The Mechanic 2 website works as a central server with metadata about individual extensions, each in its own repository.

Extension metadata is stored inside the `_data` folder as single `.yml` files.

Extensions are published by adding new files to this folder.

[Mechanic 2 website]: http://robofontmechanic.com/
[Jekyll]: http://jekyllrb.com/
[hosted on GitHub]: http://pages.github.com/
[YAML]: http://yaml.org/


Extension metadata
------------------

Extension metadata is written in [YAML] syntax and follows the [Extension Item Format]:

```yaml
extensionName: <name of the extension>
repository: <URL of the repository>
extensionPath: <path to the extension relative to the repository>
description: <description>
icon: <URL to a png file, optional>
developer: <name of the developer>
developerURL: <url of the developer>
tags:
  - <a tag>
  - <a tag>
  - <a tag>
dateAdded: YYYY-MM-DD HH:MM:SS
```

- Use existing tags whenever possible – see the [Mechanic 2 website] for the full list.
- See the [Boilerplate Extension] for examples of the different URL schemes used by GitHub, GitLab and BitBucket.


[Extension Item Format]: https://robofont.com/documentation/reference/extensions/extension-item-format/
[Boilerplate Extension]: http://github.com/robodocs/rf-extension-boilerplate


Testing extensions
------------------

It is recommended to test your extension metadata locally before submitting it to the Mechanic 2 server.

1. Save the metadata file with a `.mechanic` extension.
2. Install the extension in Mechanic 2 using *Settings > Single extension item*.


Adding extensions
-----------------

When everything is ready, follow the steps below to submit your extension to the Mechanic 2 server:

1. Fork this repository.
2. Add a `<extensionName>.yml` file to the `_data` folder.
3. Make a pull request and wait until one of the admins reviews and approves it.
