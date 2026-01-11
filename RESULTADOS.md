# 📊 Análisis de Consultas SQL


## 📈 Resumen
✅ 11 correctas de 17 queries

## ✅ Query 1: Correcto

⏱ Tiempo: 0.45 ms
🔍 No se usó ningún índice en esta consulta.

---

## ✅ Query 2: Correcto

⏱ Tiempo: 0.34 ms
🔍 No se usó ningún índice en esta consulta.

---

## ✅ Query 3: Correcto

⏱ Tiempo: 0.34 ms
🔍 No se usó ningún índice en esta consulta.

---

## ❌ Query 4: Incorrecto
```diff
--- 
+++ 
@@ -1,3 +1,3 @@
-nombre | apellido1 | apellido2 | nif
+nombre | apellido1 | apellido2 | NIF
 Antonio | Fahey | Considine | 10485008K
 Guillermo | Ruecker | Upton | 85869555K
```

⏱ Tiempo: 0.35 ms
🔍 No se usó ningún índice en esta consulta.

---

## ✅ Query 5: Correcto

⏱ Tiempo: 0.40 ms
✅ Se usó índice(s) en la consulta: id_grado

---

## ✅ Query 6: Correcto

⏱ Tiempo: 0.42 ms
✅ Se usó índice(s) en la consulta: PRIMARY,id_departamento, PRIMARY

---

## ❌ Query 7: Incorrecto
```diff
--- 
+++ 
@@ -1,4 +1,4 @@
 nombre | anyo_inicio | anyo_fin
 Álgegra lineal y matemática discreta | 2014.00 | 2015.00
-Cálculo | 2014.00 | 2015.00
-Física para informática | 2014.00 | 2015.00
+Cálculo | 2015.00 | 2016.00
+Física para informática | 2016.00 | 2017.00
```

⏱ Tiempo: 0.51 ms
✅ Se usó índice(s) en la consulta: PRIMARY,nif, PRIMARY, PRIMARY,id_asignatura

---

## ✅ Query 8: Correcto

⏱ Tiempo: 0.44 ms
✅ Se usó índice(s) en la consulta: id_profesor,id_grado, PRIMARY,id_departamento, PRIMARY

---

## ✅ Query 9: Correcto

⏱ Tiempo: 0.40 ms
✅ Se usó índice(s) en la consulta: PRIMARY,id_curso_escolar, PRIMARY

---

## ❌ Query 10: Incorrecto
```diff
--- 
+++ 
@@ -1,13 +1,13 @@
 departamento | apellido1 | apellido2 | nombre
 Agronomía | Monahan | Murray | Micaela
+Economía y Empresa | Lemke | Rutherford | Cristina
 Economía y Empresa | Fahey | Considine | Antonio
-Economía y Empresa | Lemke | Rutherford | Cristina
-Educación | Ruecker | Upton | Guillermo
 Educación | Spencer | Lakin | Esther
 Educación | Streich | Hirthe | Carmen
+Educación | Ruecker | Upton | Guillermo
+Informática | Ramirez | Gea | Zoe
 Informática | Hamill | Kozey | Manolo
-Informática | Ramirez | Gea | Zoe
+Matemáticas | Schmidt | Fisher | David
 Matemáticas | Kohler | Schoen | Alejandro
-Matemáticas | Schmidt | Fisher | David
+Química y Física | Stiedemann | Morissette | Alfredo
 Química y Física | Schowalter | Muller | Francesca
-Química y Física | Stiedemann | Morissette | Alfredo
```

⏱ Tiempo: 0.44 ms
✅ Se usó índice(s) en la consulta: PRIMARY

---

## ✅ Query 11: Correcto

⏱ Tiempo: 0.37 ms
✅ Se usó índice(s) en la consulta: PRIMARY

---

## ✅ Query 12: Correcto

⏱ Tiempo: 0.35 ms
✅ Se usó índice(s) en la consulta: id_departamento

---

## ✅ Query 13: Correcto

⏱ Tiempo: 0.38 ms
✅ Se usó índice(s) en la consulta: id_profesor, PRIMARY

---

## ✅ Query 14: Correcto

⏱ Tiempo: 0.36 ms
✅ Se usó índice(s) en la consulta: PRIMARY

---

## ❌ Query 15: Error
- **Descripción**: 1064 (42000): You have an error in your SQL syntax; check the manual that corresponds to your MySQL server version for the right syntax to use near 'SELECT count(*) AS total
FROM persona
WHERE tipo='alumno'' at line 9


## ❌ Query 16: Incorrecto
```diff
--- 
+++ 
@@ -1,2 +1,2 @@
 total
-12.00
+2.00
```

⏱ Tiempo: 0.35 ms
🔍 No se usó ningún índice en esta consulta.

---

## ❌ Query 17: Error
- **Descripción**: 'NoneType' object is not iterable

