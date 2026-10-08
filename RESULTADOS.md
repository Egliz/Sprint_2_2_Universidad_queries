# 📊 Análisis de Consultas SQL


## 📈 Resumen
✅ 0 correctas de 8 queries

## ❌ Query 1: Incorrecto
```diff
--- 
+++ 
@@ -1,13 +1,25 @@
 apellido1 | apellido2 | nombre
 Domínguez | Guerrero | Antonio
+Fahey | Considine | Antonio
 Gea | Ruiz | Sonia
 Gutiérrez | López | Juan
+Hamill | Kozey | Manolo
 Heller | Pagac | Pedro
 Herman | Pacocha | Daniel
 Hernández | Martínez | Irene
 Herzog | Tremblay | Ramón
+Kohler | Schoen | Alejandro
 Koss | Bayer | José
 Lakin | Yundt | Inma
+Lemke | Rutherford | Cristina
+Monahan | Murray | Micaela
+Ramirez | Gea | Zoe
+Ruecker | Upton | Guillermo
 Saez | Vega | Juan
 Sánchez | Pérez | Salvador
+Schmidt | Fisher | David
+Schowalter | Muller | Francesca
+Spencer | Lakin | Esther
+Stiedemann | Morissette | Alfredo
+Streich | Hirthe | Carmen
 Strosin | Turcotte | Ismael
```

⏱ Tiempo: 0.45 ms
🔍 No se usó ningún índice en esta consulta.

---

## ❌ Query 2: Error
- **Descripción**: 1064 (42000): You have an error in your SQL syntax; check the manual that corresponds to your MySQL server version for the right syntax to use near ':

-- 3. Retorna el llistat dels alumnes que van néixer en 1999. (id, nombre, a' at line 6


## ❌ Query 3: Incorrecto
```diff
--- 
+++ 
@@ -1,3 +1,4 @@
-id | nombre | apellido1 | apellido2 | fecha_nacimiento
-7.00 | Ismael | Strosin | Turcotte | 1999-05-24
-22.00 | Antonio | Domínguez | Guerrero | 1999-02-11
+nombre | apellido1 | apellido2 | nif
+Ismael | Strosin | Turcotte | 97258166K
+Antonio | Fahey | Considine | 10485008K
+Guillermo | Ruecker | Upton | 85869555K
```

⏱ Tiempo: 0.31 ms
🔍 No se usó ningún índice en esta consulta.

---

## ❌ Query 4: Incorrecto
```diff
--- 
+++ 
@@ -1,3 +1,7 @@
-nombre | apellido1 | apellido2 | nif
-Antonio | Fahey | Considine | 10485008K
-Guillermo | Ruecker | Upton | 85869555K
+id | nombre | cuatrimestre | curso | id_grado
+72.00 | Bases moleculares del desarrollo vegetal | 1.00 | 3.00 | 7.00
+73.00 | Fisiología animal | 1.00 | 3.00 | 7.00
+74.00 | Metabolismo y biosíntesis de biomoléculas | 1.00 | 3.00 | 7.00
+75.00 | Operaciones de separación | 1.00 | 3.00 | 7.00
+76.00 | Patología molecular de plantas | 1.00 | 3.00 | 7.00
+77.00 | Técnicas instrumentales básicas | 1.00 | 3.00 | 7.00
```

⏱ Tiempo: 0.34 ms
✅ Se usó índice(s) en la consulta: id_grado

---

## ❌ Query 5: Incorrecto
```diff
--- 
+++ 
@@ -1,7 +1,13 @@
-id | nombre | cuatrimestre | curso | id_grado
-72.00 | Bases moleculares del desarrollo vegetal | 1.00 | 3.00 | 7.00
-73.00 | Fisiología animal | 1.00 | 3.00 | 7.00
-74.00 | Metabolismo y biosíntesis de biomoléculas | 1.00 | 3.00 | 7.00
-75.00 | Operaciones de separación | 1.00 | 3.00 | 7.00
-76.00 | Patología molecular de plantas | 1.00 | 3.00 | 7.00
-77.00 | Técnicas instrumentales básicas | 1.00 | 3.00 | 7.00
+apellido1 | apellido2 | nombre | departamento
+Fahey | Considine | Antonio | Economía y Empresa
+Hamill | Kozey | Manolo | Informática
+Kohler | Schoen | Alejandro | Matemáticas
+Lemke | Rutherford | Cristina | Economía y Empresa
+Monahan | Murray | Micaela | Agronomía
+Ramirez | Gea | Zoe | Informática
+Ruecker | Upton | Guillermo | Educación
+Schmidt | Fisher | David | Matemáticas
+Schowalter | Muller | Francesca | Química y Física
+Spencer | Lakin | Esther | Educación
+Stiedemann | Morissette | Alfredo | Química y Física
+Streich | Hirthe | Carmen | Educación
```

⏱ Tiempo: 0.40 ms
✅ Se usó índice(s) en la consulta: PRIMARY, PRIMARY,id_departamento

---

## ❌ Query 6: Incorrecto
```diff
--- 
+++ 
@@ -1,13 +1,4 @@
-apellido1 | apellido2 | nombre | departamento
-Fahey | Considine | Antonio | Economía y Empresa
-Hamill | Kozey | Manolo | Informática
-Kohler | Schoen | Alejandro | Matemáticas
-Lemke | Rutherford | Cristina | Economía y Empresa
-Monahan | Murray | Micaela | Agronomía
-Ramirez | Gea | Zoe | Informática
-Ruecker | Upton | Guillermo | Educación
-Schmidt | Fisher | David | Matemáticas
-Schowalter | Muller | Francesca | Química y Física
-Spencer | Lakin | Esther | Educación
-Stiedemann | Morissette | Alfredo | Química y Física
-Streich | Hirthe | Carmen | Educación
+nombre | anyo_inicio | anyo_fin
+Álgegra lineal y matemática discreta | 2014.00 | 2015.00
+Cálculo | 2014.00 | 2015.00
+Física para informática | 2014.00 | 2015.00
```

⏱ Tiempo: 0.49 ms
✅ Se usó índice(s) en la consulta: PRIMARY,id_asignatura,id_curso_escolar, PRIMARY, PRIMARY,nif

---

## ❌ Query 7: Incorrecto
```diff
--- 
+++ 
@@ -1,4 +1,2 @@
-nombre | anyo_inicio | anyo_fin
-Álgegra lineal y matemática discreta | 2014.00 | 2015.00
-Cálculo | 2014.00 | 2015.00
-Física para informática | 2014.00 | 2015.00
+nombre
+Informática
```

⏱ Tiempo: 0.34 ms
✅ Se usó índice(s) en la consulta: PRIMARY, PRIMARY,id_departamento, id_profesor,id_grado

---

## ❌ Query 8: Error
- **Descripción**: 'NoneType' object is not iterable

