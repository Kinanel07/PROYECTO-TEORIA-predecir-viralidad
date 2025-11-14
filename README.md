# PROYECTO-TEORIA-predecir-viralidad

# 📘 Resumen

Este proyecto propone un modelo para predecir la viralidad de videos en TikTok,
combinando datos estadísticos con análisis automatizado del contenido visual y auditivo.
Para ello se emplearon los modelos **LLaVA-NeXT-Video-7B (Zhang et al., 2024)** para des-
cribir el contenido visual del video, y **Audio Flamingo 3 (NVIDIA, 2025)** exclusivamente
para determinar si el audio contiene música.

A partir de estas variables y métricas como número de seguidores, likes, comentarios y
compartidos, se calculó el **engagement rate**, utilizado como medida principal de rendimiento.

En lugar de emplear un umbral fijo, la clasificación de viralidad se definió utilizando el
**percentil 75 del engagement rate**. Esto significa que el 25 % de los videos con mayor
interacción fueron considerados como virales.

Este enfoque permite adaptar la definición de viralidad a la distribución real de los
datos y construir un modelo predictivo más coherente con el comportamiento observado en la base.

**Palabras clave:** viralidad; redes sociales; modelos multimodales; TikTok.


---

# 📖 Introducción

Las redes sociales se han convertido en uno de los principales medios de comunicación,
consumo cultural y entretenimiento. En plataformas como TikTok, donde predominan videos
cortos de alta rotación, la viralidad depende de múltiples factores relacionados tanto con el
creador como con el contenido.

En este proyecto se propone un modelo predictivo multimodal, combinando datos
estadísticos con información visual y auditiva. Para ello se utilizó **LLaVA-NeXT-Video-7B**
para generar descripciones automáticas de los videos, y **Audio Flamingo 3** para identificar
si el contenido incluye música. La transcripción completa del audio no se empleó en esta
versión del proyecto y se deja para trabajos futuros.

El objetivo es determinar si un video pertenece al **25 % con mayor engagement rate**,
utilizando el percentil 75 como umbral de referencia. Esta clasificación sirve para estudiar
el comportamiento del algoritmo de viralización y explorar qué características del contenido
visual y auditivo están asociadas con un mejor desempeño.
