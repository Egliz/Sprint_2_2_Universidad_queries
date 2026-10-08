# 📊 Análisis de Consultas SQL


## 📈 Resumen
✅ 0 correctas de 18 queries

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

⏱ Tiempo: 0.31 ms
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

⏱ Tiempo: 0.22 ms
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

⏱ Tiempo: 0.26 ms
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

⏱ Tiempo: 0.34 ms
✅ Se usó índice(s) en la consulta: PRIMARY,id_departamento, PRIMARY

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

⏱ Tiempo: 0.43 ms
✅ Se usó índice(s) en la consulta: PRIMARY, PRIMARY,nif, PRIMARY,id_asignatura,id_curso_escolar

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

⏱ Tiempo: 0.27 ms
✅ Se usó índice(s) en la consulta: PRIMARY,id_departamento, PRIMARY, id_profesor,id_grado

---

## ❌ Query 8: Incorrecto
```diff
--- 
+++ 
@@ -1,2 +1,4 @@
-nombre
-Informática
+nombre | apellido1 | apellido2
+Inma | Lakin | Yundt
+Irene | Hernández | Martínez
+Sonia | Gea | Ruiz
```

⏱ Tiempo: 0.27 ms
✅ Se usó índice(s) en la consulta: PRIMARY, PRIMARY,id_curso_escolar

---

## ❌ Query 9: Incorrecto
```diff
--- 
+++ 
@@ -1,4 +1,13 @@
-nombre | apellido1 | apellido2
-Inma | Lakin | Yundt
-Irene | Hernández | Martínez
-Sonia | Gea | Ruiz
+departamento | apellido1 | apellido2 | nombre
+Agronomía | Monahan | Murray | Micaela
+Economía y Empresa | Fahey | Considine | Antonio
+Economía y Empresa | Lemke | Rutherford | Cristina
+Educación | Ruecker | Upton | Guillermo
+Educación | Spencer | Lakin | Esther
+Educación | Streich | Hirthe | Carmen
+Informática | Hamill | Kozey | Manolo
+Informática | Ramirez | Gea | Zoe
+Matemáticas | Kohler | Schoen | Alejandro
+Matemáticas | Schmidt | Fisher | David
+Química y Física | Schowalter | Muller | Francesca
+Química y Física | Stiedemann | Morissette | Alfredo
```

⏱ Tiempo: 0.28 ms
✅ Se usó índice(s) en la consulta: PRIMARY

---

## ❌ Query 10: Incorrecto
```diff
--- 
+++ 
@@ -1,13 +1 @@
-departamento | apellido1 | apellido2 | nombre
-Agronomía | Monahan | Murray | Micaela
-Economía y Empresa | Fahey | Considine | Antonio
-Economía y Empresa | Lemke | Rutherford | Cristina
-Educación | Ruecker | Upton | Guillermo
-Educación | Spencer | Lakin | Esther
-Educación | Streich | Hirthe | Carmen
-Informática | Hamill | Kozey | Manolo
-Informática | Ramirez | Gea | Zoe
-Matemáticas | Kohler | Schoen | Alejandro
-Matemáticas | Schmidt | Fisher | David
-Química y Física | Schowalter | Muller | Francesca
-Química y Física | Stiedemann | Morissette | Alfredo
+apellido1 | apellido2 | nombre
```

⏱ Tiempo: 0.24 ms
✅ Se usó índice(s) en la consulta: PRIMARY

---

## ❌ Query 11: Incorrecto
```diff
--- 
+++ 
@@ -1 +1,4 @@
-apellido1 | apellido2 | nombre
+nombre
+Filología
+Derecho
+Biología y Geología
```

⏱ Tiempo: 0.21 ms
✅ Se usó índice(s) en la consulta: id_departamento

---

## ❌ Query 12: Incorrecto
```diff
--- 
+++ 
@@ -1,4 +1,11 @@
-nombre
-Filología
-Derecho
-Biología y Geología
+apellido1 | apellido2 | nombre
+Schmidt | Fisher | David
+Kohler | Schoen | Alejandro
+Lemke | Rutherford | Cristina
+Fahey | Considine | Antonio
+Spencer | Lakin | Esther
+Streich | Hirthe | Carmen
+Ruecker | Upton | Guillermo
+Monahan | Murray | Micaela
+Stiedemann | Morissette | Alfredo
+Schowalter | Muller | Francesca
```

⏱ Tiempo: 0.25 ms
✅ Se usó índice(s) en la consulta: PRIMARY, id_profesor

---

## ❌ Query 13: Incorrecto
```diff
--- 
+++ 
@@ -1,11 +1,63 @@
-apellido1 | apellido2 | nombre
-Schmidt | Fisher | David
-Kohler | Schoen | Alejandro
-Lemke | Rutherford | Cristina
-Fahey | Considine | Antonio
-Spencer | Lakin | Esther
-Streich | Hirthe | Carmen
-Ruecker | Upton | Guillermo
-Monahan | Murray | Micaela
-Stiedemann | Morissette | Alfredo
-Schowalter | Muller | Francesca
+id | nombre
+22.00 | Ingeniería de Requisitos
+23.00 | Integración de las Tecnologías de la Información en las Organizaciones
+24.00 | Modelado y Diseño del Software 1
+25.00 | Multiprocesadores
+26.00 | Seguridad y cumplimiento normativo
+27.00 | Sistema de Información para las Organizaciones
+28.00 | Tecnologías web
+29.00 | Teoría de códigos y criptografía
+30.00 | Administración de bases de datos
+31.00 | Herramientas y Métodos de Ingeniería del Software
+32.00 | Informática industrial y robótica
+33.00 | Ingeniería de Sistemas de Información
+34.00 | Modelado y Diseño del Software 2
+35.00 | Negocio Electrónico
+36.00 | Periféricos e interfaces
+37.00 | Sistemas de tiempo real
+38.00 | Tecnologías de acceso a red
+39.00 | Tratamiento digital de imágenes
+40.00 | Administración de redes y sistemas operativos
+41.00 | Almacenes de Datos
+42.00 | Fiabilidad y Gestión de Riesgos
+43.00 | Líneas de Productos Software
+44.00 | Procesos de Ingeniería del Software 1
+45.00 | Tecnologías multimedia
+46.00 | Análisis y planificación de las TI
+47.00 | Desarrollo Rápido de Aplicaciones
+48.00 | Gestión de la Calidad y de la Innovación Tecnológica
+49.00 | Inteligencia del Negocio
+50.00 | Procesos de Ingeniería del Software 2
+51.00 | Seguridad Informática
+52.00 | Biologia celular
+53.00 | Física
+54.00 | Matemáticas I
+55.00 | Química general
+56.00 | Química orgánica
+57.00 | Biología vegetal y animal
+58.00 | Bioquímica
+59.00 | Genética
+60.00 | Matemáticas II
+61.00 | Microbiología
+62.00 | Botánica agrícola
+63.00 | Fisiología vegetal
+64.00 | Genética molecular
+65.00 | Ingeniería bioquímica
+66.00 | Termodinámica y cinética química aplicada
+67.00 | Biorreactores
+68.00 | Biotecnología microbiana
+69.00 | Ingeniería genética
+70.00 | Inmunología
+71.00 | Virología
+72.00 | Bases moleculares del desarrollo vegetal
+73.00 | Fisiología animal
+74.00 | Metabolismo y biosíntesis de biomoléculas
+75.00 | Operaciones de separación
+76.00 | Patología molecular de plantas
+77.00 | Técnicas instrumentales básicas
+78.00 | Bioinformática
+79.00 | Biotecnología de los productos hortofrutículas
+80.00 | Biotecnología vegetal
+81.00 | Genómica y proteómica
+82.00 | Procesos biotecnológicos
+83.00 | Técnicas instrumentales avanzadas
```

⏱ Tiempo: 0.22 ms
✅ Se usó índice(s) en la consulta: PRIMARY

---

## ❌ Query 14: Incorrecto
```diff
--- 
+++ 
@@ -1,63 +1,14 @@
-id | nombre
-22.00 | Ingeniería de Requisitos
-23.00 | Integración de las Tecnologías de la Información en las Organizaciones
-24.00 | Modelado y Diseño del Software 1
-25.00 | Multiprocesadores
-26.00 | Seguridad y cumplimiento normativo
-27.00 | Sistema de Información para las Organizaciones
-28.00 | Tecnologías web
-29.00 | Teoría de códigos y criptografía
-30.00 | Administración de bases de datos
-31.00 | Herramientas y Métodos de Ingeniería del Software
-32.00 | Informática industrial y robótica
-33.00 | Ingeniería de Sistemas de Información
-34.00 | Modelado y Diseño del Software 2
-35.00 | Negocio Electrónico
-36.00 | Periféricos e interfaces
-37.00 | Sistemas de tiempo real
-38.00 | Tecnologías de acceso a red
-39.00 | Tratamiento digital de imágenes
-40.00 | Administración de redes y sistemas operativos
-41.00 | Almacenes de Datos
-42.00 | Fiabilidad y Gestión de Riesgos
-43.00 | Líneas de Productos Software
-44.00 | Procesos de Ingeniería del Software 1
-45.00 | Tecnologías multimedia
-46.00 | Análisis y planificación de las TI
-47.00 | Desarrollo Rápido de Aplicaciones
-48.00 | Gestión de la Calidad y de la Innovación Tecnológica
-49.00 | Inteligencia del Negocio
-50.00 | Procesos de Ingeniería del Software 2
-51.00 | Seguridad Informática
-52.00 | Biologia celular
-53.00 | Física
-54.00 | Matemáticas I
-55.00 | Química general
-56.00 | Química orgánica
-57.00 | Biología vegetal y animal
-58.00 | Bioquímica
-59.00 | Genética
-60.00 | Matemáticas II
-61.00 | Microbiología
-62.00 | Botánica agrícola
-63.00 | Fisiología vegetal
-64.00 | Genética molecular
-65.00 | Ingeniería bioquímica
-66.00 | Termodinámica y cinética química aplicada
-67.00 | Biorreactores
-68.00 | Biotecnología microbiana
-69.00 | Ingeniería genética
-70.00 | Inmunología
-71.00 | Virología
-72.00 | Bases moleculares del desarrollo vegetal
-73.00 | Fisiología animal
-74.00 | Metabolismo y biosíntesis de biomoléculas
-75.00 | Operaciones de separación
-76.00 | Patología molecular de plantas
-77.00 | Técnicas instrumentales básicas
-78.00 | Bioinformática
-79.00 | Biotecnología de los productos hortofrutículas
-80.00 | Biotecnología vegetal
-81.00 | Genómica y proteómica
-82.00 | Procesos biotecnológicos
-83.00 | Técnicas instrumentales avanzadas
+nombre
+Matemáticas
+Matemáticas
+Economía y Empresa
+Economía y Empresa
+Educación
+Educación
+Educación
+Agronomía
+Química y Física
+Química y Física
+Filología
+Derecho
+Biología y Geología
```

⏱ Tiempo: 0.22 ms
✅ Se usó índice(s) en la consulta: id_profesor, id_departamento

---

## ❌ Query 15: Incorrecto
```diff
--- 
+++ 
@@ -1,10 +1,2 @@
-nombre
-Informática
-Matemáticas
-Economía y Empresa
-Educación
-Agronomía
-Química y Física
-Filología
-Derecho
-Biología y Geología
+total
+12.00
```

⏱ Tiempo: 0.20 ms
🔍 No se usó ningún índice en esta consulta.

---

## ❌ Query 16: Incorrecto
```diff
--- 
+++ 
@@ -1,2 +1,2 @@
 total
-12.00
+2.00
```

⏱ Tiempo: 0.21 ms
🔍 No se usó ningún índice en esta consulta.

---

## ❌ Query 17: Incorrecto
```diff
--- 
+++ 
@@ -1,2 +1,7 @@
-total
-2.00
+departamento | total
+Educación | 3.00
+Informática | 2.00
+Matemáticas | 2.00
+Economía y Empresa | 2.00
+Química y Física | 2.00
+Agronomía | 1.00
```

⏱ Tiempo: 0.24 ms
✅ Se usó índice(s) en la consulta: PRIMARY, id_departamento

---

## ❌ Query 18: Error
- **Descripción**: 'NoneType' object is not iterable

