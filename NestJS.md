## Nest CLI

1. `nest new nameProject`: create new project
2. `npm run start:dev`: start server 
3. `nest generate module nameOfModule` : create new module
4. `nest generate controller messages/messages --flat`
5. `nest g module tenModule` : tao module moi
6. nest g controller tasks --no-spec : ko tao spec
7. nest g service tasks --no-spec
8. yarn add uuid: universal unique id

### Section10 : 61. How to build intercepter
Interceptor nhu 1 nguoi danh chan o ca 2 dau. request va response
- Tao interceptor su dung cho tat ca cac module

### Section 14:
#### 111: Applyinng dotenv for config
- NestJs noi la: co the su dung nhieu file .env trong 1 du an
- Dotenv noi la: chi nen su dung 1 file .env cho 1 du an
- `ConfigModule`: su dung de chi ra file .env nao minh muon su dung
- `ConfigService`: dung de doc thong tin trong file .env

### NestJS Pipe

# NESTJS ZERO TO HERO
## Section 2: Task Management Application
### 9: Introduction to NestJS module
 - @Module decorator: Khai bao 1 class nao do lam module
 - providers: 1 mang cac provider duoc su dung trong module dua vao dependency injection
 - controllers: 1 mang cac contorller duoc khoi tao trong module
 - exports: 1 mang cac provider duoc export de su dung cho cac module khac
 - imports: danh sach cac **module nào đó** can thiet cho module hien tai. Cac provider duoc export boi **module đó** cung se duoc su dung trong module hien tai dua vao DI

### 10: Create a task module
 - `nest g` : nest cli se tao duoc nhieu thu: module, entity, gateway, resouce
 - `nest g module abc`: tao ra folder abc/abcmodule.ts va tu dong import abcmodule vao app.module.ts

### 14: Introduction to NestJs prodivers and services
- prodiver co the duoc inject vao constructor neu provider duoc khai bao @Injectable()
- prividers co the la class, plain valude, sync,async factory
- providers co the export tu module nay, va duoc module khac import vao
- Service la gi? >>> duoc dinh nghia nhu la 1 provider, NOT all prodivers are services
- class duoc @Injectable() deu la SINGLETON
- **Class duoc @Injectable() se duoc import vao module, >>> tu do controller co the su dung service o constructor theo Dependency injection**
- 


