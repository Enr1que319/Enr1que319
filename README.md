### Hi there 👋

<!--
**Enr1que319/Enr1que319** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->

```python, term=True
import json
from dataclasses import asdict, dataclass

@dataclass
class AboutMe:
    name        : str   = "Enrique Vázquez"
    age         : int   = 26
    career      : str   = "Computer Engineer"
    languages   : tuple = ("Python", "JS", "Bash", "VBA")
    databases   : tuple = ("PostgreSQL", "MongoDB", "MySQL","Hive")
    frameworks  : tuple = ("Spark", "Hadoop","Pandas", "D3", "Leaflet")
    cloud       : tuple = ("Dataproc", "BigQuery", "Composer", "Storage")
    ongoing     : tuple = ("Airflow", "Go", "Scala")
    challenge   : str   = "Studying for Google Cloud Data Engineer Certificate at the end of the year 2020"

    def Myself(self):
        return json.dumps(asdict(self), indent=4)

Introduce = AboutMe()
print(Introduce.Myself())
