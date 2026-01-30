# API Refernce sheet


### Full strucuture of stored json file

```
[
    {
        "SAT_1": {
            "ID": "",
            "NAME": "",
            "RCS": "",
            "OBJ_TYP": "",
            "EXCL_VOL": ""
        },
        "SAT_2_OBJS": [
            {
                "SAT_2": {
                    "ID": "",
                    "NAME": "",
                    "RCS": "",
                    "OBJ_TYP": "",
                    "EXCL_VOL": ""
                },
                "CDMS": [
                    {
                        "CDM_ID": "",
                        "CREATED": "",
                        "TCA": "",
                        "MIN_RNG": "",
                        "PC": "",
                        "RISK_LVL": ""
                    }
                ],
                "TCA": "",
                "AI_RISK_LOG10": 0.0,
                "AI_STATUS": "",
                "AI_CERTAINTY": 0.0,
                "AI_RISK_PROB": 0.0,
                "MAX_PC": 0.0,
                "MIN_RANGE": 0.0,
                "MSG_COUNT": 0
            }
        ]

    }
]
```

### /init

```
[
    {
        "ID": 728,
        "NAME": "GGSE 1 (GGRS)",
        "RCS": "MEDIUM",
        "OBJ_TYP": "PAYLOAD",
        "EXCL_VOL": 5.0,
        "SAT2_OBJ_COUNT": 1,
        "TOTAL_CDMS": 6
    },
]
```


### /cdms?sat_id={id}

```
[
  {
    "SAT_2": {
      "ID": 37057,
      "NAME": "FENGYUN 1C DEB",
      "RCS": "SMALL",
      "OBJ_TYP": "DEBRIS",
      "EXCL_VOL": "1.00"
    },
    "CDMS": [
      {
        "CDM_ID": "1316269189",
        "CREATED": "2026-01-23 13:16:56.000000",
        "TCA": "2026-01-25T18:56:54.166000",
        "MIN_RNG": 694.0,
        "PC": 0.0001895421,
        "RISK_LVL": ""
      },
    ],
    "TCA": "2026-01-25T18:56:54.166000",
    "AI_RISK_LOG10": -3.5,
    "AI_STATUS": "ESCALATING",
    "AI_CERTAINTY": 0.85,
    "AI_RISK_PROB": 0.00032,
    "MAX_PC": 0.0003033919,
    "MIN_RANGE": 545.0,
    "MSG_COUNT": 4
  }
]
```