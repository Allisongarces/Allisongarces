<div id="header" align="center">
  <img src="https://raw.githubusercontent.com/Allisongarces/Allisongarces/main/allison.png" width="100%" style="border-radius: 50px;">
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

### 🌟 Sobre Mí (EN)

```markdown
- 🔭 I’m currently working on data analysis projects related to public policy and infrastructure.
- 🌱 I’m currently learning advanced Natural Language Processing (NLP) and building dashboards with Plotly and Dash.
- 👯 I’m looking to collaborate on open-source data projects, especially those involving public data, social impact, or education.
- 🤔 I’m looking for help with best practices in deploying data science models.
- 💬 Ask me about Python, SQL, data cleaning, exploratory analysis, and dashboards.
- 📢 How to reach me: [LinkedIn](https://www.linkedin.com/in/allison-garces/), [Fiverr](https://es.fiverr.com/s/BRlyAaz), [GitHub](https://github.com/Allisongarces)
- 😄 Pronouns: she/her
- ⚡ Fun fact: I love turning messy data into beautiful insights and visuals 🌈📊
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
