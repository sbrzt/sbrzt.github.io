---
title: Precision and Recall
---

Computing precision/recall requires a ground truth — a set of documents you know should or shouldn't be returned.

```
Precision = |Retrieved ∩ Relevant| / |Retrieved|   # of what I got, how much is correct?
Recall    = |Retrieved ∩ Relevant| / |Relevant|    # of what exists, how much did I find?
F1        = 2 * (Precision * Recall) / (Precision + Recall)
```

Recall is fundamentally unmeasurable without knowing the full relevant set. What you can realistically measure is estimated recall on your sample, and precision on your full retrieved set. F1 follows from those.