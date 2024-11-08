### 从阿里云拉取db和web的docker镜像
```
docker login --username=aliyun2870171523 crpi-rmc3vl74gfshbdna.cn-hangzhou.personal.cr.aliyuncs.com
docker pull crpi-rmc3vl74gfshbdna.cn-hangzhou.personal.cr.aliyuncs.com/mychanku/flask:v1.0
docker pull crpi-rmc3vl74gfshbdna.cn-hangzhou.personal.cr.aliyuncs.com/mychanku/chuan:v1.1
```
5002端口为web进入端口
3307端口为mysql进入端口
### 创造compose
1. 在compose.yml中设置MySQL文件地址
2. 用`docker compose up -d启动服务
3. 可以用sql文件创建数据
