# Repositorio de la materia "Exploración y Curación de Datos"
#### Diplomatura en Ciencia de Datos, Aprendizaje Automático y sus Aplicaciones. *Edición 2021*

Integrantes:
* Devesa, Maria Roberta. 
* Feldfeber, Ivana. 
* Finzi, Nadia. 
* Kinigsberg, Ezequiel. 
* Villafañe, Roxana Noelia


En este repositorio se encuentran los dos notebooks correspondientes a los dos entregables de la materia:
"Exploración y Curación de Datos". 
* Sitio web de la materia: https://diplodatos.famaf.unc.edu.ar/analisis-y-curacion-de-datos/ 

### Documentación

#### Datasets


* El conjunto de datos pre-procesado sobre [estimación de precios de ventas de propiedades](https://www.kaggle.com/dansbecker/melbourne-housing-snapshot) en Melbourne, Australia, disponible en la plataforma Kaggle. 
* Un conjunto de datos de [scrapings del sitio AirBnb](https://www.kaggle.com/tylerx/melbourne-airbnb-open-data?select=cleansed_listings_dec18.csv) para la ciudad de Melbourne, Australia, 2018, disponibilizado por Tyler Xie, a través de la plataforma Kaggle.



#### Entregable 1

Referido a las clases 1 y 2 de la materia.

*Temas:* 
* Exploración, 
* combinación de datasets 
* datos ruidosos.

**Breve descripción** 

*(para una descripción más detallada consultar la documentación disponible en este repositorio)*

* El trabajo se dividió en tres etapas principales. 
* Primero el estudio del dataset para entender y analizar la información del mismo. Luego se realizó un proceso de imputación de valores faltantes, y finalmente la composición y exportación del dataset final.
El estudio del dataset tiene como objetivo comprender la información disponible, su distribución, los rangos de las variables y las imitaciones de las mismas; como por ejemplo la cantidad de valores faltantes. Se basó en los siguientes puntos: 
* Estudio de valores extremos por medio del análisis de las variables y sus rangos.
* El análisis de los Outliers estudiando las distribuciones y los cuantiles de las variables.
* La selección de columnas de interés para el objetivo del estudio. Se estudió la información de cada columna y se analizaron sus valores.
* Se realizó un proceso de Imputación de los valores faltantes utilizando la información del dataset de AirBnB.
* Primero se investigó las variables posibles para combinar.
* Para los casos posibles se pasó a la etapa de Imputación. Se imputaron los valores faltantes de la columna CouncilArea.
* Una vez definido el dataset final se lo exportó en formato `.csv` bajo el nombre `MelbourneCurado.csv`


#### Entregable 2 

Referido a las clases 3 y 4 de la materia. 

*Temas:* 
* sesgo, 
* transformaciones, 
* normalización.

**Breve descripción**

*(para una descripción más detallada consultar la documentación disponible en este repositorio)*

* En primer se realizó un encoding de las variables excepto `BuildingArea` y `YearBuilt`, mediante la función `OneHotEncoder`.
* Posteriormente, las variables  `BuildingArea` y `YearBuilt` se imputaron mediante `IterativeImputer` con un estimador `KNNRegressor`. Se graficaron las distribuciones de valores antes y después de imputar con KNN. 
* Luego, estos resultados se procesaron mediante Análisis de Componentes Principales (PCA) y se graficaron las varianzas acumuladas en cada componente principal. 
* Se agregaron las columnas correspondientes del análisis de PCA a la matriz original de datos. 
* Composición de resultado: en esta etapa se guardaron los cambios en un `pandas.DataFrame`.
* Se documentaron los pasos realizados. 

