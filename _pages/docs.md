---
layout: default
---

# Documents

{% assign strategy_docs = site.documents | where:"type","strategy" | sort: "title" %}
## Annual strategy
{% for doc in strategy_docs %}
[{{ doc.title }}]({{ doc.url }})
{% endfor %}

{% assign corp_docs = site.documents | where:"type","corporate" | sort: "title" %}
## Corporate stuff
{% for doc in corp_docs %}
[{{ doc.title }}]({{ doc.url }})
{% endfor %}
