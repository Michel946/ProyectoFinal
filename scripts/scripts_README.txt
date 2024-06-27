#Filogenia del genero Euphorbia
Mi proyecto consiste en realizar una filogenia del genero Euphorbia perteneciente a la familia Euphorbeacea. Para ello utilice 10 especies del genero Euphorbia y 1 especie del genero Croton como grupo externo. Realice el análisis apartir del gen rps7. La secuencias de cada especie las obtuve del NCBI. 

#Paso 1 
 En el NCBI busqué el gen rsp7 del genero de plantas Euphorbia. Descargue las secuencias del gen de 10 especies. De igual forma descargue la secuencia del gen rps7 de una especie del genero Croton utilizada como grupo externo 

#Programas utilizados 

Git Bash
Software Muscle
IQ-TREE
FigTree
Sublime


#Instalación del programa IQ-TREE para Windows
Se obtuvo el programa IQ-TREE a traves del siguiente enlace:
https://github.com/iqtree/iqtree2/releases/download/v2.2.0/iqtree-2.2.0-Windows.zip

#Comandoa
1. Git Bash 
Crear una carpeta en el Desktop y tres subarpetas (data, results, scripts)
mkdir ProyectoFinalMichelleSuntaxi
mkdir data results scripts

2. Secuencias
Las secuencias que utilicé las descargue de NCBI. Estas fueron guardadas en la carpeta data.

3. Programa Sublime
Modifiqué las secuencias en el programa Sublime y solo deje el nombre científico de la especie y la secuencia.


4. Software Muscle
Subí mi documento de las secuencias en formato fasta en la pagina Muscle software. Seleccioné el archico Pearson (fasta).
Una vez obtenido el documento alineado lo descargué y lo guardé en la carpeta results.

5. Git Bash
Al descargar el programa iqtree lo guarde en Desktop y apliqué los siguientes comandos: 
cd Desktop/
cd iqtree-2.2.0-Windows/
ls
cd bin/
"#"export PROJ_DIR=
pwd
/c/Users/Familia/Desktop/iqtree-2.2.0-Windows/bin/

Copié ese comando y lo modifiqué , obteninedo la siguiente línea:
export PROJ_DIR=/c/Users/Familia/Desktop/iqtree-2.2.0-Windows/bin/iqtree2.exe

Finalmente para obtener mis árboles coloque el siguiente comando:
$PROJ_DIR -s secuencias_alineamiento.aln-fasta -B 1000

6. Figtree
Emplee el archivo secuencias_alineamineto.aln-fasta.treefile guardado en la carpeta results.
Enraíce a mi especie del genero Croton como grupo externo.
Modifique el árbol para que las especies queden alineadas.

