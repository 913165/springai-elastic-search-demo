# springai-elastic-search-demo


```dockerfile
docker network create  somenetwork
docker run -it --name elasticsearch --net somenetwork -p 9200:9200 -p 9300:9300 -e "discovery.type=single-node" elasticsearch:8.15.1
```

### git bash commands
```shell
openssl s_client -showcerts -connect localhost:9200 </dev/null | sed -n -e '/-.BEGIN/,/-.END/ p' > certifs.cer
keytool -import -alias elasticcert -file "C:\temp\certifs.cer" -keystore "C:\Program Files\Java\jdk-22\lib\security\cacerts"
```
