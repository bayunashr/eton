---
title: "{{ replace .Name "-" " " | title }}"
date: {{ .Date }}
# weight: 1
tags: ["tag", "tag2"]
draft: false
summary: Summary text
cover:
    image: "<image path/url>" # image path/url
    alt: "<alt text>" # alt text
    caption: "<text>" # display caption under cover
    relative: false # when using page bundles set this to true
    hidden: true # only hide on current single page
---