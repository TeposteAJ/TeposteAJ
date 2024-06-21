```python
#!/usr/bin/python
# -*- coding: utf-8 -*-

class PythonDeveloper:
    def __init__(self):
        self.name = "Angie"
        self.perceived_role = "Web developer"
        self.official_title = " Developer Analyst"
        self.language_spoken = ["esp_LATAM", "en_US"]
        self.currently_learning = ["automated_test","JavaScript"]
        self.currently_working = ["API's web", "Open Source", "ERP", "Personal Project"]
        
    def say_random(self):
        print("If a line of code from your life transcends, you've done more than most.")

me = PythonDeveloper()
me.say_random()
```

```python
from odoo import models, fields, api

class OdooDeveloper(models.Model):
    _name = 'python.developer'
    _description = 'Partner Odoo Developer'

    name = fields.Char(string='Name', default="Angie")
    perceived_role = fields.Char(string='Perceived Role', default="Web Developer")
    official_title = fields.Char(string='Official Title', default="Developer Analyst")
    language_spoken = fields.Selection(
        [('es_MX', 'Spanish (MEX)'), ('en_US', 'English (US)')],
        string='Language Spoken',
        default='es_MX'
    )
    currently_learning = fields.Many2many(
        'learning.topic', 
        string='Currently Learning'
    )
    currently_working = fields.Many2many(
        'work.topic', 
        string='Currently Working'
    )

    @api.model
    def say_random(self):
        return "If a line of code from your life transcends, you've done more than most."

    def print_learning_and_working(self):
            learning_topics = ', '.join(self.currently_learning.mapped('name'))
            working_topics = ', '.join(self.currently_working.mapped('name'))
            print(f"Currently Learning: {learning_topics}")
            print(f"Currently Working: {working_topics}")


```
<div align="left">
<h2> Languages and Tools  <img src="https://media.tenor.com/Es9wm76r9QkAAAAi/angry-typing-cat.gif" width="40"> :</h2>
</div>
<a href="https://fortran-lang.org/es/index" target="Fortran"><img align="left" alt="Fortran" height ="42px" src="https://upload.wikimedia.org/wikipedia/commons/thumb/b/b8/Fortran_logo.svg/800px-Fortran_logo.svg.png"/> </a>
<a href="https://datastudio.withgoogle.com/" target="GoogleDataStudio"><img align="left" alt="Java" height ="42px" src="https://cdn.worldvectorlogo.com/logos/google-data-studio.svg"/> </a>
<a href="https://www.python.org" target="_blank"><img align="left" alt="Python" height ="50px" src="https://raw.githubusercontent.com/rahul-jha98/github_readme_icons/main/language_and_tools/square/python/python.svg"/> </a>
<a href="https://www.django-rest-framework.org/" target="Django"> <img align="left" alt="Django" height ="42px" src="https://cdn.worldvectorlogo.com/logos/django.svg" alt="firebase" height ="42px"/> </a>
<a href="https://www.postman.com/" target="Postman"> <img align="left" alt="Postman" height ="42px"img src="https://uxwing.com/wp-content/themes/uxwing/download/brands-and-social-media/postman-icon.png" /> </a>
<a href="https://www.postgresql.org/" target="Postgresql"> <img align="left" alt="Postgresql" height ="42px" src="https://upload.wikimedia.org/wikipedia/commons/2/29/Postgresql_elephant.svg"/> </a>
<a href="https://devcenter.heroku.com/" target="Heroku"><img align="left" alt="Heroku" height ="42px" src="https://cdn-icons-png.flaticon.com/512/873/873120.png"/> </a>

<a href="https://git-scm.com/" target="Git"> <img align="left" alt="Git" height ="42px" img src="https://raw.githubusercontent.com/rahul-jha98/github_readme_icons/main/language_and_tools/square/git-scm/git-scm.svg"/> </a>
<a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript" target="JavaScript"> <img align="left" alt="JavaScript" height ="42px"  src="https://raw.githubusercontent.com/rahul-jha98/github_readme_icons/main/language_and_tools/square/javascript/javascript.svg"> </a>
<a href="https://reactjs.org/" target="React"> <img align="left" alt="React" height ="42px" src="https://raw.githubusercontent.com/rahul-jha98/github_readme_icons/main/language_and_tools/square/react/react.svg"/> </a>
<a href="https://www.netlify.com/" target="Netifly"> <img align="left" alt="Netifly" height ="42px" src="https://cdn.freebiesupply.com/logos/large/2x/netlify-logo-png-transparent.png"/> </a>
<a href="https://www.figma.com/" target="Figma"> <img align="left" alt="Figma" height ="42px" src="https://raw.githubusercontent.com/rahul-jha98/github_readme_icons/main/language_and_tools/square/figma/figma.svg"/> </a>
<a href="https://code.visualstudio.com/" target="VisualStudioCode"> <img align="left" alt="VSC" height ="42px" img src="https://upload.wikimedia.org/wikipedia/commons/thumb/9/9a/Visual_Studio_Code_1.35_icon.svg/2048px-Visual_Studio_Code_1.35_icon.svg.png"/> </a>
