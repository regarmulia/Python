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

```
X1 = friday_new.iloc[:, 0:83]
y1 = friday_new.iloc[:, 79:80]
```

```
X1.Label.value_counts()
y1.value_counts()
```

```
c1 = X1.loc[y1['Label'] == 0]
c2 = y1.loc[y1['Label'] == 0]
```
