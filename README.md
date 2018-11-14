# ServeRmore

A package to improve fast and iterative workflow between RStudio and AWS Lambda Function hosting.

## Prerequisites

Please refer to our [LAPTOP.md Guide](LAPTOP.md) for necessary manual configurations.

## Developing

```
python3 setup.py sdist
aws s3 cp dist/ServeRmore-0.0.1.tar.gz s3://origent-public-demo/survival-titanic/ServeRmore-0.0.1.tar.gz

aws s3 cp s3://origent-public-demo/survival-titanic/ServeRmore-0.0.1.tar.gz ServeRmore-0.0.1.tar.gz

pip3 install ServeRmore-0.0.1.tar.gz
```

We are currently working at the 1st usable package release, v0.0.1. You will be able to install this package on RStudio Desktop (using Ubuntu on Linux) or RStudio Server (running on Linux).  From there, you can interact with the package from the RStudio Terminal, and ideally through RScripts.

To Do:
* Create a generic handler.py
* Practice updating RStudio code and redeploying to a Lambda Function
* Setup a Test API and practice with it
