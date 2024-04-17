# CAC BUOC THUC HIEN

# Tao local repo
cd This PC 
cd Documents
cd Zalo Recieve Files 
mkdir backend-mongodb 
cd backend-mongodb
echo "CAC BUOC THUC HIEN" > README.md 

# Tao CSDL bang MongoDB
use bookstore
db.createCollection('books')
db.books.insert({title: 'Book Title', author: 'Author Name', year: 2024})
db.books.find({year: {$gt: 2000}})
db.books.find({author: 'Author Name'})
db.books.find({title: /^A/}) 
db.books.update({title: 'Book Title'}, {$set: {year: 2025}})
db.books.update({title: 'Book Title'}, {$set: {author: 'New Author Name'}})
db.books.remove({title: 'Book Title'})

# Tao repo tren git va push file len 
