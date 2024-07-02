+++
title = "Batch rename files bash script"
date = 2024-07-02
+++

```bash
num=0; for i in *; do mv "$i" "$(printf '%04d' $num).${i#*.}"; ((num++)); done
```