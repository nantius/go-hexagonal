### WHAT IS THIS?
A small example of hexagonal architecture using GO.

## SETUP
docker-compose up
docker exec -it appproduct bash
sqlite3 db.sqlite
create table products(id string, name string, price float, status string);

## COBRA CLI
cobra init --pkg-name=github.com/nantius/go-hexagonal
go run main.go cli -a=create -n="product cli"  -p=25.0
go run main.go cli -a=get --id=b7288904-9e30-421f-832b-a66abe09ac8b

## STARTING SERVER
go run main.go http