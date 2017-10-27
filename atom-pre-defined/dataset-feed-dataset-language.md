# Language for download link

**Purpose**: Where alternative language representations of datasets are linked to, the \" [hreflang attribute](#hreflang) \" attribute of the [link](#downloadlink) element must be used to indicate the language of the target dataset as described in the Atom specification.

**Prerequisites**

**Test method**

* if an [entry](#entry) has more than 1 download [link](#downloadlink), test that each of these download links provides the [hreflang attribute](#hreflang)

**Reference(s)**:

* [TG DL](http://inspire.ec.europa.eu/id/ats/download-service/3.1/atom-pre-defined/README#ref_TG_DL), Requirements 31, 38
* [Atom](http://inspire.ec.europa.eu/id/ats/download-service/3.1/atom-pre-defined/README#ref_atom)

**Test type**: Automated

**Notes**

## Contextual XPath references

The namespace prefixes used as described in [README.md](http://inspire.ec.europa.eu/id/ats/download-service/3.1/atom-pre-defined/README#namespaces).

Abbreviation                                               |  XPath expression
---------------------------------------------------------- | -------------------------------------------------------------------------
entry <a name="entry"></a> | //atom:entry/
link <a name="downloadlink"></a> | //atom:entry/atom:link[(@rel='alternate' and @type!='application/atom+xml') or (@rel='section')]
hreflang <a name="hreflang"></a> | //atom:link[@rel=('alternate','section')]/@hreflang
