# Análisis de Datos: Evaluación del Rendimiento de un Negocio de E-commerce "Showz" (Empresa de venta de entradas de eventos)

Este proyecto ofrece un análisis exhaustivo del rendimiento de una plataforma de e-commerce. El objetivo es evaluar métricas comerciales clave relacionadas con la actividad de los usuarios, las ventas y la eficiencia del marketing para identificar fortalezas, debilidades y áreas de mejora.

## Objetivo
Evaluar la salud general de la plataforma de e-commerce mediante el análisis de:
- La participación y retención de los usuarios.
- El rendimiento de las ventas y el valor de vida del cliente.
- La eficiencia y rentabilidad de las inversiones en marketing.

## 🛠️ Tecnologías Utilizadas
- **Python:** Pandas, NumPy (para la manipulación de datos)
- **Jupyter Notebook:** Entorno interactivo para el análisis.
- **Visualización de Datos:** Matplotlib, Seaborn
- **Conjuntos de Datos CSV:** Contienen registros de visitas de usuarios, pedidos y costos de marketing.

## Pasos Clave
1.  **Preparación de Datos:**
    - Se cargaron y limpiaron tres conjuntos de datos: `visits_log_us.csv`, `orders_log_us.csv` y `costs_us.csv`.
    - Se convirtieron los tipos de datos y se crearon nuevas características (ej., `duración_sesión`, `mes_cohorte`) para un análisis más profundo.
2.  **Análisis de Actividad y Retención de Usuarios:**
    - Se calcularon los usuarios activos diarios (DAU), semanales (WAU) y mensuales (MAU) para comprender la escala de usuarios.
    - Se realizó un análisis de cohortes para rastrear la retención de usuarios a lo largo del tiempo.
3.  **Análisis de Ventas y Valor del Cliente:**
    - Se analizó el comportamiento de compra, incluyendo el tiempo hasta la primera compra y el valor medio del pedido.
    - Se calculó el Valor de Vida del Cliente (LTV) para comprender los ingresos a largo plazo generados por cohorte de usuarios.
4.  **Análisis de la Eficiencia del Marketing:**
    - Se calculó el gasto total en marketing y el Costo de Adquisición de Clientes (CAC) por fuente.
    - Se analizó el Retorno de la Inversión en Marketing (ROMI) de forma mensual.

## Resultados
El análisis confirma que, si bien la plataforma tiene una base de usuarios sólida y activa, existen desafíos significativos en la retención de usuarios y la rentabilidad del marketing:

*   **Actividad de Usuarios:** La plataforma tiene una base de usuarios sólida con un **DAU de ~907**, un **WAU de ~5,800** y un **MAU de ~23,000**. Los usuarios realizan una sesión promedio por día con una duración de **11 minutos**.
*   **Retención:** La retención de usuarios es un desafío importante. La retención cae a menos del **10 %** en el primer mes y se mantiene consistentemente baja en los meses siguientes.
*   **Monetización:** El tamaño medio de compra es de **$5.00**. El tiempo medio hasta la primera compra de un usuario es de **17 días**. El **LTV** de las cohortes de usuarios más recientes es más bajo que el de las anteriores, lo que indica una disminución en el valor del usuario con el tiempo.
*   **Eficiencia del Marketing:** El gasto total en marketing fue de **$329k**. El **CAC varía significativamente** según la fuente, siendo las fuentes 9 ($0.59), 4 ($0.73) y 10 ($0.72) las más eficientes. De manera crítica, el **ROMI mensual fue consistentemente negativo**, lo que significa que el gasto en marketing no generó suficientes ingresos para ser rentable.

## Cómo Ejecutarlo
1.  Clona este repositorio:
    ```bash
    git clone <(https://github.com/ferchi4/Proyecto-spring-9)>
    ```
2.  Asegúrate de tener instaladas las dependencias necesarias:
    ```bash
    pip install pandas numpy matplotlib seaborn scipy jupyter
    ```
3.  Coloca los archivos CSV (`visits_log_us.csv`, `orders_log_us.csv`, `costs_us.csv`) en el mismo directorio que el notebook.

4.  Abre y ejecuta el Jupyter Notebook `proyecto9.ipynb` para ver el análisis completo.
