# Proyecto Data Science 

## Objetivo primario

El objetivo final del trabajo será predecir si un cliente de un banco va a dejar de serlo o no en el futuro. Este tipo de predicciones es muy común en los bancos y funciona como un killer para un posible crédito a un cliente vigente. Por ejemplo, a la hora de obtener el universo a calificar para un posible crédito se scorean los clientes y, luego, se verifican ciertos killers, hay algunos que son filtros duros que los bancos no suelen flexibilizar y otros, son filtros blandos, los cuales pueden ser flexibilizados con el debido análisis de un Credit Risk Analyst. Dentro de los filtros duros, suele encontrarse el killer riesgo churn, que implica que el cliente va a dejar de serlo en un futuro, por lo tanto, a este cliente, no queremos alcanzarlo con un crédito porque podría implicar un riesgo de default mayor.

## Primeros pasos

En un primer momento queremos intentar de entender la correlación entre las distintas variables que figuran en el data set. Nuestra variable target va a ser Exited, la cual puede tomar los valores de 1 o 0 dependiendo de si el cliente deja el banco o no respectivamente. Todos los análisis están hechos en relación con esta variable target para ver qué peso van a tener dentro del modelo estas variables subyacentes. Además, gracias a estos análisis previos podemos verificar correlaciones fuertes y débiles, positivas y negativas. 

## Composición de dataset
Shape del dataset: 10.000 (filas), 18 (columnas).
RowNumber: corresponde a el número de las filas.
CustomerId: números al azar que identifican a los clientes.
Surname: apellido de los clientes del banco.
CreditScore: score de crédito, podría tener cierto efecto en churn (los clientes con mejor score son menos propensos a dejar el banco).
Geography: país de locación del cliente (puede afectar a la decisión de dejar el banco o no).
Gender: genero, femenino o masculino (puede afectar a la decisión de dejar el banco o no).
Age: edad del cliente (los clientes "mayores" son menos propensos a dejar el banco que los más jóvenes).
Tenure: número de años que el individuo ha sido cliente del banco. Generalmente, clientes más antiguos son más leales y tienden a irse del banco en menor medida.
Balance: deuda en el banco. Suele ser un buen indicador de churn. Personas con mayor deuda en sus cuentas son menos propensas a abandonar el banco que los que tienen menos deuda. 
NumOfProducts: número de productos que el cliente ha comprado en el banco.
HasCrCard: denota si el cliente tiene o no una tarjeta de crédito. Esta columna puede ser relevante ya que aquellos que tienen tarjetas son menos propensos a dejar el banco.
IsActiveMember: cliente activo (son menos propensos a dejar el banco lógicamente).
EstimatedSalary: salario estimado, al igual que la deuda (Balance) personas con menor salario son más propensas a dejar el banco.
Exited: si el cliente dejó o no efectivamente el banco.
Complain: si el cliente ha hecho una queja o no.
Satisfaction Score: score provisto por el cliente por la resolución de su queja.
Card Type: typo de tarjeta de crédito que tiene el cliente.
Points Earned: puntos ganados por el cliente al haber usado la tarjeta de crédito.

## Aclaración de composición del dataset 

Hay muchas variables que, a priori, sabemos o intuímos por el conocimiento del negocio que pueden influir en que un cliente se vaya o no de un banco, por lo tanto, son necesarias para el modelo. Ahora, tomando en cuenta la muestra de clientes del banco que tenemos, vemos que hay muchos casos en que no necesariamente la relación es tan predominante como pensaríamos.

## Link a la notebook

El link para poder acceder a la notebook donde se encuentran explicado todos los análisis y las preguntas es el siguiente:
https://colab.research.google.com/drive/1ACsOF8IvIh6cX4ddaIbyAH7a9G0_tH71?usp=sharing

