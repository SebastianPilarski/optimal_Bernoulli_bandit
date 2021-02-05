# **Rate of Suboptimal Decisions**
This data reports what fraction of decisions a given algorithm makes while playing are suboptimal (i.e., would disagree with the optimal policy). 

## **Directory Structure**
```
|-- 2-arm
    |-- ucb
        |-- beta_1_1
            |-- *_csop
            |-- *_sop
        |-- ... 
    |-- ...
|-- 3-arm
    |-- ...
```

## **File Types**
All data is averaged across 1 million runs.
|**File Type** | **Meaning**                  |
|--------------|-------------------------     |
|sop           | Rate of suboptimal decisions on last arm pull  |
|csop          | Rate of suboptimal decisions across entire game|
