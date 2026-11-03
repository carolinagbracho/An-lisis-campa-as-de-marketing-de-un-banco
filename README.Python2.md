**TÍTULO DEL PROYECTO**  
**Análisis de campañas de marketing de un banco**   
 

**DESCRIPCIÓN DEL PROYECTO**  
Análisis exploratorio de datos (EDA) con Python y Pandas sobre campañas de marketing por teléfono de una entidad bancaria portuguesa, cuyo objetivo era que los clientes contrataran un depósito a plazo.   
Se trabaja con dos fuentes de datos: 

- bank-additional.csv: 43.000 llamadas con datos del cliente, de la llamada, de campañas anteriores y del contexto económico.  
- customer-details.xlsx: 3 hojas (clientes dados de alta en 2012, 2013 y 2014\) con ingreso anual, hijos, fecha de alta y visitas web mensuales.

**ESTRUCTURA DEL PROYECTO**  
├──DataProject\_ Proyecto EDA con Python.docx  
	├──customer-details.xlsx  
	├──bank-additional.csv  
├──bank\_additional2.ipynb  
├──Python\_for\_data\_PROYECT (1).pdf  
├── README.md 

**INSTALACIÓN Y REQUISITOS** 

- Python 3.10 o superior   
- Librerías: pandas, numpy, matplotlib, seaborn, scipy, openpyxl (para leer el Excel) y jupyter (o la extensión de Jupyter de Visual Studio Code)

**RESULTADOS Y CONCLUSIONES**

### Resultados

- Tasa global de contratación: 11,3 % (fuerte desbalance entre "sí" y "no")   
- Resultado de campaña previa success:65,3 % de contratación (frente al 8,8 % sin contacto previo)   
- Estudiantes y jubilados:	31,4 % y 25,2 % (más del doble de la media)  
- Contacto por móvil frente a fijo:14,7 % frente a 5,2 %   
- Ingreso, hijos, visitas web: Sin relación con la contratación (p \= 0,447 y p \= 0,266; \|r\| ≤ 0,01)

### Conclusiones

- El resultado de la campaña anterior es el factor más asociado a la contratación.   
- La profesión influye: estudiantes y jubilados contratan mucho más; blue-collar y services, menos.   
- El contexto económico (euríbor, empleo) se asocia a menos contratación cuando está alto. Las tres variables macroeconómicas miden esencialmente un único factor.   
- Las llamadas más largas se asocian a más contratación (r \= 0,40), pero la duración solo se conoce después de la llamada, por lo que no sirve para decidir a quién llamar.   
- Los datos demográficos del segundo dataset (ingreso, hijos, visitas web) no explican la contratación.

**Recomendaciones**: recontactar a clientes con éxito previo, segmentar hacia estudiantes y jubilados (son segmentos pequeños, aprox. 6 % de la base), priorizar el móvil, no insistir con muchos contactos y evitar segmentar por ingreso o familia.   
**Limitaciones**: variable objetivo desbalanceada, fuga de datos en duration, grupos pequeños (por ejemplo illiterate, n \= 18), valores imputados en ‘euribor3m’, ‘age’ y ‘education’, y datos con apariencia sintética en el dataset de clientes.

El informe completo, con tablas y gráficos, está en el archivo del informe del análisis.

**CONTRIBUCIONES**  
Las contribuciones son bienvenidas. Si deseas mejorar el proyecto, por favor abre un pull request o una issue. 

**AUTORES Y AGRADECIMIENTOS**   
Carolina Gómez Bracho

https\://github.com/carolinagbracho/katas\_python