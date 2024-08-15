## Hi there 👋

<a href="https://ibharatbhushan.netlify.app/" target="_blank">
    <img width="1680" alt="Screenshot 2024-08-15 at 8 23 44 PM" src="https://github.com/user-attachments/assets/a5a0a76c-fa8b-4be6-b107-f08c522ed967">
</a>
<a href="https://www.linkedin.com/in/bhushan9473" target="_blank">
    <img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn Badge"/>
</a><a href="https://linktr.ee/Bharat_29_11" target="_blank">
    <img src="https://img.shields.io/badge/Linktree-000000?style=for-the-badge&logo=linktree&logoColor=white" alt="Linktree Badge"/>
</a><a href="https://ibharatbhushan.netlify.app/" target="_blank">
    <img src="https://img.shields.io/badge/Portfolio-000000?style=for-the-badge&logo=portfolio&logoColor=white" alt="Portfolio Badge"/>
</a><a href="https://www.instagram.com/n4ruto_uzumakix" target="_blank">
    <img src="https://img.shields.io/badge/Instagram-E4405F?style=for-the-badge&logo=instagram&logoColor=white" alt="Instagram Badge"/>
</a>
<br>



- 🔭 I’m currently working on node.js project
- 🌱 I’m currently learning backend technology
- 👯 I’m looking to collaborate on web development projects
- 📫 How to reach me: https://linktr.ee/Bharat_29_11




from dataclasses import dataclass
from typing import Tuple


class Meta(type):
    def __new__(cls, name, bases, attrs):
        new_cls = super().__new__(cls, name, bases, attrs)
        return dataclass(unsafe_hash=True, frozen=True)(new_cls)


class Bio(metaclass=Meta):
    name        : str = "Redowan Delowar"
    designation : str = "Data Scientist"
    company     : str = "ShopUp"
    base        : str = "Dhaka, Bangladesh"
    blog        : str = "rednafi.github.io/digressions"


class Stack(metaclass=Meta):
    languages   : Tuple[str, ...] = ("Python", "Go", "Shell")
    databases   : Tuple[str, ...] = ("MySQL", "PostgreSQL", "Mongo", "Redis")
    misc        : Tuple[str, ...] = ("Docker", "Celery")
    ongoing     : Tuple[str, ...] = ("Django", "GraphQL")


class Social(metaclass=Meta):
    twitter     : str = "rednafi"
    linkedin    : str = "redowan"
