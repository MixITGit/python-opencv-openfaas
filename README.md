# OpenFaaS python openCV

Template for running OpenCV with python
## Quickstart

1. Dodwload tepmplate
    ```
    faas-cli template pull https://github.com/MixITGit/python-opencv-openfaas.git
    ```
2. Create new function
    ```
    faas-cli new --lang python3-opencv demo
    ```

Example handler:

```python
import cv2
def handle(req):
    """handle a request to the function
    Args:
        req (str): request body
    """

    return cv2.__version__
```