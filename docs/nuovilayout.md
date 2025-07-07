```mermaid
---
title: Nuovi layout architecture
---
classDiagram
class IDAO~T~
<<interface>>IDAO~T~
IDAO~T~: Read List~T~
IDAO~T~: Read(AId) T
IDAO~T~: Read(AFilter) List~T~
IDAO~T~: Insert(AModel) Int
IDAO~T~: Delete(AId)
IDAO~T~: Update(AModel)

IDAO~T~ <|-- TDAOFireDAC~T~ : implements
IDAO~T~ <|-- TDAOMarshmallow~T~ : implements
IDAO~T~ <|-- TDAOJSONMockup~T~ : implements
```
