##README

Estos son los pasos que he seguido para componer el proyecto:

1- En primer lugar, he importado el dataset 'companies.json' a df_filtered.py
Después de haberle echado una primera ojeada al dataframe, he analizado los requisitos que se exigían a la hora de escoger empresas/ locales.
He decidido tener en cuenta un único requisito: el año de fundación de la empresa, ya que una de las solicitudes era el estar cerca de start-ups. También he mantenido columnas que he considerado que podría tratar más adelante, como 'total_money_raised'. No obstante, no he querido entrar en intentar homogeneizar las monedas. He eliminado muchas filas manteniendo aquellas que tuvieran únicamente los valores que me interesaban, quitando los 0 de la columna 'total_money_raised', etc.

2- El segundo Jupyter Notebook que he creado se llama 'df_geopoint'. En él he procurado filtrar aún más mi dataset trabajando sobre la columna 'founded_year'. He creado una nueva columna haciendo la media del año de fundación de las empresas que estuviesen a un radio de 1km de cada una de las empresas (filas) que me quedaban. Y he limitado aún más la base de datos, eliminando las filas en las que la media del año de fundación fuese inferior a 2013. 

3- He creado muchos documentos, muchos dataframes y he hecho varias pruebas en Tableau. He intentado varias veces conectarme a la API, sin resultado. 