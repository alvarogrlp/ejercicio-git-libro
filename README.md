# Ejercicio Libro

**1. Primero usamos el comando**

```bash
mkdir capitulos
```
Con esto creamos las carpeta y añadimos el primer documento .txt que en mi caso lo hice desde el VS Code.


**2. Añadimos los cambios y lo comentamos**

```bash
git add .
git commit -m "Añadido capítulo 1."
git log
```
En mi caso el log que me da como resultado es el log final ya que me olvidé de hacerlo meidante iba realizando los pasos.

**3. Hacemos lo mismo con el capitulo 2**

```bash
git add .
git commit -m "Añadido capítulo 2."
git diff HEAD~2..HEAD
```
Este es el resultado del diff:
```bash
diff --git a/capitulos/bibliografia b/capitulos/bibliografia
new file mode 100644
index 0000000..c90a592
--- /dev/null
+++ b/capitulos/bibliografia
@@ -0,0 +1,2 @@
+# Hacer los cambios indicados en el fichero
+
diff --git a/bibliografia.txt b/capitulos/bibliografia.txt
similarity index 100%
rename from bibliografia.txt
rename to capitulos/bibliografia.txt
diff --git a/capitulo1.txt b/capitulos/capitulo1.txt
similarity index 100%
rename from capitulo1.txt
rename to capitulos/capitulo1.txt
diff --git a/capitulo2.txt b/capitulos/capitulo2.txt
similarity index 100%
rename from capitulo2.txt
rename to capitulos/capitulo2.txt
diff --git a/capitulo3.txt b/capitulos/capitulo3.txt
similarity index 100%
rename from capitulo3.txt
rename to capitulos/capitulo3.txt
diff --git a/capitulo4.txt b/capitulos/capitulo4.txt
similarity index 100%
rename from capitulo4.txt
rename to capitulos/capitulo4.txt
diff --git "a/\303\255ndice.txt" "b/capitulos/\303\255ndice.txt"
similarity index 100%
rename from "\303\255ndice.txt"
rename to "capitulos/\303\255ndice.txt"
(END)
```

**4. Repetimos los mismo con el capitulo 4**

```bash
git add .
git commit -m "Añadido capítulo 3."
git log
git diff ed192fbd6654e7ed4bd03c6c11e41cb87daf7fb8..HEAD
```
Este es el resultado final del log:

```bash
commit ed192fbd6654e7ed4bd03c6c11e41cb87daf7fb8 (HEAD -> main, origin/main, origin/HEAD)
Author: alvarogrlp <alvarogarciaprof@gmail.com>
Date:   Mon Oct 14 16:09:48 2024 +0100

    Añado los archivos a la carpeta

commit ddf0e9a0ddfaa91e89391e810ac946f92213d216
Author: alvarogrlp <alvarogarciaprof@gmail.com>
Date:   Mon Oct 14 15:41:10 2024 +0100

    Solucionado conflicto bibliografía.

commit 4951d4f791b2e38055960a833ebb41fe81bab4ec
Merge: c6349ff a66d104
Author: alvarogrlp <alvarogarciaprof@gmail.com>
Date:   Thu Oct 10 18:47:25 2024 +0100

    Solucionado conflicto bibliografía.

commit c6349ff9025dc507ff4b2b209f31312161c11b74
Author: alvarogrlp <alvarogarciaprof@gmail.com>
Date:   Thu Oct 10 18:45:58 2024 +0100

    Añadida nueva referencia bibliográfica.

commit a66d1040a56e7bea50b250dedb4cf19beac44f35 (bibliografia)
Author: alvarogrlp <alvarogarciaprof@gmail.com>
Date:   Thu Oct 10 18:44:23 2024 +0100

    Añadida nueva referencia bibliográfica.

commit 6682e0bd1b5b1eb06f935b82799e1ec08bd115f6
Merge: 9fa5aa8 8ef7835
Author: alvarogrlp <alvarogarciaprof@gmail.com>
Date:   Thu Oct 10 18:35:37 2024 +0100

    Añadida primera referencia bibliográfica.

commit 9fa5aa851bc0a4dd97089a72282d61857eda024c
Author: alvarogrlp <alvarogarciaprof@gmail.com>
Date:   Thu Oct 10 18:33:18 2024 +0100

    Añadida primera referencia bibliográfica.

commit 8ef7835008ee3c8338809eb0608413a1a278b468
Author: alvarogrlp <alvarogarciaprof@gmail.com>
Date:   Thu Oct 10 18:28:26 2024 +0100

    Añadido el capitulo4.txt

commit 2c507dc9a211537982dab2f6ad331a6c938cb887
Author: alvarogrlp <alvarogarciaprof@gmail.com>
Date:   Thu Oct 10 18:25:42 2024 +0100

    Añado el índice.txt

commit 3d84094babad99a2c16733d349328893d6fda9bd
Author: alvarogrlp <alvarogarciaprof@gmail.com>
Date:   Thu Oct 10 18:19:29 2024 +0100

    Añado el nuevo capitulo3.txt

commit 5371baf13991a78dab8a655cbaef1501284cd4c3
Author: alvarogrlp <alvarogarciaprof@gmail.com>
Date:   Thu Oct 10 18:15:36 2024 +0100

    Añado el capitulo2.txt con el contenido

commit a9e8ef905f3914f9ce3501d36c33e482633ff0b7
Author: alvarogrlp <alvarogarciaprof@gmail.com>
Date:   Thu Oct 10 18:12:23 2024 +0100

    Modifico el capitulo1.txt por un error

commit 0b22acf1631b9c58c31a5f4ee938ea0c4b9e1c0f
Author: alvarogrlp <alvarogarciaprof@gmail.com>
Date:   Thu Oct 10 18:10:57 2024 +0100

    Añadimos el capitulo1.txt

commit 8445bbce8a98b0d5be7ce3bd836fef3cd91df14e
Author: alvarogrlp <alvarogarciaprof@gmail.com>
Date:   Thu Oct 10 18:02:09 2024 +0100

    Initial commit
(END)
```

Y este es el resultado del diff:

```bash
diff --git a/README.md b/README.md
index 9a06b52..c50379a 100644
--- a/README.md
+++ b/README.md
@@ -1 +1,257 @@
-# ejercicio-git-libro
\ No newline at end of file
+# Ejercicio Libro
+
+**1. Primero usamos el comando**
+
+```bash
+mkdir capitulos
+```
+Con esto creamos las carpeta y añadimos el primer documento .txt que en mi caso lo hice desde el VS Code.
+
+
+**2. Añadimos los cambios y lo comentamos**
+
+```bash
+git add .
+git commit -m "Añadido capítulo 1."
+git log
+```
+En mi caso el log que me da como resultado es el log final ya que me olvidé de hacerlo meidante iba realizando los pasos.
+
+**3. Hacemos lo mismo con el capitulo 2**
+
+```bash
+git add .
+git commit -m "Añadido capítulo 2."
+git diff HEAD~2..HEAD
+```
+Este es el resultado del diff:
+```bash
+diff --git a/capitulos/bibliografia b/capitulos/bibliografia
+new file mode 100644
+index 0000000..c90a592
+--- /dev/null
++++ b/capitulos/bibliografia
+@@ -0,0 +1,2 @@
++# Hacer los cambios indicados en el fichero
++
+diff --git a/bibliografia.txt b/capitulos/bibliografia.txt
+similarity index 100%
+rename from bibliografia.txt
+rename to capitulos/bibliografia.txt
+diff --git a/capitulo1.txt b/capitulos/capitulo1.txt
+similarity index 100%
+rename from capitulo1.txt
+rename to capitulos/capitulo1.txt
+diff --git a/capitulo2.txt b/capitulos/capitulo2.txt
+similarity index 100%
+rename from capitulo2.txt
+rename to capitulos/capitulo2.txt
+diff --git a/capitulo3.txt b/capitulos/capitulo3.txt
+similarity index 100%
+rename from capitulo3.txt
+rename to capitulos/capitulo3.txt
+diff --git a/capitulo4.txt b/capitulos/capitulo4.txt
+similarity index 100%
+rename from capitulo4.txt
+rename to capitulos/capitulo4.txt
+diff --git "a/\303\255ndice.txt" "b/capitulos/\303\255ndice.txt"
+similarity index 100%
+rename from "\303\255ndice.txt"
+rename to "capitulos/\303\255ndice.txt"
+(END)
+```
+
+**4. Repetimos los mismo con el capitulo 4**
+
+```bash
+git add .
+git commit -m "Añadido capítulo 3."
+git log
+git diff ed192fbd6654e7ed4bd03c6c11e41cb87daf7fb8..HEAD
+```
+Este es el resultado final del log:
+
+```bash
+commit ed192fbd6654e7ed4bd03c6c11e41cb87daf7fb8 (HEAD -> main, origin/main, origin/HEAD)
+Author: alvarogrlp <alvarogarciaprof@gmail.com>
+Date:   Mon Oct 14 16:09:48 2024 +0100
+
+    Añado los archivos a la carpeta
+
+commit ddf0e9a0ddfaa91e89391e810ac946f92213d216
+Author: alvarogrlp <alvarogarciaprof@gmail.com>
+Date:   Mon Oct 14 15:41:10 2024 +0100
+
+    Solucionado conflicto bibliografía.
+
+commit 4951d4f791b2e38055960a833ebb41fe81bab4ec
+Merge: c6349ff a66d104
+Author: alvarogrlp <alvarogarciaprof@gmail.com>
+Date:   Thu Oct 10 18:47:25 2024 +0100
+
+    Solucionado conflicto bibliografía.
+
+commit c6349ff9025dc507ff4b2b209f31312161c11b74
+Author: alvarogrlp <alvarogarciaprof@gmail.com>
+Date:   Thu Oct 10 18:45:58 2024 +0100
+
+    Añadida nueva referencia bibliográfica.
+
+commit a66d1040a56e7bea50b250dedb4cf19beac44f35 (bibliografia)
+Author: alvarogrlp <alvarogarciaprof@gmail.com>
+Date:   Thu Oct 10 18:44:23 2024 +0100
+
+    Añadida nueva referencia bibliográfica.
+
+commit 6682e0bd1b5b1eb06f935b82799e1ec08bd115f6
+Merge: 9fa5aa8 8ef7835
+Author: alvarogrlp <alvarogarciaprof@gmail.com>
+Date:   Thu Oct 10 18:35:37 2024 +0100
+
+    Añadida primera referencia bibliográfica.
+
+commit 9fa5aa851bc0a4dd97089a72282d61857eda024c
+Author: alvarogrlp <alvarogarciaprof@gmail.com>
+Date:   Thu Oct 10 18:33:18 2024 +0100
+
+    Añadida primera referencia bibliográfica.
+
+commit 8ef7835008ee3c8338809eb0608413a1a278b468
+Author: alvarogrlp <alvarogarciaprof@gmail.com>
+Date:   Thu Oct 10 18:28:26 2024 +0100
+
+    Añadido el capitulo4.txt
+
+commit 2c507dc9a211537982dab2f6ad331a6c938cb887
+Author: alvarogrlp <alvarogarciaprof@gmail.com>
+Date:   Thu Oct 10 18:25:42 2024 +0100
+
+    Añado el índice.txt
+
+commit 3d84094babad99a2c16733d349328893d6fda9bd
+Author: alvarogrlp <alvarogarciaprof@gmail.com>
+Date:   Thu Oct 10 18:19:29 2024 +0100
+
+    Añado el nuevo capitulo3.txt
+
+commit 5371baf13991a78dab8a655cbaef1501284cd4c3
+Author: alvarogrlp <alvarogarciaprof@gmail.com>
+Date:   Thu Oct 10 18:15:36 2024 +0100
+
+    Añado el capitulo2.txt con el contenido
+
+commit a9e8ef905f3914f9ce3501d36c33e482633ff0b7
+Author: alvarogrlp <alvarogarciaprof@gmail.com>
+Date:   Thu Oct 10 18:12:23 2024 +0100
+
+    Modifico el capitulo1.txt por un error
+
+commit 0b22acf1631b9c58c31a5f4ee938ea0c4b9e1c0f
+Author: alvarogrlp <alvarogarciaprof@gmail.com>
+Date:   Thu Oct 10 18:10:57 2024 +0100
+
+    Añadimos el capitulo1.txt
+
+commit 8445bbce8a98b0d5be7ce3bd836fef3cd91df14e
+Author: alvarogrlp <alvarogarciaprof@gmail.com>
+Date:   Thu Oct 10 18:02:09 2024 +0100
+
+    Initial commit
+(END)
+```
+
+**5. Añadimos el indice**
+
+```bash
+git add .
+git commit -m "Se crea el indice."
+echo "Indice de los cápitulos, con conceptos avanzados de git" >> indice.xt
+git add .
+git commit -m "Añadido el índice ."
+git annotate indice.txt
+```
+
+**6. Ahora vamos a crear la nueva rama**
+
+```bash
+git branch bibliografia
+git branch -av
+```
+
+**7. Creo el fichero 4**
+
+```bash
+git add .
+git commit -m "Añadido capítulo 4."
+git log --graph --all --oneline
+```
+Este es el resultado del log final como comenté antes
+
+```bash
+* ed192fb (HEAD -> main, origin/main, origin/HEAD) Añado los archivos a la carpeta
+* ddf0e9a Solucionado conflicto bibliografía.
+*   4951d4f Solucionado conflicto bibliografía.
+|\  
+| * a66d104 (bibliografia) Añadida nueva referencia bibliográfica.
+* | c6349ff Añadida nueva referencia bibliográfica.
+|/  
+*   6682e0b Añadida primera referencia bibliográfica.
+|\  
+| * 8ef7835 Añadido el capitulo4.txt
+* | 9fa5aa8 Añadida primera referencia bibliográfica.
+|/  
+* 2c507dc Añado el índice.txt
+* 3d84094 Añado el nuevo capitulo3.txt
+* 5371baf Añado el capitulo2.txt con el contenido
+* a9e8ef9 Modifico el capitulo1.txt por un error
+* 0b22acf Añadimos el capitulo1.txt
+* 8445bbc Initial commit
+(END)
+```
+
+**8. Ahora vamos a crear un nuevo commit en la rama bibliografia**
+
+```bash
+git checkout bibliografia
+cat > bibliografia.txt
+- Chacon, S. and Straub, B. Pro Git. Apress.
+```
+
+**9. En este paso vamos a fucionar las ramas**
+
+```bash
+ git checkout main
+ git merge bibliografia
+ git log --graph --all --oneline
+ git branch -d bibliografia
+ git log --graph --all --oneline
+```
+
+**10. Por ultimo terminamos con la biliografia**
+
+```bash
+git branch bibliografia
+git checkout bibliografia
+cat > bibliografia.txt
+- Scott Chacon and Ben Straub. Pro Git. Apress.
+- Ryan Hodson. Ry's Git Tutorial. Smashwords (2014)
+
+    Nota:Ctrl+D salimos del cat.
+
+git commit -a -m "Añadida nueva referencia bibliográfica."
+git checkout main
+cat > bibliografia.txt
+- Chacon, S. and Straub, B. Pro Git. Apress.
+- Loeliger, J. and McCullough, M. Version control with Git. O'Reilly.
+
+    Nota:Ctrl+D salimos del cat.
+
+ git commit -a -m "Añadida nueva referencia bibliográfica."
+ git merge bibliografia
+ git nano bibliografia
+ # Hacer los cambios indicados en el fichero
+ git commit -a -m "Solucionado conflicto bibliografía."
+ git log --graph --all --oneline
+```
+
+
(END)
```

**5. Añadimos el indice**

```bash
git add .
git commit -m "Se crea el indice."
echo "Indice de los cápitulos, con conceptos avanzados de git" >> indice.xt
git add .
git commit -m "Añadido el índice ."
git annotate indice.txt
```

**6. Ahora vamos a crear la nueva rama**

```bash
git branch bibliografia
git branch -av
```

**7. Creo el fichero 4**

```bash
git add .
git commit -m "Añadido capítulo 4."
git log --graph --all --oneline
```
Este es el resultado del log final como comenté antes

```bash
* ed192fb (HEAD -> main, origin/main, origin/HEAD) Añado los archivos a la carpeta
* ddf0e9a Solucionado conflicto bibliografía.
*   4951d4f Solucionado conflicto bibliografía.
|\  
| * a66d104 (bibliografia) Añadida nueva referencia bibliográfica.
* | c6349ff Añadida nueva referencia bibliográfica.
|/  
*   6682e0b Añadida primera referencia bibliográfica.
|\  
| * 8ef7835 Añadido el capitulo4.txt
* | 9fa5aa8 Añadida primera referencia bibliográfica.
|/  
* 2c507dc Añado el índice.txt
* 3d84094 Añado el nuevo capitulo3.txt
* 5371baf Añado el capitulo2.txt con el contenido
* a9e8ef9 Modifico el capitulo1.txt por un error
* 0b22acf Añadimos el capitulo1.txt
* 8445bbc Initial commit
(END)
```

**8. Ahora vamos a crear un nuevo commit en la rama bibliografia**

```bash
git checkout bibliografia
cat > bibliografia.txt
- Chacon, S. and Straub, B. Pro Git. Apress.
```

**9. En este paso vamos a fucionar las ramas**

```bash
 git checkout main
 git merge bibliografia
 git log --graph --all --oneline
 git branch -d bibliografia
 git log --graph --all --oneline
```

**10. Por ultimo terminamos con la biliografia**

```bash
git branch bibliografia
git checkout bibliografia
cat > bibliografia.txt
- Scott Chacon and Ben Straub. Pro Git. Apress.
- Ryan Hodson. Ry's Git Tutorial. Smashwords (2014)

    Nota:Ctrl+D salimos del cat.

git commit -a -m "Añadida nueva referencia bibliográfica."
git checkout main
cat > bibliografia.txt
- Chacon, S. and Straub, B. Pro Git. Apress.
- Loeliger, J. and McCullough, M. Version control with Git. O'Reilly.

    Nota:Ctrl+D salimos del cat.

 git commit -a -m "Añadida nueva referencia bibliográfica."
 git merge bibliografia
 git nano bibliografia
 # Hacer los cambios indicados en el fichero
 git commit -a -m "Solucionado conflicto bibliografía."
 git log --graph --all --oneline
```


