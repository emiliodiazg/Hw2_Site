# Dataframe: `hw2:fed_funds_futures` - 30-Day Fed Funds Futures (ZQ), Daily Bars

Daily bars from the CME Globex dataset (GLBX.MDP3), pulled with parent symbology (ZQ.FUT) and the ohlcv-1d schema. Columns: date (tz-naive trading date), symbol, open, high, low, close, volume. ZQ contracts are quoted as 100 minus the average effective fed funds rate over the contract month, so the implied rate is 100 - close. The file includes calendar-spread symbols alongside the outright monthly contracts; filter them with fedwatch.filter_outright_contracts before use. Free under the course Databento subscription; the pull checks that the cost estimate is $0.00 before downloading.


## DataFrame Glimpse

```
Rows: 11755
Columns: 7
$ date   <datetime[ns]> 2026-10-19 00:00:00
$ symbol          <str> 'ZQN7'
$ open            <f64> 95.45
$ high            <f64> 95.45
$ low             <f64> 95.375
$ close           <f64> 95.38
$ volume          <u64> 1479


```

## Dataframe Manifest

| Dataframe Name                 | 30-Day Fed Funds Futures (ZQ), Daily Bars                                                          |
|--------------------------------|--------------------------------------------------------------------------------------|
| Dataframe ID                   | [fed_funds_futures](../dataframes/hw2/fed_funds_futures.md)                                       |
| Sources                        | CME Group                                          |
| Providers                      | Databento                                        |
| Provider Links                 | https://databento.com/                                   |
| Tags                           | Futures, Monetary Policy, Federal Reserve, Fedwatch                                             |
| Access Types                   |                                       |
| How is data pulled?            | Databento Historical API via Python                                                   |
| Data available up to (min)     | 2026-10-19 00:00:00                                                             |
| Data available up to (max)     | 2026-10-19 00:00:00                                                             |
| Dataframe Path                 | /Users/emiliodiaz/Library/CloudStorage/OneDrive-Personal/UChicago/Autum_Quarter/Data_Pipeline/hw2-emiliodiazg/_data/fed_funds_futures.parquet                                             |


**Linked Charts:**


- [hw2:fedwatch_latest_forecast](../../charts/hw2.fedwatch_latest_forecast.md)



## Pipeline Manifest

| Pipeline Name                   | HW 2: The Yield Curve and the Policy Path                       |
|---------------------------------|--------------------------------------------------------|
| Pipeline ID                     | [hw2](../../../index.md)              |
| Maintainer                      | Jeremiah Bejarano               |
| Contributors                    | Jeremiah Bejarano |
| Repository                     | https://github.com/hw-finm-32800/hw2                  |
| Pipeline Web Page               | <a href="file:///Users/emiliodiaz/Library/CloudStorage/OneDrive-Personal/UChicago/Autum_Quarter/Data_Pipeline/hw2-emiliodiazg/docs/index.html">Pipeline Web Page      |
| Date of Last Code Update        | 2026-10-20 22:10:08           |
| OS Compatibility                | Windows, Linux, macOS |
| Linked Dataframes               |  [hw2:crsp_treasury_consolidated](../../dataframes/hw2/crsp_treasury_consolidated.md)<br>  [hw2:fed_yield_curve](../../dataframes/hw2/fed_yield_curve.md)<br>  [hw2:fed_funds_futures](../../dataframes/hw2/fed_funds_futures.md)<br>  |


**Build Commands:**
```
doit

```

