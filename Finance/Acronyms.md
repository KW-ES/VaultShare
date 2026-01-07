---
type: "[[Notes]]"
related:
  - "[[Useful]]"
---

- SCF: Simple Cashflow

# Dataview

```dataview
TABLE
link(
  file.path,
  choice(
    contains(file.path, "Personal"),
    file.name,
    choice(
      contains(file.name, dateformat(file.day, "yyyy-MM-dd")),
      join(
        slice(
          split(file.name, " "),
          1
        ),
        " "
      ),
      file.name
    )
  )
) AS "Page",
a AS "Acronym"
WHERE any(a) = True


```
