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

:sparkles: [pr](https://github.com/erdengk/shenyu-helm-chart/commit/53f210ebe103a942a70c902dd68dadb0ea89343e) 实现了CI和自动发版

:sparkles: [pr](https://github.com/erdengk/shenyu-helm-chart/tree/062d312ac23fc297e2881e045d03532a8897ae0b) 验证了发版流程

vim /charts/shenyu/Chart.yaml

cd docs

helm package ../charts/shenyu

helm repo index  --merge index.yaml .


:sparkles: [pr](https://github.com/erdengk/shenyu-helm-chart/commit/1e1609602eda91a72c899ad50c0ab863b0a5a895)

实现了ci 与 发版
但还没有验证是否能够识别出错误的chart


:sparkles: [pr](https://github.com/erdengk/shenyu-helm-chart/commit/099493e70f877e6e994adaa4537ddb44f63b453f)
验证了ci的正确性，可以识别出错误的chart

