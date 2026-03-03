---
type: source
source_type: paper
title: "{{title}}"
authors: [{% for creator in creators %}{{creator.firstName}} {{creator.lastName}}{% if not loop.last %}, {% endif %}{% endfor %}]
year: {{date | format("YYYY")}}
citekey: {{citekey}}
doi: {% if DOI %}{{DOI}}{% endif %}
zotero: "{{desktopURI}}"
created: {{importDate | format("YYYY-MM-DD")}}
tags: [paper{% for t in tags %}, {{t.tag}}{% endfor %}]
---

# {{title}}

**{% for creator in creators %}{{creator.firstName}} {{creator.lastName}}{% if not loop.last %}, {% endif %}{% endfor %}** ({{date | format("YYYY")}})

{% if abstractNote %}
## Abstract
> {{abstractNote}}
{% endif %}

## Key Claims
-

{% persist "annotations" %}
## Annotations
{% for annotation in annotations %}
{% if annotation.annotatedText %}
> {{annotation.annotatedText}} [(p. {{annotation.page}})]({{annotation.attachment.desktopURI}})
{% endif %}{% if annotation.comment %}
**Comment:** {{annotation.comment}}
{% endif %}

{% endfor %}
{% endpersist %}

{% persist "notes" %}
## My Thoughts

{% endpersist %}

## Links
-
