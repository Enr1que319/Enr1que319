### Just run the script ⚙️🧠😎

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
    name            : str   = "Enrique Vázquez"
    age             : int   = 30
    career          : str   = "Computer Engineer"
    languages       : tuple = ("Python", "Scala", "JS", "Bash", "VBA")
    databases       : tuple = ("PostgreSQL", "MongoDB", "MySQL","Hive","Server","Firebase", "Snowflake")
    frameworks/lib  : tuple = ("Spark","Pandas","Airflow")
    cloud           : tuple = ("GCP", "AWS")
    ongoing         : tuple = ("Kafka", "Databricks")
    challenge       : str   = "Getting new certs"

    def Myself(self):
        return json.dumps(asdict(self), indent=4)

Introduce = AboutMe()
print(Introduce.Myself())

```
