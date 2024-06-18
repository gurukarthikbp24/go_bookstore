# GoBookstoreAPI

## Description
This project is a RESTful API for managing a bookstore. It allows users to perform CRUD (Create, Read, Update, Delete) operations on books in the database.

## Technology Stack
- **Language**: Golang
- **Database**: MySQL

## Setup
1. **Clone the repository**
   
2. **Initialize the Go module and install dependencies**:
```bash
go mod init
go get "github.com/jinzhu/gorm"
go get "github.com/jinzhu/gorm/dialects/mysql"
go get "github.com/gorilla/mux"
```
  
3. **Set up the MySQL database container**:
```bash
docker pull container-registry.oracle.com/mysql/community-server:latest
docker run --name my-mysql-container -e MYSQL_ROOT_PASSWORD=root -e MYSQL_DATABASE=password -p 3306:3306 -d mysql:latest
```

4. **Run the application**:
```bash
go build
go run main.go
```
## Usage
The API endpoints include:
- `POST /books`: Add a new book to the bookstore.
- `GET /books`: Retrieve a list of all books.
- `GET /books/:id`: Retrieve a book by its ID.
- `PUT /books/:id`: Update a book's information.
- `DELETE /books/:id`: Remove a book from the bookstore.

## License
This project is licensed under the MIT License
