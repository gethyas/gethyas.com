---
title: "Archetypes"
description: "Customize archetype templates for blog posts and default pages."
lead: "Customize archetype templates for blog posts and default pages."
date: 2020-09-21T13:58:42+02:00
lastmod: 2020-09-21T13:58:42+02:00
draft: false
images: []
menu:
  docs:
    parent: "setup"
weight: 323
toc: true
---

```bash
..
├── blog.md
└── default.md
```

See also the Hugo docs: [Archetypes](https://gohugo.io/content-management/archetypes/).

## Customize archetypes

### blog.md

```md
---
title: "{{ replace .Name "-" " " | title }}"
description: ""
excerpt: ""
date: {{ .Date }}
lastmod: {{ .Date }}
draft: true
weight: 50
images: ["{{ .Name | urlize }}.jpg"]
categories: [""]
---
```

### default.md

```md
---
title: "{{ replace .Name "-" " " | title }}"
description: ""
date: {{ .Date }}
lastmod: {{ .Date }}
draft: true
images: []
---
```
