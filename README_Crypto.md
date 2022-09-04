## Usage of Daisi

It is recommended to use this application on the daisi platform itself using the link https://app.daisi.io/daisies/vijay/Crypto%20Tracker/app. However, you can still use your own editor using the below method:

### First, load the Packages:

```
import pydaisi as pyd
import plotly.express as px
```

### Now, connect to Daisi and access the functions using:

```
crypto_hist = data_crypto.history(start=start_date, end=end_date, interval=data_interval)
fig = px.line(crypto_hist, x=crypto_hist.index, y=value_selector, labels={"x": "Date"})
fig.show()
```

## And done! We have the history chart of the required cryptocurrency!
