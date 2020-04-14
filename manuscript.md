---
author-meta:
- Charles Tapley Hoyt
bibliography:
- content/manual-references.json
date-meta: '2020-04-14'
header-includes: '<!--

  Manubot generated metadata rendered from header-includes-template.html.

  Suggest improvements at https://github.com/manubot/manubot/blob/master/manubot/process/header-includes-template.html

  -->

  <meta name="dc.format" content="text/html" />

  <meta name="dc.title" content="Extension of Roles in the ChEBI Ontology" />

  <meta name="citation_title" content="Extension of Roles in the ChEBI Ontology" />

  <meta property="og:title" content="Extension of Roles in the ChEBI Ontology" />

  <meta property="twitter:title" content="Extension of Roles in the ChEBI Ontology" />

  <meta name="dc.date" content="2020-04-14" />

  <meta name="citation_publication_date" content="2020-04-14" />

  <meta name="dc.language" content="en-US" />

  <meta name="citation_language" content="en-US" />

  <meta name="dc.relation.ispartof" content="Manubot" />

  <meta name="dc.publisher" content="Manubot" />

  <meta name="citation_journal_title" content="Manubot" />

  <meta name="citation_technical_report_institution" content="Manubot" />

  <meta name="citation_author" content="Charles Tapley Hoyt" />

  <meta name="citation_author_orcid" content="0000-0003-4423-4370" />

  <meta name="twitter:creator" content="@cthoytp" />

  <link rel="canonical" href="https://chemical-roles.github.io/manuscript/" />

  <meta property="og:url" content="https://chemical-roles.github.io/manuscript/" />

  <meta property="twitter:url" content="https://chemical-roles.github.io/manuscript/" />

  <meta name="citation_fulltext_html_url" content="https://chemical-roles.github.io/manuscript/" />

  <meta name="citation_pdf_url" content="https://chemical-roles.github.io/manuscript/manuscript.pdf" />

  <link rel="alternate" type="application/pdf" href="https://chemical-roles.github.io/manuscript/manuscript.pdf" />

  <link rel="alternate" type="text/html" href="https://chemical-roles.github.io/manuscript/v/11cc1445a0f9427cd1d44522bc19e30ae65598f9/" />

  <meta name="manubot_html_url_versioned" content="https://chemical-roles.github.io/manuscript/v/11cc1445a0f9427cd1d44522bc19e30ae65598f9/" />

  <meta name="manubot_pdf_url_versioned" content="https://chemical-roles.github.io/manuscript/v/11cc1445a0f9427cd1d44522bc19e30ae65598f9/manuscript.pdf" />

  <meta property="og:type" content="article" />

  <meta property="twitter:card" content="summary_large_image" />

  <link rel="icon" type="image/png" sizes="192x192" href="https://manubot.org/favicon-192x192.png" />

  <link rel="mask-icon" href="https://manubot.org/safari-pinned-tab.svg" color="#ad1457" />

  <meta name="theme-color" content="#ad1457" />

  <!-- end Manubot generated metadata -->'
keywords:
- ChEBI
- Cheminformatics
- Ontologies
lang: en-US
manubot-clear-requests-cache: false
manubot-output-bibliography: output/references.json
manubot-output-citekeys: output/citations.tsv
manubot-requests-cache-path: ci/cache/requests-cache
title: Extension of Roles in the ChEBI Ontology
...






<small><em>
This manuscript
([permalink](https://chemical-roles.github.io/manuscript/v/11cc1445a0f9427cd1d44522bc19e30ae65598f9/))
was automatically generated
from [chemical-roles/manuscript@11cc144](https://github.com/chemical-roles/manuscript/tree/11cc1445a0f9427cd1d44522bc19e30ae65598f9)
on April 14, 2020.
</em></small>

## Authors



+ **Charles Tapley Hoyt**<br>
    ![ORCID icon](images/orcid.svg){.inline_icon}
    [0000-0003-4423-4370](https://orcid.org/0000-0003-4423-4370)
    · ![GitHub icon](images/github.svg){.inline_icon}
    [cthoyt](https://github.com/cthoyt)
    · ![Twitter icon](images/twitter.svg){.inline_icon}
    [cthoytp](https://twitter.com/cthoytp)<br>
  <small>
  </small>



## Motivation {.page_break_before}

The Chemical Entities of Biological Interest (ChEBI) [@pmid:23180789] ontology models chemicals, their classes,
their roles, and their interrelations ({@fig:overview}, left). While many roles correspond to how their substituent
chemicals affect proteins, protein families, protein complexes, pathways, pathologies, or organisms, this information is
unstructured. Yan et al. (2011) previously described how these correspondences could be theoretically formalized.
This article proposes a concrete schema and axioms through which these roles can be linked to their target entities
({@fig:overview}, right), a suite of open source, reusable curation tools, and ultimately a manually curated database of
relationships between chemical roles and their targets. 

![Schema for inference of chemicals' relations to targets via roles.
Targets may be other chemicals, proteins, protein families, protein
complexes, pathways, pathologies, or organisms.](images/overview.svg){#fig:overview}

Throughout this article, the term role (in the context of the ChEBI ontology) will be used in the colloquial sense
described by Batchelor *et al.* [@isbn:9781607505341] rather than the formal sense prescribed by the
Basic Formal Ontology [@isbn:9781607505341].


## References {.page_break_before}

<!-- Explicitly insert bibliography here -->
<div id="refs"></div>
