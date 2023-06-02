# Pandas
```
import pandas as pd
import numpy as np
```

```
dataset = "C:/NOTE/SourceCodes/Python/Trial3/Tuesday-WorkingHours.pcap_ISCX.csv"
data = pd.read_csv(dataset)
data
```

```
monday.drop(['Unnamed: 0', 'Flow ID', 'Source IP', 'Destination IP', 'Timestamp'], axis = 1, inplace = True)
```

```
monday_new = monday[np.isfinite(monday).all(1)]
```
