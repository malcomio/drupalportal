## Release Notes

### v0.3.2 (2015-07-08)

* Unresolved references leave the original reference in the document so as not to break JSON Schema validation

### v0.3.1 (2015-07-08)

* Errors resolving remote references no longer bubble up errors and instead show up in metadata as unresolved

### v0.3.0 (2015-07-08)

* Fix issue with Bower build as it had old dependency paths in it *(PR #15)*
* Fix issue with circular references not being detected in arrays *(Issue #20)*
* Fix problem with references at the root of the document and having hashes *(Issue #19)*
* Support relative references *(Issue 11)*
* Support to specify a depth for `#resolveRefs` for circular references *(Issue #5)*

### v0.2.0 (2015-05-12)

* Replace file loading with [path-loader](https://github.com/whitlockjc/path-loader)

### v0.1.10 (2015-04-16)

* Fixed an issue due to difference in superagent in browser vs. Node.js

### v0.1.9 (2015-04-16)

* Fixed a browser build issue

### v0.1.8 (2015-04-16)

* Updated `isRemotePointer` to only return `true` for explicit URLs or relative paths

### v0.1.7 (2015-04-16)

* Added support in `resolveRefs` to alter a remote request prior to sending the request _(Useful for authentication)_
_(Issue #12)_
* Added support in `resolveRefs` to process the remote request responses
* Fixed bug in `resolveRefs` where multiple remote references resulted in callback being called multiple times
* Updated `isRemotePointer` to handle relative references and file URL references _(Issue #9)_
* Updated `resolveRefs` to return resolution metadata _(What references were resolved, where they were located and what
they resolved to)_
