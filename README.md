Cách tạo đồ án react

tạo 2 file client và server

sau đó vào client nhập lệnh bên dưới
npx create-react-app .	

tạo tên tailwind nhập 2 lệnh bên dưới
npm install -D tailwindcss
npx tailwindcss init

sau đó vào tailwind.config 
thay đổi thành 

/** @type {import('tailwindcss').Config} */
module.exports = {
  content: ["./src/**/*.{html,js}"],
  theme: {
    extend: {},
  },
  plugins: [],
}


sau đó nhập lệnh này vào client

npm i redux react-redux redux-persist


Tải thêm thư viện 

npm i thunk axios react-router-dom

thunk: dùng để sử lí bất động bộ của react và redux
axios: dùng để call api
react-router-dom: để tạp router cho react 

2 cái file bên trong container là
Public: dùng để hiển thị những trang mà không cần đăng nhập
System: dùng để cần có login mới coi được 


cài icon 
npm install react-icons


==============================


Server

đầu tiên cài lệnh để -y cho nó là mặc định
npm init -y

sau đó vào package.json

đổi trong script

test -> start
bên trong đổi lại thành 

nodemon --exec babel-node server.js


sau đó cài thêm để call api

npm i express dotenv cors nodemon

và 

npm i -D @babel/core @babel/node @babel/preset-env




nhập lệnh này để tải thư viện kết nối 

npm install --save sequelize mysql2


sau đó cài để tương tác với db

npm install --save-dev sequelize-cli

npx sequelize-cli init



để tạo model User gõ

npx sequelize-cli model:generate --name User --attributes firstName:string,lastName:string,email:string


gõ lệnh này nó sẽ tự tạo 1 cái bảng trong db

npx sequelize db:migrate 



Sau đó cập nhật lại db 

npx sequelize db:migrate


Sau đó cài 

npm i bcryptjs jsonwebtoken


Cài 

npm i uuid
