+++
title = '{{ replace .File.ContentBaseName "-" " " | title }}'
date = {{ .Date }}
album = '{{ replace .File.ContentBaseName "-" " " | title }}'
draft = true
+++
{{< gallery "album path" >}}