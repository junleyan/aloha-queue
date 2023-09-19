# AlohaQueue
A user-friendly Python library designed to streamline the process of checking appointment availability on AlohaQ. 
 <br>*( Currently, appointment checking is ONLY available for the written permit test )*


## Installation
``` sh
pip install aloha-queue
```   

## Examples
```py
from alohaqueue import QueueChecker

# QueueChecker(location, target month, target day, target year)
checker = QueueChecker("KAPA", 12, 12, 2023)

# returns all available appointment dates before 12/12/2023
available_dates = checker.get_available_dates()
# returns all available appointment time on 06/06/2023
available_time = checker.get_available_time("2023-06-06")
```

## Locations Abbreviations 
- `"KAPA"` : Kapalama Driver Licensing Center
- `"KAPO"` : Kapolei Driver Licensing Center
- `"KOOL"` : Koolau Driver Licensing Center
- `"WADL"` : Wahiawa Driver Licensing Center
- `"WAIA"` : Waianae Driver Licensing Center
