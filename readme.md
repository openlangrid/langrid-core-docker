# docker files for servicegrid core node

## Getting started

1. Place dump sql to ./volumes/postgresql/initdb/
2. Modify ./volumes/tomcat/conf/Catalina/localhost/service_manager.xml to fit your settings.
3. Place war file to ./volumes/tomcat/webapps
4. Modify ./docker-compose.yml to make settings consistent.
5. Run docker-compose
```
# You need to build postgresql first
docker-compose up postgresql
# Then, launch services (postgresql, tomcat)
docker-compose up -d
```

