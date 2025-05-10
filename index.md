---
title: Welcome to my Portfolio
---
This is where you can view examples of my work including full projects, code snippets with use cases, and workflows.

<style>
  .filter-button {
    display: inline-block;
    padding: 5px 12px;
    margin: 4px;
    background-color: #f0f0f0;
    border-radius: 5px;
    text-decoration: none;
    font-weight: bold;
    color: #333;
    cursor: pointer;
    transition: background-color 0.3s;
  }
  .filter-button:hover {
    background-color: #cce7ff;
  }
  .project {
    transition: all 0.4s ease-in-out;
  }
</style>

<script>
function filterProjects(tag) {
  const projects = document.querySelectorAll('.project');
  projects.forEach(p => {
    const tags = p.getAttribute('data-tags');
    if (tags.includes(tag) || tag === 'All') {
      p.style.display = 'block';
      p.style.opacity = '1';
    } else {
      p.style.display = 'none';
      p.style.opacity = '0';
    }
  });
}
</script>

# Portfolio index.md template for GitHub Pages using Markdown

# My GIS & Data Portfolio

Welcome! Below are some of the projects I've worked on. Use the links below to jump to each project or filter by category:

### 🧩 Filter by Category
<a class="filter-button" onclick="filterProjects('All')">All</a>
<a class="filter-button" onclick="filterProjects('ArcGIS')">ArcGIS</a>
<a class="filter-button" onclick="filterProjects('Python')">Python</a>
<a class="filter-button" onclick="filterProjects('SQL')">SQL</a>

---

<div class="project" data-tags="ArcGIS Python">

## 🗺️ Project 1 <a name="project-1"></a>
**Title:** *Project Title Goes Here*

**Categories:** ArcGIS, Python

**Description:**
> _Write a few sentences describing what this project is about, what tools you used, and what your role was._

**Image:**
![Alt Text](path/to/your/image1.jpg)

**Live Demo or Repo:**
[View Project](https://your-project-link.com)

</div>
---

<div class="project" data-tags="SQL Python">

## 📊 Project 2 <a name="project-2"></a>
**Title:** *Project Title Goes Here*

**Categories:** SQL, Python

**Description:**
> _Add a description of your project. Mention your data sources, any analyses you performed, and final outcomes._

**Image:**
![Alt Text](path/to/your/image2.jpg)

**Live Demo or Repo:**
[View Project](https://your-project-link.com)

</div>
---

<div class="project" data-tags="ArcGIS SQL">

## 🌐 Project 3 <a name="project-3"></a>
**Title:** *Project Title Goes Here*

**Categories:** ArcGIS, SQL

**Description:**
> _Add your summary here. You might want to include challenges you overcame or technologies you explored._

**Image:**
![Alt Text](path/to/your/image3.jpg)

**Live Demo or Repo:**
[View Project](https://your-project-link.com)

</div>
---

<div class="project" data-tags="Python SQL ArcGIS">

## 🛰️ Project 4 <a name="project-4"></a>
**Title:** *Project Title Goes Here*

**Categories:** Python, SQL, ArcGIS

**Description:**
> _Write your description here. This section can include maps, data dashboards, or visual outputs._

**Image:**
![Alt Text](path/to/your/image4.jpg)

**Live Demo or Repo:**
[View Project](https://your-project-link.com)

</div>
---

### 📫 Contact
Feel free to connect with me via [LinkedIn](https://linkedin.com/in/your-profile) or [email](mailto:your@email.com).

*Last updated: {{ site.time | date: '%B %d, %Y' }}*
