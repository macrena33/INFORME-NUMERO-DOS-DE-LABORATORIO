# Laboratorio 02 - Alineamiento de secuencias [![img](https://github.com/bioinf-biotec/labs_bioinf/raw/master/images/vertical-alignment.png?raw=true)](https://github.com/bioinf-biotec/labs_bioinf/blob/master/images/vertical-alignment.png?raw=true)

### Parte 1: Colectar genes homólogos.



**1.** ¿Qué función cumple el gen SRY? [2]

-  Este gen sin intrones codifica un factor de transcripción que es un miembro de la familia de proteínas de unión a ADN del grupo de alta movilidad (HMG). Esta proteína es el factor determinante de los testículos (TDF), que inicia la determinación del sexo masculino. Las mutaciones en este gen dan lugar a mujeres XY con disgenesia gonadal (síndrome de Swyer); la translocación de parte del cromosoma Y que contiene este gen al cromosoma X causa el síndrome XX masculino.

  [ncbi gen ](https://www.ncbi.nlm.nih.gov/gene/6736) 

**2.** ¿Cuántos genes ortólogos están anotados en esa base de datos? [1]

-  29 gene 

[ncbi gen](https://www.ncbi.nlm.nih.gov/gene/?Term=ortholog_gene_6736[group]) 

### Parte 2: Alineamiento múltiple.



**3.** ¿Qué es el EMBL-EBI? [2]

-  Proporcionan servicios de bioinformática y datos de libre acceso a la comunidad científica. Es una base de datos.

[EMBL-EBI](https://www.ebi.ac.uk/about) 

**4.** ¿Cuál es el programa que ellos ofrecen que funciona mejor para secuencias de proteínas? [2]

- MUSCLE , herramienta precisa de MSA, especialmente buena con proteínas. Adecuado para alineaciones medianas. 

  [EMBL-EBI](https://www.ebi.ac.uk/Tools/msa/)

**5.** ¿Qué otros tipo de herramientas ofrece EMBL-EBI? [2]

- Ofrece herramientas de tipo, para el uso de alineamientos grandes, pequeños y medianos, ya sea para proteínas, secuencias multiples o secuencias de una alineacion. Tomando en cuenta la filogenia e informacion evolutiva. 

  [EMBL-EBI](https://www.ebi.ac.uk/Tools/msa/) 

**6.** ¿Cuál es el costo de abrir un gap? [1]

- Según EMBL-EBI un Gap tiene un costo de 1,53

  [EMBL-EBI](https://www.ebi.ac.uk/Tools/msa/mafft/) 

**7.** ¿Cuál es el costo de extender un gap? [1]

- Según EMBL-EBI el costo deextender un Gap es de 0,123

  [EMBL-EBI](https://www.ebi.ac.uk/Tools/msa/mafft/)

**8.** ¿Cuál es la longitud total del alineamiento? [1]

- la longitud total del aliniamiento es de  1935

  [EMBL-EBI](https://www.ebi.ac.uk/Tools/msa/mafft/)

------



![](https://raw.githubusercontent.com/YarabiConchaVillagran/Informe-2./master/Captura%201.PNG)



![](https://raw.githubusercontent.com/YarabiConchaVillagran/Informe-2./master/Filogenia.PNG)



**9.** ¿Cuál es la especie cuyo gen SRY está más relacionado con el gen SRY de humanos? [2]

- El gen mas cercano al de humanos es Piliocolubus_tephorosceles 0.00133.

  [RAW.GITHUB](https://raw.githubusercontent.com/YarabiConchaVillagran/Informe-2./master/Captura%201.PNG)

**10.** ¿Cuál es el más lejano? [2]

- Son dos genes los mas lejanos, el Bos_indicus 0.00109 y Bison_bison 0.00326

  [RAW.GITHUB](https://raw.githubusercontent.com/YarabiConchaVillagran/Informe-2./master/Filogenia.PNG)

**11.** ¿Cuál es la especie cuyo gen SRY es más cercana a la del burro? [2]

- El gen mas cercano corresponde a Equus_przewalskii 0.00076

  [RAW.GITHUB](https://raw.githubusercontent.com/YarabiConchaVillagran/Informe-2./master/Filogenia.PNG)

**12.** ¿Cómo esperas que sea el alineamiento si el costo de abrir un gap aumenta? ¿Y si disminuye? [3]

- Si el costo de abrir un  gap aumenta se obserbaran mas extenciones de este mismo y si disminuye se vera todo lo contrario, una disminucion en la extencion de estos.

  ![Gap con un costo de 1.53](https://raw.githubusercontent.com/YarabiConchaVillagran/Informe-2./master/1%2C53.PNG)



![Gap costo 2.00](https://raw.githubusercontent.com/YarabiConchaVillagran/Informe-2./master/2%2C0.PNG)

**13.** ¿Cómo esperas que sea el alineamiento si el costo de extender un gap aumenta? ¿Y si disminuye? [3]

- Como se puede obserbar cuando el costo de extender un gap aumenta hay menos extenciones y si el costo de extender un gap disminuye habra mas extenciones. 

![gap costo 0.123](https://raw.githubusercontent.com/YarabiConchaVillagran/Informe-2./master/0%2C123.PNG)

![gap costo 0.300](https://raw.githubusercontent.com/YarabiConchaVillagran/Informe-2./master/0%2C300.PNG)

**14.** ¿Cuál fue el efecto de aumentar el costo de abrir un gap en la longitud total del alineamiento? [2]

- Cuando se habre un gap en su maximo valor, obtenemos mas extenciones de este.

  ![gap a costo maximo](https://raw.githubusercontent.com/YarabiConchaVillagran/Informe-2./master/Gap%203.PNG)

**15.** Prueba lo mismo, pero esta vez **disminuyendo al mínimo el costo de extender un gap**. Describe cómo cambia el alineamiento. [2]

- Cuando se disminuyen el costo de extender un gap, se ve menos acortada la secuencia de genes.

  ![gap a un costo minimo](https://raw.githubusercontent.com/YarabiConchaVillagran/Informe-2./master/ext%200%2C001.PNG)

#### Parte 3: Diseño de partidores.



**16.** Agrega a tu informe una lista de los "*LEFT PRIMER*" y "*RIGHT PRIMER*" que obtuviste usando Primer3. [3]

- LEFT PRIMER        175   20   59.02   50.00    0.00   0.00    0.00 11.00 AGAGTGAAGCGACCCATGAA
- RIGHT PRIMER       365   20   59.02   50.00    3.32   0.00    0.00 10.00 TCTCTGTGCATGGCCTGTAA

**17.** Indica los partidores *forward* y *reverse* que escogiste y explica por qué son la mejor opción para amplificar el gen SRY de humano. [5]

- En el programa "AmplifX" se puede decir que los partidores (forward y reverse) que son la mejor opcion son los siguientes: AGATGCTGCCGAAGAATTGC, GCTTTGTCCAGTGGCTGTAG y CGAAGATGCTGCCGAAGAAT, CTACAGCTTTGTCCAGTGGC. 

  Debido a que estos secuencian un mayor % de bases nitrogenadas Guanina y Citosina (56%) lo cual hace que la secuencia mucho más estable, ya que estas tienen 3 puntes de hidrógeno.

**18.** ¿Cuál es el largo del amplicón? ¿Y la temperatura de *annealing* sugerida? [3]

- El largo del primer primer nombrado es de 204 pb y su temperatura de alineamiento sugerida es de 55°C. En cuanto al segundo primer nombrado, este tiene un largo de 212 pb y su temperatura de alineamiento sugerida es de 55°C siendo esta igual que el anterior.



------





​	Macarena González Bustos.

​        Ingenería en Biotecnología.

​         Viernes 17 de agosto 2018.