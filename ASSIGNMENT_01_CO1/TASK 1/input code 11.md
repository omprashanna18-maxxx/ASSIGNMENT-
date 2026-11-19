**import json**



**RATE\_CARD = {**

&#x20;   **"base": 30.0,**

&#x20;   **"fat": 0.40,**

&#x20;   **"snf": 0.30**

**}**



**def calculate\_rate(fat, snf):**

&#x20;   **fat\_steps = round((fat - 3.5) / 0.1)**

&#x20;   **snf\_steps = round((snf - 8.5) / 0.1)**



&#x20;   **rate = RATE\_CARD\["base"] + fat\_steps \* RATE\_CARD\["fat"] + snf\_steps \* RATE\_CARD\["snf"]**

&#x20;   **return round(rate, 2)**



**for fat, snf in \[(3.5, 8.5), (4.2, 8.7), (3.1, 8.3)]:**

&#x20;   **print("Rate:", calculate\_rate(fat, snf))**

