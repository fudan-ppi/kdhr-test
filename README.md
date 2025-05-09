# kdhr-test
This project contains tests for kdhr project.

We prepare a docker image on [baidu netdisk](https://pan.baidu.com/s/1P24DQjRLry7eFph_gUpR8w?pwd=ruen).
Download this image, and execute the following commands to open the test environment:
```bash
gunzip kdhr-test.tar.gz
docker import kdhr-test.tar kdhr-test:latest
docker run -itd --privileged --name kdhr-test:latest /bin/bash
docker exec -it kdhr-test /bin/bash
su dhr # Password = 123456
cd ~/kdhr-test
```
Then run tests by `./test.exp <test_name>`.
Example:
```bash
./test.exp test2.1
```
