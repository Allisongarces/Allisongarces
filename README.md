<div id="header" align="center">
     <img src="https://github.com/Allisongarces/Allison.-/blob/2a7486463ff79b3b1c1ec399a11aa42845912000/%20Banner%20para%20linkedin.png" width="80%" style="border-radius: 50px;">
  <h1 align="center" style="color:#5400A8">Hola a todos 👩🏻‍💻, Soy Allison Garcés</h1>

  <p align="center" style="color:#6141AC; max-width:700px; margin:auto">
    🎓 Analista de Datos con Maestría en <strong>Big Data & Data Analytics</strong>, y formación técnica en programación de software.<br><br>

    💼 Experiencia aplicando <strong>Python, SQL, Power BI</strong> y <strong>herramientas estadísticas</strong> para análisis de datos, automatización de reportes y visualización interactiva.<br><br>

    🌍 Buscando oportunidades <strong>remotas o en Europa</strong> para transformar datos en <strong>insights accionables</strong> que impulsen decisiones estratégicas.<br><br>

    ✨ Tecnologías: Python (Pandas, Matplotlib, NLTK), SQL, Power BI, Excel, R, Jupyter, Git, GitHub, NLP.
  </p>

  <p align="center">
    📢 <a href="https://www.linkedin.com/in/allison-garces/">LinkedIn</a> |
    💼 <a href="https://es.fiverr.com/s/BRlyAaz">Fiverr</a> |
    📁 <a href="https://github.com/Allisongarces">GitHub</a>
  </p>
</div>

<div align="center">
  <h3 style="color:#5400A8">Conecta conmigo</h3>
  <hr width="50%">
  <a href="https://www.linkedin.com/in/allison-garces/" target="_blank">
    <img src="https://img.shields.io/twitter/url?color=blueviolet&label=LinkedIn&logo=linkedin&style=social&url=https%3A%2F%2Fwww.linkedin.com%2Fin%2Fallison-garces%2F" alt="LinkedIn badge">
  </a>
  <a href="https://www.instagram.com/allisoncastano_/" target="_blank">
    <img src="https://img.shields.io/twitter/url?label=Instagram&logo=Instagram&style=social&url=https%3A%2F%2Fwww.instagram.com%2Fallisoncastano_%2F" alt="Instagram badge">
  </a>
  <a href="https://github.com/Allisongarces" target="_blank">
    <img src="https://img.shields.io/github/followers/Allisongarces?color=violet&label=Github&style=social" alt="GitHub badge">
  </a>
</div>

---

### 🌟 Sobre Mí

```markdown
- 🔭 Actualmente estoy trabajando en proyectos de análisis de datos relacionados con políticas públicas e infraestructura.
- 🌱 Estoy aprendiendo procesamiento de lenguaje natural (NLP) avanzado y desarrollando dashboards con Plotly y Dash.
- 👯 Estoy buscando colaborar en proyectos de datos open-source, especialmente aquellos que involucren datos públicos, impacto social o educación.
- 🤔 Busco ayuda con buenas prácticas para desplegar modelos de ciencia de datos.
- 💬 Pregúntame sobre Python, SQL, limpieza de datos, análisis exploratorio y dashboards.
- 📢 Cómo contactarme: [LinkedIn](https://www.linkedin.com/in/allison-garces/), [Fiverr](https://es.fiverr.com/s/BRlyAaz), [GitHub](https://github.com/Allisongarces)
- 😄 Pronombres: ella
- ⚡ Dato curioso: me encanta convertir datos desordenados en insights y visualizaciones hermosas 🌈📊

```

---

### 💡 Código Interesante

```python
# Extracción de entidades con spaCy
import spacy
from collections import Counter

nlp = spacy.load("en_core_web_sm")
text = open("documents_summary.txt").read()
doc = nlp(text)

entities = [ent.text for ent in doc.ents if ent.label_ in ["ORG", "GPE", "PERSON"]]
most_common = Counter(entities).most_common(10)

print("Entidades más frecuentes:")
for entity, count in most_common:
    print(f"{entity}: {count} veces")
```

```sql
-- Consulta SQL para ver tendencias de inversión por año
SELECT YEAR(Fecha_Inversion) AS Año, 
       SUM(Monto_USD) AS Total_Inversion_USD
FROM inversiones
GROUP BY Año
ORDER BY Año;
