# Analisis-de-embudo-y-retencion-ecommerce-SQL

Mapeo del embudo de conversión y análisis de retención por cohortes para MercadoLibre, identificando puntos de fuga en el customer journey y patrones de recurrencia. 

Tecnologías: SQL Avanzado (CTEs, Window Functions), Análisis de Cohortes, Métricas de Retención (D1, D7, D30), Optimización de Tasa de Conversión (CRO) y Metodología C-F-I. 

## 1. Contexto del Proyecto

Este proyecto simula el rol de un analista de producto dentro del equipo de Crecimiento y Retención de MercadoLibre. El objetivo principal fue entender en qué etapas del embudo de conversión se pierden más usuarios y cómo evoluciona su retención a lo largo del tiempo. Para ello, trabajé con dos datasets: uno centrado en eventos del funnel (first_visit → purchase) y otro orientado a retención por cohortes (D7, D14, D21, D28).
El trabajo incluyó la construcción del embudo completo mediante SQL, el cálculo de tasas de conversión, la segmentación por país, dispositivo y fuente de tráfico, y el análisis de retención mensual para identificar patrones de engagement y oportunidades de mejora.

##2. Análisis Realizado 

A través de SQL y CTEs construí un embudo de siete etapas clave, evaluando el comportamiento de los usuarios entre enero y agosto de 2025. El análisis reveló que la mayor caída ocurre entre select_item (76.9%) y add_to_cart (11.0%), lo que representa una pérdida de 65.9 puntos porcentuales y una caída relativa del 85.7% de usuarios interesados que no avanzan a inicio de compra.
Al segmentar por país, Uruguay mostró el mejor desempeño con un 4.33% de usuarios completando todo el journey, mientras que Paraguay no registró compras. Brasil, Argentina y Paraguay presentaron las mayores oportunidades de mejora, con pérdidas superiores al 70% en la transición select_item → add_to_cart.
En retención, analicé cohortes de usuarios registrados entre enero y junio de 2025. La cohorte de marzo mostró la mejor retención D7 (87.7%), mientras que junio tuvo la más baja (85.9%). La retención D28 no superó el 3% en ninguna cohorte, aunque Perú y México destacaron con valores ligeramente superiores. La retención D14 se mantuvo estable con variaciones menores al 5% entre países.

## 3. Conclusiones y Recomendaciones

El punto crítico del embudo es la etapa add_to_cart, donde se pierde la mayor cantidad de usuarios. Mejorar esta transición tendría un impacto directo en todas las etapas posteriores, por lo que priorizaría optimizaciones como pruebas A/B del botón (tamaño, color, copy), simplificación del flujo y retargeting para recuperar al menos un 15% de usuarios perdidos.
En retención, los datos muestran que el engagement cae significativamente después del día 14 y que la retención D28 es baja en todos los países. Perú y México destacan como benchmarks positivos, por lo que se recomienda analizar su onboarding y replicar prácticas que impulsen la actividad temprana. También se sugiere implementar campañas de re-engagement entre D14 y D21 para reducir la caída del 52% al 35%.
En general, el análisis permitió identificar los principales puntos de fuga, entender diferencias entre mercados y proponer mejoras accionables basadas en datos reales.

### Documentación del Proyecto
Para más detalles técnicos, puedes consultar el siguiente documento:
👉 [Haz clic aquí para ver el Manual de Usuario (PDF)](./Proyecto4.pdf)
