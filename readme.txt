mockgen -destination=application/mocks/application.go -source=application/product.go application

sudo apt-get install sqlite3

touch sqlite.db

sqlite3 sqlite.db

go run main.go http