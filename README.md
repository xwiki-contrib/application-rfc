# RFC Application

> "A Request for Comments (RFC) is a publication of the Internet Engineering Task Force (IETF) and the Internet Society, the principal technical development and standards-setting bodies for the Internet" ([Wikipedia](https://en.wikipedia.org/wiki/Request_for_Comments))

This application provides a way for authoring documents that share some common traits with IETF's RFC. These documents can be used to describe different aspects inside an organization. An RFC has a category (informational, experimental or best current practice), a status (draft or final), an abstract and a content, and can obsolete another RFC (which is then shown as superseded).

* Project Lead: Clément Christiaens
* Original author: [Fabio Mancinelli](https://www.xwiki.org/xwiki/bin/view/XWiki/fmancinelli)
* [Documentation & Downloads](https://extensions.xwiki.org/xwiki/bin/view/Extension/RFC%20Application)
* [Issue Tracker (TODO)](https://jira.xwiki.org/browse/RFC)
* Communication (TODO): [Forum](https://forum.xwiki.org/), [Chat](https://dev.xwiki.org/xwiki/bin/view/Community/Chat)
* [Development Practices](https://dev.xwiki.org)
* Minimal XWiki version supported: XWiki 17.10.0
* License: LGPL 2.1
* Translations: N/A
* Continuous Integration Status (TODO): [![Build Status](https://ci.xwiki.org/job/XWiki%20Contrib/job/application-rfc/job/master/badge/icon)](https://ci.xwiki.org/job/XWiki%20Contrib/job/application-rfc/job/master/)

## Security note

RFC pages enforce XWiki's required rights: script macros in the content or the title of an RFC run only if an administrator declares the corresponding required right on that page. Pages created from the RFC template inherit this setting, and the migration page applies it to the pages it converts from version 1.x.

## Building

```
mvn clean install
```

The wiki pages live in `application-rfc-ui/src/main/resources`. After editing one of them, normalize it with:

```
mvn xar:format -pl application-rfc-ui
```
