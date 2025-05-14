# kdhr-test
This project contains tests for kdhr project.

We prepare a docker image on [baidu netdisk](https://pan.baidu.com/s/1R4PHpcVAS2xEkqVgWHvNEg?pwd=bqrh).
Download this image, and execute the following commands to open the test environment:
```bash
gunzip kdhr-test.tar.gz
docker import kdhr-test.tar kdhr-test:latest
docker run -itd --privileged --name kdhr-test:latest /bin/bash
docker exec -it kdhr-test /bin/bash
su dhr # Password = 123456
cd ~/kdhr-test
```
Then run tests by `sudo ./test.exp <test_name> [noprotect]`.
Example:
```bash
sudo ./test.exp test2.1
sudo ./test.exp test2.2/rop noprotect
```
