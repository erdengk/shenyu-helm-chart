# Apache ShenYu Helm Chart

Apache ShenYu (Incubating) is a High-performance,multi-protocol,extensible,responsive API Gateway.

This chart bootstraps all the components needed to run Apache ShenYu on a Kubernetes Cluster using Helm.

## Prerequisites

- Kubernetes 1.16+
- Helm v3.0+

## Install

[Helm](https://helm.sh) must be installed to use the charts.  Please refer to
Helm's [documentation](https://helm.sh/docs) to get started.


### Add repo


> helm repo add shenyu https://erdengk.github.io/shenyu-helm-chart
> 
> helm repo update

### Install ShenYu

It can be installed directly with the following command, it will install the latest version of ShenYu by default.

> helm install my-shenyu shenyu-test/shenyu 

### Uninstall the Chart

To uninstall/delete the my-release deployment,

> helm delete my-shenyu

The command removes all the Kubernetes components associated with the chart and deletes the release.

## Configuration

Specify each parameter using the `--set key=value[,key=value]` argument to `helm install`. For example,

> helm install my-shenyu \
--set replicas=3 \
shenyu-test/shenyu

The above command deploys ShenYu with 3 brokers (replicas).

You also can provide a YAML file specifying parameter values when installing the chart. For example,

> helm install my-shenyu -f values.yaml shenyu-test/shenyu

### Option

The following table lists the configurable parameters of the Skywalking chart and their default values.

| **Parameter**     | Description | Default |
| ----------------- | ----------- | ------- |
| admin.tag         |             | 2.4.3   |
| admin.enabled     |             | true    |
| bootstrap.tag     |             | 2.4.3   |
| bootstrap.enabled |             | True    |
| replicas          |             | 1       |




## License

Licensed under the Apache License, Version 2.0 (the "License"); you may not use this file except in compliance with the License. You may obtain a copy of the License at

> http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the specific language governing permissions and limitations under the License.



