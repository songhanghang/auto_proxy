# Android自动设置网络代理
> 代理抓包从未如此简单....

## 正常流程

1. 进入设置
2. 进入 WLAN
3. 找对应 wifi 连接
4. 进入详情
5. 找到代理
6. 选择手动
7. 输入主机名
8. 输入端口号
9. 最后保存

每次都是重复操作，累加的时间成本很高，
一不小心，还会写错 ...

## 自动设置
只需一行代码，自动获取本机 IP 设置抓包代理。
支持WiFi和网线环境下自动设置代理

#### 设置默认代理
``` bash
$ easyproxy set
```
#### 设置自定义代理
```bash
$ easyproxy set ****:8888
```
#### 清除代理

```bash
$ easyproxy clean
```
## 安装


```bash
./install.sh
```
如果使用zsh, 辛苦执行下
``` shell
$ source ~/.zshrc
```

## 

### FAQ
* Q: 执行命令时 Not find Command
  A: 解决办法 
  bash下 
  
  ``` shell
   $ source ~/.bashrc
  ``` 
  zsh下 

  ``` shell
  $ source ~/.zshrc
  ```
* Q: 设置代理后WiFi高级选项中看不到代理信息? 没办法取消代理?
  A: 对滴，手机上无法取消，必须通过命令取消！！！ 鱼与熊掌自选...
