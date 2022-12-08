# ViTASD: A novel dataset and method for Vietnamese Targeted Aspect-based Sentiment Analysis (ViTASA)

Table of Contents
=================

  * [General Introduction](#General)
    * [Data Example](#openstack)
    * [Usage](#Usage)
    * Citation

### 👨🏻‍💻 &nbsp;About Me

💡 &nbsp;I like to explore new technologies and develop software solutions and quick hacks.\
🎓 &nbsp;I'm currently studying Computer Science and Mathematics at the University of Massachusetts Amherst.\
🌱 &nbsp;I'm on track for learning more about Artificial Intelligence, Systems Design, and Cloud Architecture.\
✍️ &nbsp;In my free time, I pursue Graphic Design and Blog Writing as hobbies/side hustles.\
💬 &nbsp;Feel free to reach out to me for pro bono consulting and volunteering, or just for some interesting discussion.\
✉️ &nbsp;You can shoot me an email at avsingh@umass.edu! I'll try to respond as soon as I can.\
📄 &nbsp;Please have a look at my [Résumé](https://www.adityavsingh.com/resume.html) for more details about me. I'm open to feedback and suggestions!

<img alt="Night Coding" src="https://raw.githubusercontent.com/AVS1508/AVS1508/master/assets/Night-Coding.gif" align="right"/>

### 🛠 &nbsp;Keywords & Tech Stack

![Vietnamese TASA](https://img.shields.io/badge/%20-Vietnamese%20TASA-05122A?logo=data:image/png;base64,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)&nbsp;
![Huggingface](https://img.shields.io/badge/🤗-Huggingface-05122A)&nbsp;
![Pytorch](https://img.shields.io/badge/-Pytorch-05122A?style=flat&logo=pytorch)&nbsp;
![Python](https://img.shields.io/badge/-Python-05122A?style=flat&logo=python)&nbsp;
![Flask](https://img.shields.io/badge/-Flask-05122A?style=flat&logo=flask)&nbsp;
![HTML](https://img.shields.io/badge/-HTML-05122A?style=flat&logo=HTML5)&nbsp;
![CSS](https://img.shields.io/badge/-CSS-05122A?style=flat&logo=CSS3&logoColor=1572B6)&nbsp;
![Git](https://img.shields.io/badge/-Git-05122A?style=flat&logo=git)&nbsp;
![GitHub](https://img.shields.io/badge/-GitHub-05122A?style=flat&logo=github)&nbsp;
![Markdown](https://img.shields.io/badge/-Markdown-05122A?style=flat&logo=markdown)\
![Visual Studio Code](https://img.shields.io/badge/-Visual%20Studio%20Code-05122A?style=flat&logo=visual-studio-code&logoColor=007ACC)&nbsp;

## Task description <a name="General"/>
ViTASD is a new benchmark dataset for evaluating Vietnamese Targeted Aspect-based Sentiment Analysis models. The ViTASA dataset consists of .... We divide the dataset randomly into training, development and testing sets with a ratio of 7:1:2.

## Dataset <hr/>
![example](https://user-images.githubusercontent.com/62872625/205845803-972a5f17-f558-43cb-bfb6-5df5a7279c0b.png)

## Usage <a name="Usage"/>

## Evaluation

## References 

## Citation
Please cite the following paper if you found it useful in your work.
```
@inproceedings{tran-etal-2023-vitasd-vietnamese,
    title = "ViTASA: Vietnamese Targeted Aspect-based Sentiment Analysis in Multiple Data Domains",
    author = "",
    booktitle = "",
    month = "",
    year = "",
    address = "",
    publisher = "",
    url = "",
    pages = "",
}
```

### ⚙️ &nbsp;GitHub Analytics

<p align="center">
<a href="https://github.com/AVS1508">
  <img height="180em" src="https://github-readme-stats-eight-theta.vercel.app/api?username=kh4nh12&show_icons=true&theme=algolia&include_all_commits=true&count_private=true"/>
  <img height="180em" src="https://github-readme-stats-eight-theta.vercel.app/api/top-langs/?username=kh4nh12&layout=compact&langs_count=8&theme=algolia"/>
</a>
</p>

### 🤝🏻 &nbsp;Connect with Me

<p align="center">
<a href="https://www.adityavsingh.com"><img src="https://img.shields.io/badge/-khanhtq.com-3423A6?style=flat&logo=Google-Chrome&logoColor=white"/></a>
<a href="https://www.linkedin.com/in/kh4nh12/"><img src="https://img.shields.io/badge/-Khanh%20Quoc%20Tran-0077B5?style=flat&logo=Linkedin&logoColor=white"/></a>
<a href="mailto:khanhtq@uit.edu.vn"><img src="https://img.shields.io/badge/-khanhtq@uit.edu.vn-D14836?style=flat&logo=Gmail&logoColor=white"/></a>
<a href="https://www.facebook.com/khanhos0412/"><img src="https://img.shields.io/badge/-Khanh Quoc Tran-1877F2?style=flat&logo=Facebook&logoColor=white"/></a>
<!-- <a href="https://www.pinterest.ca/AVS1508"><img src="https://img.shields.io/badge/-@AVS1508-BD081C?style=flat&logo=Pinterest&logoColor=white"/></a> -->
<!-- <a href="https://www.behance.net/AVS1508"><img src="https://img.shields.io/badge/-@AVS1508-1769FF?style=flat&logo=Behance&logoColor=white"/></a> -->
</p>

-----
