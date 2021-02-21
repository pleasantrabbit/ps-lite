How to use

build by `make test` in the root directory, then run

```bash
# GPU <-> CPU push_pull
NODE_ONE_IP=xxx NODE_TWO_IP=yyy BINARY="./tests/test_benchmark" LOCAL_SIZE=2 bash ./test.sh
# CPU <-> CPU push_pull
NODE_ONE_IP=xxx NODE_TWO_IP=yyy BINARY="./tests/test_benchmark" LOCAL_SIZE=0 bash ./test.sh
# CPU <-> CPU gather scatter
NODE_ONE_IP=xxx NODE_TWO_IP=yyy BINARY="./tests/test_benchmark_stress" bash ./test_stress.sh
# local CPU multi-port
DMLC_NODE_HOST=xxx bash run_benchmark.sh `ROLE`
```
