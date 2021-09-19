# Deploy
* `docker-compose up-d`
* open `http://localhost:3000/` in the browser
* create new connection using username `root`, password `example`

# Import Northwind.MySQL5.sql
* `docker ps`
* copy `mysql` container id
* `docker cp ~/Downloads/Northwind.MySQL5.sql CONTAINER_ID:/var/db.sql`
* `docker exec -it CONTAINER_ID bash`
* `mysql -u root -p example`
* `source /var/db.sql`