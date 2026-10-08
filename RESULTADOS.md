# 📊 Análisis de Consultas SQL


## 📈 Resumen
✅ 0 correctas de 4 queries

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

⏱ Tiempo: 0.33 ms
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

⏱ Tiempo: 0.24 ms
🔍 No se usó ningún índice en esta consulta.

---

## ❌ Query 4: Error
- **Descripción**: 'NoneType' object is not iterable

