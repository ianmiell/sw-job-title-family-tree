# Software industry job title family tree

A Graphviz family tree of software industry job titles, from the 1940s
("Computer", "Coder", "Programmer") to the present (SRE, Platform Engineer,
Forward Deployed Engineer, AI Engineer).

![Family tree](job_title_family_tree.png)

- Columns are decades: roughly when a title became common, not its first
  recorded use.
- Solid arrow: the title grew out of its parent. Dashed arrow: influence or a
  common career move.
- Colours mark families: development, architecture/leadership,
  operations/infrastructure, networks/security, data/AI, quality/test,
  support/customer-facing.

## Rendering

```sh
dot -Tsvg job_title_family_tree.dot -o job_title_family_tree.svg
dot -Tpng -Gdpi=110 job_title_family_tree.dot -o job_title_family_tree.png
```

Each title is one node line in `job_title_family_tree.dot`; its era is set
in the `rank=same` blocks and its parents in the lineage section.
