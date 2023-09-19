# aloha-queue
A user-friendly Python library designed to streamline the process of checking appointment availability on AlohaQ. 


## Installation
``` sh
pip install aloha-queue
```   

## Examples
```py
from alohaqueue import QueueChecker

checker = QueueChecker("KAPA", 12, 12, 2023)

# returns all available appointment dates before 12/12/2023
available_dates = checker.get_available_dates()
# returns all available appointment time on 12/12/2023
available_time = checker.get_available_time("2023-12-12")
```
