# shenyu-helm-chart
Helm deployment documentation written for Apache/Shenyu

# Artifact Hub

[![Artifact Hub](https://img.shields.io/endpoint?url=https://artifacthub.io/badge/repository/shenyu-test)](https://artifacthub.io/packages/search?repo=shenyu-test)


## Usage

[Helm](https://helm.sh) must be installed to use the charts.  Please refer to
Helm's [documentation](https://helm.sh/docs) to get started.

Once Helm has been set up correctly, add the repo as follows:

add repo

> helm repo add shenyu https://erdengk.github.io/shenyu-helm-chart

install:

> helm install my-shenyu shenyu-test/shenyu --version 0.1.0



have fun～

## Timeline


### Validated release process

:sparkles: [pr](https://github.com/erdengk/shenyu-helm-chart/tree/062d312ac23fc297e2881e045d03532a8897ae0b) 


~~vim /charts/shenyu/Chart.yaml~~

~~cd docs~~

~~helm package ../charts/shenyu~~

~~helm repo index  --merge index.yaml .~~

~~git push~~

~~merge into main~~


### Implemented CI and release

But it has not been verified whether the wrong chart can be identified

:sparkles: [pr](https://github.com/erdengk/shenyu-helm-chart/tree/1e1609602eda91a72c899ad50c0ab863b0a5a895)


### The correctness of ci is verified 

**The wrong chart can be identified**

:sparkles: [pr](https://github.com/erdengk/shenyu-helm-chart/commit/099493e70f877e6e994adaa4537ddb44f63b453f)

### V2.4.25

🎉🎉🎉

~~Implemented automatic deployment~~

Implemented CI validation

### V2.4.27

🎉🎉🎉

Implemented automatic deployment




