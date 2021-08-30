## Setup Instructions
1. Create Environment - ```conda env create -f api_crtn_env.yml```
2. Activate Environment - ```conda activate flask_env```
3. Run ```python server.py``` to start serving the API
4. Once the server is started, open another terminal and execute the below command:
     1. ``import requests``
     2. ``import json``
     3. ``header = {'Content-Type': 'application/json', 'Accept': 'application/json'}``
     4. ``resp = requests.post("http://127.0.0.1:5000/checkout", data = json.dumps(['001','001','002']),headers= header) ``
     5. ``resp.json()``
