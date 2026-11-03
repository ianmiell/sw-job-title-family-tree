# Software industry job title family tree

A Graphviz family tree of software industry job titles, from the 1940s
("Computer", "Coder", "Programmer") to the present (SRE, Platform Engineer,
Forward Deployed Engineer, AI Engineer).

**View it: https://ianmiell.github.io/sw-job-title-family-tree/** (zoomable; click a family,
or use the buttons, to show just that column, e.g. [Data & AI](https://ianmiell.github.io/sw-job-title-family-tree/#data))

![Family tree](job_title_family_tree.png)

- Time runs from top to bottom. Each title carries a date and sits in the row
  for its five-year period: roughly when the title became common, not its first recorded use. "c." means approximate;
  exact years are given where well known (e.g. SRE at Google, 2003; "DevOps"
  coined 2009; "Data Scientist" 2008). They are best estimates, not sourced
  citations, so corrections are welcome.
- Solid arrow: the title grew out of its parent. Dashed arrow: influence or a
  common career move.
- Titles sit in coloured columns by family: development; analysis, architecture
  and leadership; operations and infrastructure; networks and security;
  data and AI; quality and test; support and customer-facing. Arrows take
  the colour of the family they lead into, and landmark titles are bold.

## Rendering

```sh
dot -Tsvg job_title_family_tree.dot -o job_title_family_tree.svg
dot -Tpng -Gdpi=110 job_title_family_tree.dot -o job_title_family_tree.png
```

Each title is one node line in `job_title_family_tree.dot`; its row is set
in the `rank=same` blocks (one per five-year period) and its parents in the lineage section.
