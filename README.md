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
class Person():

    def __init__(self):
        self.name = 'Luis Enrique Vázquez Rodríguez'
        self.nationality = 'mexican'
        self.age = 26
        self.education = 'Computer Engineering'
        self.career = 'Data Engineer'

class Profesional(Person):

        coding = ['Python','Javascript','HTML','CSS','SQL','NoSQL','VBA']
        tools = ['PySpark','GCP','Dataproc','Composer', 'Hadoop', 'Hive']
        architecture = ['ETL','Pipelines','Dataframes','Nodes','Visualizations']
        challenge = 'Studying for Google Cloud Data Engineer Certificate at the end of the year 2020'

def Present():
    me = Profesional()
    print('Hi there!')
    print(f"My name is {me.name}, I'm an {me.nationality} {me.career} with a {me.education} degree")
    print("Here are the lenguajes that I know so far:", *me.coding, sep=',')
    print("And here the tools that I can handle:", *me.tools, sep=',')
    print("The architectures in my day a day:", *me.architecture, sep=',')
    print(f"All of us have challenges and here is mine :D => {me.challenge}")
    print("That's all! See you later :)")

Present()
