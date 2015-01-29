# Download Service feed provides a title for each entry

**Purpose**: 

The title element of an entry shall be populated with a human readable title for that entry.

**Test method**

* For each [entry](#entry) in the Download Service Feed, check if an [entry title](#entrytitle) is provided. 
* the [entry title](#entrytitle) must be non-empty text; the text content must include at least one alpha-numeric letter.

**Reference(s)**: 

* TG, Req 18

**Test type**: 

Automated

**Notes**

## Contextual XPath references

The namespace prefixes used as described in [README.md](README.md#namespaces).

Abbreviation                                               |  XPath expression
---------------------------------------------------------- | -------------------------------------------------------------------------
entry <a name="entry"></a> | //atom:entry
entry title <a name="entrytitle"></a> | //atom:entry/atom:title