# **Core Data**
Core data contains normalized simulation data averaged over 1 million simulations. 
## **Directory Structure**
```
|-- 2-arm
    |-- ...
    |-- opt
        |-- beta_1_1 
            |-- *_cmax
            |-- data
                |-- *_cmax
                |-- ...
            |-- ...
        |-- ... 
    |-- ...
|-- 3-arm
    |-- ...
|-- 10-arm
    |-- ...
|-- 15-arm
    |-- ...
```


Files in data subdirectories concern individual runs from time 1 to time horizon. Files extracted by scripts - in the parent directory and not in a data directory - concern consecutive time horizons (i.e., extracted last element from each accompanying time horizon run).

## **File Types**
All files contain normalized data (i.e., value is divided by its time). E.g., to get total reward multiply the data in a mean file by the accompanying time.

**Non-cumulative** - Averaged over 1 million runs
|**File Type** | **Meaning**                  |
|--------------|-------------------------     |
|max           | Maximum reward               |
|mean          | Average reward               |
|msd           | Std. deviation of max        |
|opsd          | Std. deviation of best arm selection   |
|optm          | Best arm selected            |
|rgrt          | Regret          |
|rgsd          | Std. deviation of regret     |
|sdev          | Std. deviation of mean reward|

\
**Cumulative:** - Averaged over 1 million runs
|**File Type**  | **Meaning**                             |
|-------------- |-------------------------                |
|cmax           | Cumulative maximum reward               |
|cmean          | Cumulative average reward               |
|cmsd           | Cumulative std. deviation of max        |
|copsd          | Cumulative std. deviation of best arm selection   |
|coptm          | Cumulative best arm selected            |
|crgrt          | Cumulative regret          |
|crgsd          | Cumulative std. deviation of regret     |
|csdev          | Cumulative std. deviation of mean reward|