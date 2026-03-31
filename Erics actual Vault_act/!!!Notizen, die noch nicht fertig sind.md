
Filter:
aus Ressources ohne Lit = alle pkm-Notizen ohne die Literaturnotizen
bei denen der Status new oder ongoing ist 

```dataview
list status
from "03 Ressources"
AND !"03 Ressources/Lit"
where contains(status, "new") OR contains(status, "ongoing")
SORT status Asc
```
