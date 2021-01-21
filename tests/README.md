How to use

build by `make test` in the root directory, then run

```bash
UCX_RNDV_SCHEME=put_zcopy SKIP_DEV_ID_CHECK=1 TEST_ENABLE_CPU=0 LOCAL_SIZE=2 BINARY="./test_benchmark" NODE_ONE_IP=xxx NODE_TWO_IP=yyy bash ./ucx_multi_node.sh
SKIP_DEV_ID_CHECK=1 TEST_ENABLE_CPU=1 DMLC_PS_ROOT_PORT=12355 LOCAL_SIZE=0 BINARY="./test_benchmark" NODE_ONE_IP=10.130.23.14 NODE_TWO_IP=10.130.23.21 bash ./ucx_multi_node.sh
```
