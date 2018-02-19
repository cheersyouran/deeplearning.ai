### How to download coursera jupyter notebook and all reference files?
### 如何下载coursera jupyter notebook以及所有文件？

1. Open a online jupyter notebook, and then click `File > Open ...`
2. Launch new terminal instance: `New > Terminal`
3. tarball the folder:
```shell
tar czvhf coursera.tar.gz *
```
3. a. split it (usually this file might be too large for your instance to allow download)
```shell
split -b 100M -d coursera.tar.gz coursera.
```
4. Go to view in 2.
5. Download the file(s) by selecting it (square) then clicking on `Download`.

6. if you split the file, join them:
```shell
cat coursera.* > coursera.tar.gz
```
7. Extract files:
```shell
tar xzvf coursera.tar.gz
```
