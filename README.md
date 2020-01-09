![Iron Hack](https://github.com/rogerzadi/ModeloSupervivencia/blob/master/images/ironhack.png)
# Web Scraping (Ideame.com)
Este programa se utiliza para scrapear mas de 1,000 proyectos de [Ideame](https://www.idea.me/), la cuyal es una pagina de crowdfunding a nivel Latinoamerica, en esta pagina hay diversas categorias, las cuales fueron scrapeadas para completar y limpiar un DataSet de Kickstart encontrado en Kaggle, esto porque en el dataset habia muy poca presencia de proyectos latinoamericanos.

### Modelos Utilizados
Se utiliza las siguientes librerias:
- requests
- time 
- BeautifulSoup
- Asi como tambien se hace uso de Selenium

## Modelo

Primero se limpia el dataset de KickStart para ver las variables mas relevantes y las que concuerden con las obtenidas en IDEAME,
se requiere instalar un driver de Chrome o Firefox para el funcionamiento de Selenium, se utiliza ya que para ver mas proyectos se requiere dar click en "Ver Mas".

El request se hace directamente en la URL de los proyectos donde a cada iteracion se cambia de categoria.

El programa tiene 3 variables de entrada con las cuales puedes jugar:

-URL (Por si se requiere escrapear otra URL)
- Paginas a scrapear 
- Veces de clicks en "Ver màs"

Una vez obtenida la información se guarda en un DataFrame y se concatena con el DataSet inicial de Kickstart
