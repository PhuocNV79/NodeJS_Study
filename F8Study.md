## NodeJS la 1 moi truong runtime duoc xay dung dua tren Chrome's V8 JavaScript engine cua google

- Chrome's V8 JavaScipt engine la 1 `trinh thong dich code javascript` **khong phai bien dich**
- NodeJS chay tren server, NodeJS su dung Chrome's V8 JavaScript engine
- `node -v` : kiem tra version nodejs
- `npm -v` : kiem tra version node package management
- `nvm -v` : kiem tra version node version manageent
- `npm init` : khoi tao du an nodejs
- **package.json** : filie cau hinh va thong tin du an
- **package-lock.json** : file quan ly dependencies, dependencies cua dependencies...
- `npm install express` : cai dat framework expressjs
- trang chu expressjs
- `require('express')` : cu phap nap thu vien express. Nodejs se di vao thu muc "express" trong thu muc node_modlues de no tai. Cac thu vien khac cung nap tuong tu
- `app = express()` : tao 1 instance cua thu vien express ten la app. app dai dien cho ung dung nodejs cua minh
- `node index.js` : chay file index.js bang nodejs
- `inspect source, header, response ...`

### Nodemon & inspector

- nodemon se lang nghe nhung thay doi trong source code va auto restart lai ung dung => khong can phai tat node va khoi chay lai node thu cong
- `npm install -g nodemon --save-dev` : cai nodemon o global, se cai o thu muc node_modules o Users chu ko phai o thu muc du an hien tai, va chi phuc vu cho viec dev chu ko phai cho product sau nay
- `npm install nodemon` : cai nodemon o thu muc du an
- `start: "nodemon index.js` : bao cho nodemon khoi chay file index.js khi start nodemon
- `npm start` : Cau lenh nay se doc dong script `start: "nodemon index.js` de chay nodemon index.js
- `--inspect` : giup debug ung dung nodejs => neu co beakpoint thi ung dung se dung tai breakpoit de debug\

### Morgan

- morgan giup quan sat duoc cac log cua request tu phia client gui len nodejs server
- `npm install morgan --save-dev` : cai dat thu vien morgan de phuc vu trong dev => save trong devdependencies trong package.json
- `combined tiny common ...` : predefined format string trong khi ghi log voi morgan
- `app.use(morgan(combined))` : su dung morgan ghi log voi dinh dang combined

### Handlebars template engine
### Bug template engine de viet code html css

### Basic routing 

- `app.get(path, handler)` : xu ly voi duong dan path on server (source code on server localhost, server cloud, server abc) voi phuong thuc get voi cach xu ly handler. **method o dang lowercase**

### Get method
### Post method

- `req.body` : lay du lieu duoc gui len tu client voi phuong thuc post
- express da tich hop san 1 middware de xu ly query parameters. con body thi chua co
- express version >= 4.16 da co tich hop middware xu ly body , `body-parser`
- `app.use(express.urlendcoded({extended : true}))` : apply middware xu ly du lieu tu form subbmit len bang phuong thuc post
- `body-parser` : phu thuoc vao `qs`
- `qs` : ban chat la querystring, qs parse sang dang key:value

### Route & Controllers

- `module.exports = new NewsController` : export Class NewsController ra ngoai
- tat ca file route deu can duoc nap vao file index.js trong folder routes

### MVC Model

- `npm install pg-promise` : cai dat module pg-promise de ket noi voi postgresql


