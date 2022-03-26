```
usage: active [-l LIMIT] [-h] [--export {csv,json,xlsx}]
```

Print up to 25 top most actively traded intraday tickers. [Source: [Yahoo Finance](https://finance.yahoo.com/most-active/?count=25&offset=0)]

```
optional arguments:
  -l LIMIT, --limit LIMIT
                        Limit of stocks to display. (default: 5)
  -h, --help            show this help message (default: False)
  --export {csv,json,xlsx}
                        Export raw data into csv, json, xlsx (default: )
```

Example:
```
2022 Feb 16, 03:46 (✨) /stocks/disc/ $ active -l 25
                                                                 Most Active Stocks
┏━━━━━━━━┳━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━┳━━━━━━━━━━━━━━━━━━┳━━━━━━━━┳━━━━━━━━━━┳━━━━━━━━━━┳━━━━━━━━━━━━━━━━━━━┳━━━━━━━━━━━━┳━━━━━━━━━━━━━━━━┓
┃ Symbol ┃ Name                                 ┃ Price (Intraday) ┃ Change ┃ % Change ┃ Volume   ┃ Avg Vol (3 month) ┃ Market Cap ┃ PE Ratio (TTM) ┃
┡━━━━━━━━╇━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━╇━━━━━━━━━━━━━━━━━━╇━━━━━━━━╇━━━━━━━━━━╇━━━━━━━━━━╇━━━━━━━━━━━━━━━━━━━╇━━━━━━━━━━━━╇━━━━━━━━━━━━━━━━┩
│ SPCE   │ Virgin Galactic Holdings, Inc.       │ 10.74            │ 2.60   │ +31.94%  │ 178.62M  │ 14.077M           │ 2.771B     │                │
├────────┼──────────────────────────────────────┼──────────────────┼────────┼──────────┼──────────┼───────────────────┼────────────┼────────────────┤
│ AMD    │ Advanced Micro Devices, Inc.         │ 121.47           │ 7.20   │ +6.30%   │ 141.257M │ 73.478M           │ 145.679B   │ 47.26          │
├────────┼──────────────────────────────────────┼──────────────────┼────────┼──────────┼──────────┼───────────────────┼────────────┼────────────────┤
│ NVDA   │ NVIDIA Corporation                   │ 264.95           │ 22.28  │ +9.18%   │ 70.175M  │ 51.247M           │ 660.255B   │ 81.70          │
├────────┼──────────────────────────────────────┼──────────────────┼────────┼──────────┼──────────┼───────────────────┼────────────┼────────────────┤
│ F      │ Ford Motor Company                   │ 18.08            │ 0.62   │ +3.55%   │ 64.555M  │ 108.718M          │ 72.397B    │ 4.06           │
├────────┼──────────────────────────────────────┼──────────────────┼────────┼──────────┼──────────┼───────────────────┼────────────┼────────────────┤
│ AAPL   │ Apple Inc.                           │ 172.79           │ 3.91   │ +2.32%   │ 64.286M  │ 104.284M          │ 2.82T      │ 28.73          │
├────────┼──────────────────────────────────────┼──────────────────┼────────┼──────────┼──────────┼───────────────────┼────────────┼────────────────┤
│ ZNGA   │ Zynga Inc.                           │ 9.05             │ -0.01  │ -0.11%   │ 55.461M  │ 35.399M           │ 10.231B    │                │
├────────┼──────────────────────────────────────┼──────────────────┼────────┼──────────┼──────────┼───────────────────┼────────────┼────────────────┤
│ RBLX   │ Roblox Corporation                   │ 73.30            │ 4.98   │ +7.29%   │ 49.158M  │ 22.259M           │ 42.429B    │                │
├────────┼──────────────────────────────────────┼──────────────────┼────────┼──────────┼──────────┼───────────────────┼────────────┼────────────────┤
│ SOFI   │ SoFi Technologies, Inc.              │ 12.58            │ 0.58   │ +4.83%   │ 50.868M  │ 50.382M           │ 10.059B    │                │
├────────┼──────────────────────────────────────┼──────────────────┼────────┼──────────┼──────────┼───────────────────┼────────────┼────────────────┤
│ PLTR   │ Palantir Technologies Inc.           │ 14.17            │ 0.91   │ +6.86%   │ 48.047M  │ 42.817M           │ 28.408B    │                │
├────────┼──────────────────────────────────────┼──────────────────┼────────┼──────────┼──────────┼───────────────────┼────────────┼────────────────┤
│ NIO    │ NIO Inc.                             │ 25.79            │ 2.00   │ +8.41%   │ 46.697M  │ 53.892M           │ 41.021B    │                │
├────────┼──────────────────────────────────────┼──────────────────┼────────┼──────────┼──────────┼───────────────────┼────────────┼────────────────┤
│ AAL    │ American Airlines Group Inc.         │ 18.84            │ 1.41   │ +8.09%   │ 46.529M  │ 40.319M           │ 12.203B    │                │
├────────┼──────────────────────────────────────┼──────────────────┼────────┼──────────┼──────────┼───────────────────┼────────────┼────────────────┤
│ FB     │ Meta Platforms, Inc.                 │ 221.00           │ 3.30   │ +1.52%   │ 42.685M  │ 29.422M           │ 601.549B   │ 16.05          │
├────────┼──────────────────────────────────────┼──────────────────┼────────┼──────────┼──────────┼───────────────────┼────────────┼────────────────┤
│ BAC    │ Bank of America Corporation          │ 47.79            │ 0.37   │ +0.78%   │ 41.879M  │ 52.171M           │ 386.04B    │ 13.39          │
├────────┼──────────────────────────────────────┼──────────────────┼────────┼──────────┼──────────┼───────────────────┼────────────┼────────────────┤
│ ITUB   │ Itaú Unibanco Holding S.A.           │ 5.14             │ 0.08   │ +1.58%   │ 41.059M  │ 45.848M           │ 50.269B    │ 9.92           │
├────────┼──────────────────────────────────────┼──────────────────┼────────┼──────────┼──────────┼───────────────────┼────────────┼────────────────┤
│ AMC    │ AMC Entertainment Holdings, Inc.     │ 19.48            │ 1.73   │ +9.75%   │ 39.222M  │ 49.237M           │ 10B        │                │
├────────┼──────────────────────────────────────┼──────────────────┼────────┼──────────┼──────────┼───────────────────┼────────────┼────────────────┤
│ ABEV   │ Ambev S.A.                           │ 2.95             │ 0.05   │ +1.72%   │ 38.479M  │ 21.416M           │ 46.429B    │ 15.36          │
├────────┼──────────────────────────────────────┼──────────────────┼────────┼──────────┼──────────┼───────────────────┼────────────┼────────────────┤
│ INTC   │ Intel Corporation                    │ 48.44            │ 0.86   │ +1.81%   │ 35.858M  │ 36.63M            │ 197.248B   │ 9.97           │
├────────┼──────────────────────────────────────┼──────────────────┼────────┼──────────┼──────────┼───────────────────┼────────────┼────────────────┤
│ VALE   │ Vale S.A.                            │ 17.14            │ -0.35  │ -2.00%   │ 33.93M   │ 32.586M           │ 80.669B    │ 4.79           │
├────────┼──────────────────────────────────────┼──────────────────┼────────┼──────────┼──────────┼───────────────────┼────────────┼────────────────┤
│ UBER   │ Uber Technologies, Inc.              │ 37.09            │ 2.50   │ +7.23%   │ 36.234M  │ 32.245M           │ 71.959B    │                │
├────────┼──────────────────────────────────────┼──────────────────┼────────┼──────────┼──────────┼───────────────────┼────────────┼────────────────┤
│ FCEL   │ FuelCell Energy, Inc.                │ 5.49             │ 0.87   │ +18.83%  │ 34.067M  │ 23.922M           │ 2.013B     │                │
├────────┼──────────────────────────────────────┼──────────────────┼────────┼──────────┼──────────┼───────────────────┼────────────┼────────────────┤
│ T      │ AT&T Inc.                            │ 24.34            │ 0.29   │ +1.21%   │ 31.096M  │ 62.336M           │ 173.812B   │ 8.82           │
├────────┼──────────────────────────────────────┼──────────────────┼────────┼──────────┼──────────┼───────────────────┼────────────┼────────────────┤
│ CCL    │ Carnival Corporation & plc           │ 22.78            │ 1.42   │ +6.65%   │ 31.595M  │ 43.634M           │ 26.684B    │                │
├────────┼──────────────────────────────────────┼──────────────────┼────────┼──────────┼──────────┼───────────────────┼────────────┼────────────────┤
│ NOK    │ Nokia Corporation                    │ 5.60             │ 0.17   │ +3.13%   │ 29.464M  │ 24.911M           │ 32.265B    │ 17.07          │
├────────┼──────────────────────────────────────┼──────────────────┼────────┼──────────┼──────────┼───────────────────┼────────────┼────────────────┤
│ PBR    │ Petróleo Brasileiro S.A. - Petrobras │ 13.77            │ -0.21  │ -1.50%   │ 27.492M  │ 31.187M           │ 89.809B    │ 3.49           │
├────────┼──────────────────────────────────────┼──────────────────┼────────┼──────────┼──────────┼───────────────────┼────────────┼────────────────┤
│ MSFT   │ Microsoft Corporation                │ 300.47           │ 5.47   │ +1.85%   │ 27.379M  │ 35.818M           │ 2.253T     │ 32.00          │
└────────┴──────────────────────────────────────┴──────────────────┴────────┴──────────┴──────────┴───────────────────┴────────────┴────────────────┘
```