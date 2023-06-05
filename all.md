# Pandas

# Import Library
```
import pandas as pd
import numpy as np
```

# Import Dataset
```
dataset = "C:/NOTE/SourceCodes/Python/Trial3/Tuesday-WorkingHours.pcap_ISCX.csv"
data = pd.read_csv(dataset)
data
```

# Drop kolom permanen ['Unnamed: 0', 'Flow ID', 'Source IP', 'Destination IP', 'Timestamp']
```
monday.drop(['Unnamed: 0', 'Flow ID', 'Source IP', 'Destination IP', 'Timestamp'], axis = 1, inplace = True)
```

# Change infinite  
```
monday_new = monday[np.isfinite(monday).all(1)]
```

# Choose colomn
```
X1 = friday_new.iloc[:, 0:83]
y1 = friday_new.iloc[:, 79:80]
```

# Count value of parameter
```
X1.Label.value_counts()
y1.value_counts()
```

# Choose with Label = 0
```
c1 = X1.loc[y1['Label'] == 0]
c2 = y1.loc[y1['Label'] == 0]
```
