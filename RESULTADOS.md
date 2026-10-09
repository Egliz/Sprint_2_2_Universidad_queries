# 📊 Análisis de Consultas SQL


## 📈 Resumen
✅ 25 correctas de 26 queries

## ✅ Query 1: Correcto

⏱ Tiempo: 0.28 ms
🔍 No se usó ningún índice en esta consulta.

---

## ✅ Query 2: Correcto

⏱ Tiempo: 0.14 ms
🔍 No se usó ningún índice en esta consulta.

---

## ✅ Query 3: Correcto

⏱ Tiempo: 0.13 ms
🔍 No se usó ningún índice en esta consulta.

---

## ✅ Query 4: Correcto

⏱ Tiempo: 0.12 ms
🔍 No se usó ningún índice en esta consulta.

---

## ✅ Query 5: Correcto

⏱ Tiempo: 0.16 ms
✅ Se usó índice(s) en la consulta: id_grado

---

## ✅ Query 6: Correcto

⏱ Tiempo: 0.21 ms
✅ Se usó índice(s) en la consulta: PRIMARY, PRIMARY,id_departamento

---

## ✅ Query 7: Correcto

⏱ Tiempo: 0.29 ms
✅ Se usó índice(s) en la consulta: PRIMARY, PRIMARY,id_asignatura,id_curso_escolar, PRIMARY,nif

---

## ✅ Query 8: Correcto

⏱ Tiempo: 0.18 ms
✅ Se usó índice(s) en la consulta: PRIMARY, PRIMARY,id_departamento, id_profesor,id_grado

---

## ✅ Query 9: Correcto

⏱ Tiempo: 0.16 ms
✅ Se usó índice(s) en la consulta: PRIMARY, PRIMARY,id_curso_escolar

---

## ✅ Query 10: Correcto

⏱ Tiempo: 0.17 ms
✅ Se usó índice(s) en la consulta: PRIMARY

---

## ✅ Query 11: Correcto

⏱ Tiempo: 0.13 ms
✅ Se usó índice(s) en la consulta: PRIMARY

---

## ✅ Query 12: Correcto

⏱ Tiempo: 0.12 ms
✅ Se usó índice(s) en la consulta: id_departamento

---

## ✅ Query 13: Correcto

⏱ Tiempo: 0.13 ms
✅ Se usó índice(s) en la consulta: PRIMARY, id_profesor

---

## ✅ Query 14: Correcto

⏱ Tiempo: 0.13 ms
✅ Se usó índice(s) en la consulta: PRIMARY

---

## ✅ Query 15: Correcto

⏱ Tiempo: 0.14 ms
✅ Se usó índice(s) en la consulta: id_asignatura, id_profesor, id_departamento

---

## ✅ Query 16: Correcto

⏱ Tiempo: 0.11 ms
🔍 No se usó ningún índice en esta consulta.

---

## ✅ Query 17: Correcto

⏱ Tiempo: 0.11 ms
🔍 No se usó ningún índice en esta consulta.

---

## ✅ Query 18: Correcto

⏱ Tiempo: 0.13 ms
✅ Se usó índice(s) en la consulta: PRIMARY, id_departamento

---

## ❌ Query 19: Incorrecto
```diff
--- 
+++ 
@@ -1,10 +1,10 @@
 departamento | total
+Educación | 3.00
+Economía y Empresa | 2.00
 Informática | 2.00
 Matemáticas | 2.00
-Economía y Empresa | 2.00
-Educación | 3.00
+Química y Física | 2.00
 Agronomía | 1.00
-Química y Física | 2.00
+Biología y Geología | 0.00
+Derecho | 0.00
 Filología | 0.00
-Derecho | 0.00
-Biología y Geología | 0.00
```

⏱ Tiempo: 0.14 ms
✅ Se usó índice(s) en la consulta: id_departamento

---

## ✅ Query 20: Correcto

⏱ Tiempo: 0.12 ms
✅ Se usó índice(s) en la consulta: id_grado

---

## ✅ Query 21: Correcto

⏱ Tiempo: 0.13 ms
✅ Se usó índice(s) en la consulta: id_grado

---

## ✅ Query 22: Correcto

⏱ Tiempo: 0.13 ms
✅ Se usó índice(s) en la consulta: PRIMARY, id_grado

---

## ✅ Query 23: Correcto

⏱ Tiempo: 0.14 ms
✅ Se usó índice(s) en la consulta: PRIMARY, id_curso_escolar

---

## ✅ Query 24: Correcto

⏱ Tiempo: 0.15 ms
✅ Se usó índice(s) en la consulta: PRIMARY, id_profesor

---

## ✅ Query 25: Correcto

⏱ Tiempo: 0.12 ms
🔍 No se usó ningún índice en esta consulta.

🚨 **Problemas detectados:**
⚠️ Evitar `SELECT *`. Usar solo las columnas necesarias.

---

## ✅ Query 26: Correcto

⏱ Tiempo: 0.14 ms
✅ Se usó índice(s) en la consulta: PRIMARY, id_profesor, PRIMARY,id_departamento

---
