---
author-meta:
- Charles Tapley Hoyt
bibliography:
- content/manual-references.json
date-meta: '2020-06-07'
header-includes: '<!--

  Manubot generated metadata rendered from header-includes-template.html.

  Suggest improvements at https://github.com/manubot/manubot/blob/master/manubot/process/header-includes-template.html

  -->

  <meta name="dc.format" content="text/html" />

  <meta name="dc.title" content="Extension of Roles in the ChEBI Ontology" />

  <meta name="citation_title" content="Extension of Roles in the ChEBI Ontology" />

  <meta property="og:title" content="Extension of Roles in the ChEBI Ontology" />

  <meta property="twitter:title" content="Extension of Roles in the ChEBI Ontology" />

  <meta name="dc.date" content="2020-06-07" />

  <meta name="citation_publication_date" content="2020-06-07" />

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

  <link rel="alternate" type="text/html" href="https://chemical-roles.github.io/manuscript/v/1384990ea0c087343f8f7f5f549f69bf49076112/" />

  <meta name="manubot_html_url_versioned" content="https://chemical-roles.github.io/manuscript/v/1384990ea0c087343f8f7f5f549f69bf49076112/" />

  <meta name="manubot_pdf_url_versioned" content="https://chemical-roles.github.io/manuscript/v/1384990ea0c087343f8f7f5f549f69bf49076112/manuscript.pdf" />

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
([permalink](https://chemical-roles.github.io/manuscript/v/1384990ea0c087343f8f7f5f549f69bf49076112/))
was automatically generated
from [chemical-roles/manuscript@1384990](https://github.com/chemical-roles/manuscript/tree/1384990ea0c087343f8f7f5f549f69bf49076112)
on June 7, 2020.
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

The Chemical Entities of Biological Interest (ChEBI) [@pmid:23180789; @pmid:26467479] ontology models chemicals, their classes,
their roles, and their interrelations (Figure {@fig:overview}, left). While many roles correspond to how their
substituent chemicals affect proteins, protein families, protein complexes, pathways, pathologies, or organisms, this
information is unstructured. Yan *et al.* previously described how these correspondences could be theoretically
formalized [@raw:ying2011]. This article proposes a concrete schema and axioms through which these roles can be linked to their target
entities (Figure {@fig:overview}, right), a suite of open source, reusable curation tools, and ultimately a manually
curated database of relationships between chemical roles and their targets. 

![Schema for inference of chemicals' relations to targets via roles.
Targets may be other chemicals, proteins, protein families, protein
complexes, pathways, pathologies, or organisms.](images/overview.svg){#fig:overview}

Throughout this article, the term role (in the context of the ChEBI ontology) will be used in the colloquial sense
described by Batchelor *et al.* [@isbn:9781607505341] rather than the formal sense prescribed by the
Basic Formal Ontology [@doi:10.3233/AO-160164; @arxiv:1502.04108].


## Extension of the ChEBI Schema

Before generalizing the rules for the relationships between targets, it is best to examine a specific example. Chemicals that have the role *p53 activator* [@url:https://identifiers.org/CHEBI:77731] obviously affect a certain target. The type of effect is directly activates [@url:http://purl.obolibrary.org/obo/RO_0002406]. The type of the target is protein. The target itself is the protein encoded by the *TP53* [@url:https://identifiers.org/hgnc:11998] gene. Because the chemical CBL0137 [@url:https://identifiers.org/CHEBI:138650] has the role *p53 activator*, it can be inferred that *CBL0137 directly activates TP53*. 

While Yan *et al.* exemplified the formalization of the relationship between roles from the ChEBI ontology and their targets using the Manchester syntax, this article will only informally describe axioms. It is intended that these descriptions are easily understandable such that the focus can remain on the practical utility of the relations curated and inferred during the work described here. The following informal amalgamation of a shape expression (common to graph query languages like SPARQL) and propositional logic outlines how to infer if a chemical C is an activator of protein P given it has the role R and role R is related to the activation of protein P.


## References {.page_break_before}

<!-- Explicitly insert bibliography here -->
<div id="refs"></div>
