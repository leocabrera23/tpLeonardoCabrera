---
# Trabajo Practico N° 1

### Alumno: Leonardo Cabrera

### Curso: 2°1°

### Materia: Programación

### Profesor: Alberto Cortez

### IES Manuel Belgrano (ciudad)
---


## Consignas   
#### 1- Crear con sequelize una base de datos con sus relaciones 

#### 2- Exportala a workbench

#### 3- Generar un gráfico de entidad relación con la herramienta de ingeniería inversa
---



## _Comandos para la creación de las tablas_

### sin clave foránea:

```
sequelize model:generate --name Brand --attributes name:string

sequelize model:generate --name Color --attributes name:string

sequelize model:generate --name User --attributes firstName:string,lastName:string,email:string,password:string

sequelize model:generate --name Category --attributes name:string
```
### con clave foránea:

```
sequelize model:generate --name Product --attributes name:string,description:text,price:decimal,image:string,keywords:text,userId:integer,brandId:integer

sequelize model:generate --name ColorProduct --attributes productId:integer,colorId:integer

sequelize model:generate --name CategoryProduct --attributes productId:integer,categoryId:integer
```
---


<h2 align="center">Gráfico</h2>
 
<p align="center">
  <img 
 src="https://user-images.githubusercontent.com/83379102/122651691-d2b9b580-d110-11eb-95cf-ea79e958ffdb.png"/>
</p>




