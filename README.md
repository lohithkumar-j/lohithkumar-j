# generate_readme.py

data = {
    "name": "Shrinath Munagapati",
    "github_username": "MShrinath",
    "about_me": "Interested in Cyber Security",
    "socials": {
        "LinkedIn": "https://linkedin.com/in/mshrinath",
        "Instagram": "https://instagram.com/mr.shido_",
        "GitLab": "https://gitlab.com/MShrinath"
    },
    "tech_stack": [
        {"name": "Arduino", "url": "https://www.arduino.cc/"},
        {"name": "Bash", "url": "https://www.gnu.org/software/bash/"},
        {"name": "C", "url": "https://www.cprogramming.com/"},
        {"name": "CSS", "url": "https://www.w3schools.com/css/"},
        {"name": "Django", "url": "https://www.djangoproject.com/"},
        {"name": "Express.js", "url": "https://expressjs.com/"},
        {"name": "Firebase", "url": "https://firebase.google.com/"},
        {"name": "Git", "url": "https://git-scm.com/"},
        {"name": "HTML", "url": "https://www.w3.org/html/"},
        {"name": "Java", "url": "https://www.java.com/"},
        {"name": "JavaScript", "url": "https://developer.mozilla.org/en-US/docs/Web/JavaScript"},
        {"name": "Linux", "url": "https://www.linux.org/"},
        {"name": "MongoDB", "url": "https://www.mongodb.com/"},
        {"name": "Node.js", "url": "https://nodejs.org/"},
        {"name": "Pandas", "url": "https://pandas.pydata.org/"},
        {"name": "PostgreSQL", "url": "https://www.postgresql.org/"},
        {"name": "Postman", "url": "https://postman.com/"},
        {"name": "Python", "url": "https://www.python.org/"},
        {"name": "React", "url": "https://reactjs.org/"}
    ]
}

def generate_socials_md(socials):
    lines = []
    for name, url in socials.items():
        badge_url = f"https://img.shields.io/badge/{name}-blue?logo={name.lower()}&style=for-the-badge"
        lines.append(f"[![{name}]({badge_url})]({url})  ")
    return "\n".join(lines)

def generate_tech_stack_md(tech_stack):
    lines = []
    for tech in tech_stack:
        tech_name = tech["name"].replace(" ", "%20")
        badge_url = f"https
