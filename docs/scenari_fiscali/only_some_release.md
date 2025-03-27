```mermaid
---
title: Bugfix / feature da rilasciare solamente in alcune versioni
---
gitGraph
   branch 6.8
   branch 6.7
   branch 6.6
   branch 6.5
   checkout 6.5
   commit
   checkout 6.6
   commit
   checkout 6.7
   commit
   checkout 6.8
   commit type: HIGHLIGHT tag: "6.8.1.0"
   checkout 6.7
   merge 6.8 tag: "6.7.1.0"
   checkout 6.6
   merge 6.8 tag: "6.6.1.0"
```
