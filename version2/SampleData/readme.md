Dataset V2 structured in a 14 day folder (Day1 up to Day14), the structure of each folder is like follows:
```
Day
├── container_level
├── NFV_level
├── physical_level
└── RAN_level
    ├── site1_2
    ├── site3
    └── site4
```

This is a sample dataset extracted from the main dataset, Each file has the following attributes:


    format: csv
    duration: 10 mins
    sampling interval: 300ms

    columns --> features
    rows --> data instances

File specific information:

    physical_level:
        Sample_Server_1.csv
            number of rows: 2000
            number of columns: 2360
            file size: 26 MB (approx)

        Sample_Server_2.csv
            number of rows: 2000
            number of columns: 2570
            file size: 29 MB (approx)

        Sample_Server_3.csv
            number of rows: 2000
            number of columns: 2509
            file size: 28 MB (approx)

        Sample_Server_4.csv
            number of rows: 2000
            number of columns: 2085
            file size: 23 MB (approx)

        Sample_Server_5.csv
            number of rows: 2000
            number of columns: 2826
            file size: 26 MB (approx)

        Sample_Server_6.csv
            number of rows: 2000
            number of columns: 1374
            file size: 15 MB (approx)

        Sample_Server_7.csv
            number of rows: 2000
            number of columns: 1211
            file size: 12 MB (approx)

    container_level:
        Sample_Open5GS.csv
            number of rows: 2000
            number of columns: 695
            file size: 6 MB (approx)

        Sample_SRS_gNB.csv
            number of rows: 2000
            number of columns: 821
            file size: 6 MB (approx)

        Sample_SRS_UE_Set1.csv:
            number of rows: 2000
            number of columns: 1010
            file size: 7 MB (approx)

    NFV_level:
        Sample_amf.csv
            number of rows: 2000
            number of columns: 26
            file size: < 1 MB (approx)

        Sample_pcf.csv
            number of rows: 2000
            number of columns: 13
            file size: < 1 MB (approx)

        Sample_smf.csv
            number of rows: 2000
            number of columns: 28
            file size: < 1 MB (approx)

        Sample_upf.csv
            number of rows: 2000
            number of columns: 15
            file size: < 1 MB (approx)
    
    RAN_level:
        Sample_gnb01_metrics_day10.json
            number of rows: 200
            number of columns: 90
            file size: < 1 MB (approx)

        Sample_ue01_metrics_day10.csv
            number of rows: 200
            number of columns: 64
            file size: < 1 MB (approx)