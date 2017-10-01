# docker-compose的使用

```
docker-compose的使用
	创建machine
		docker-machine create --virtualbox-disk-size "<the-size>" --driver virtualbox <machine-name>
		如：docker-machine create --virtualbox-disk-size "2048"  --driver virtualbox test

	运行machine
		docker-machine start <machine-name>
		如：docker-machine start test

	获取machine配置
		docker-machine env <machine-name>
		如：docker-machine env test

	设置machine参数
		 eval $("D:\Program Files\Docker Toolbox\docker-machine.exe" env <machine-name>)
		 如： eval $("D:\Program Files\Docker Toolbox\docker-machine.exe" env test1)

	进入docker-compose目录(docker-compose.yml文件所在的目录)
		如：cd /c/machine/docker-compose-env/docker-lnmp-3

	运行docker-compose
		docker-compose build
		docker-compose up -d
		docker-compose down

```
