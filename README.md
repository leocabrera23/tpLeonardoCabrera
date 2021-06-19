#"Trabajo Practico N° 1"#

##"Comandos para la creación de las tablas"##

"sin clave foránea"
sequelize model:generate --name Brand --attributes name:string

sequelize model:generate --name Color --attributes name:string

sequelize model:generate --name User --attributes firstName:string,lastName:string,email:string,password:string

sequelize model:generate --name Category --attributes name:string
 
 "con clave foránea"
sequelize model:generate --name Product --attributes name:string,description:text,price:decimal,image:string,keywords:text,userId:integer,brandId:integer

sequelize model:generate --name ColorProduct --attributes productId:integer,colorId:integer

sequelize model:generate --name CategoryProduct --attributes productId:integer,categoryId:integer

![image](https://user-images.githubusercontent.com/83379102/122650418-33dd8b00-d109-11eb-8c3a-ef0e0f41eb90.png)
![image](https://user-images.githubusercontent.com/83379102/122650427-43f56a80-d109-11eb-9fb2-af90b2bca114.png)

Materia: Programación 

Alumno: Leonardo Cabrera

Profesor: Alberto Cortez
