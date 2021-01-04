How to use this doc
=====================

This doc is a template for [Nobs • Share Buttons documentation](https://sharebuttons.social/doc/).
It's split into several repository that work together:

* [The plugin repository](https://github.com/geoffreycrofte/juiz-social-post-sharer) where the JSDoc settings are, and also where the plugin files are scanned to generate the doc.
* [The documentation repository](https://github.com/geoffreycrofte/juiz-sps-plugin-documentation) with only HTML files in it, almost. I usually clone it directly into the /plugins folder next to the documented plugin itself. (because of npm related command, see below)
* [The doc template repository](https://github.com/geoffreycrofte/juiz-sps-plugin-template-doc) which is the structure being used by the tool to generate documentation.

## Things to know

* The hookdoc.json file handle the folder source and destination.
* The destination is outside the plugin folder for having a separate repository.
* The package.json set the command `del '../nobs-share-buttons-doc/**' '!../nobs-share-buttons-doc/.git' -f && jsdoc inc -c hookdoc.json` using the `del-cli` package to delete everything but the .git repository. (`npm install del-cli` to make it work)
