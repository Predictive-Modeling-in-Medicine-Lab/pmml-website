  ![on-push](../../actions/workflows/on-push.yaml/badge.svg)
  ![on-pull-request](../../actions/workflows/on-pull-request.yaml/badge.svg)
  ![on-schedule](../../actions/workflows/on-schedule.yaml/badge.svg)

# The Predictive Modeling in Medicine Lab Website

This repository contains the source code for the website of **The Predictive Modeling in Medicine Lab**, run by **Dr. Charles Taylor** at **The University of Texas at Austin**.  
The website is publicly available at: **[michaelkapteyn.github.io/taylor-lab-website](https://michaelkapteyn.github.io/taylor-lab-website)**

Our website is built using the [**Lab Website Template**](https://github.com/greenelab/lab-website-template) developed by the Greene Lab.  

Full documentation for the template, including advanced configuration and customization options, is available here:  
👉 https://greene-lab.gitbook.io/lab-website-template-docs/

This README provides a quick-start guide for lab members who want to make simple edits, add content, and contribute changes.


---

## 🧑‍💻 Getting Started
*(Adapted from: [Preview your site locally](https://greene-lab.gitbook.io/lab-website-template-docs/getting-started/preview-your-site#on-your-computer-locally))*

### 1. Clone the Repository

```bash
git clone https://github.com/michaelkapteyn/taylor-lab-website.git
cd website
```

### 2. Run the website via docker

1. Install [Docker Desktop](https://www.docker.com/products/docker-desktop/) (recommended) or just [Docker](https://docs.docker.com/get-docker/) and start it.
2. Run `./.docker/run.sh`.
3. Wait for Docker to build a sandbox with all the languages and packages the template needs. Should take \~2 min the first time and be almost instant on subsequent runs.
4. Wait for Docker to start the preview. You should shortly get a `localhost` link that you can open in your browser to see your site preview.
5. When you make a change to a file in your repo folder, your preview should refresh/update automatically, except for changes to `_config.yaml` which require you to manually refresh.
6. When you make a change to your sources or metasources, the [cite process](../basics/citations.md) should automatically re-run, and when finished be reflected in your preview via the same behavior as above.

### 3. Preview the website in your browser
You should see a live preview at 
```
http://localhost:4000
```
The site will automatically reload as you make edits.  


---

## 🚀 Contributing Your Changes

1. Create a new branch for your edits:

   ```bash
   git checkout -b feature/your-change
   ```

2. Make your edits (see sections below for how to add content).
3. Commit your changes:

   ```bash
   git add .
   git commit -m "Add/update content"
   ```

4. Push your branch to GitHub:

   ```bash
   git push origin feature/your-change
   ```

5. Open a **Pull Request (PR)** on GitHub.  
   Your changes will be reviewed and approved by a lab admin, at which before being merged into the main branch and pushed to the live site.

---

## 🧩 Adding Content

### 🧠 Adding a New Research Project

To add a new project:

1. Open up `_data/projects.yaml`
2. Add a new section for your project, following the format of previous projects. This should create a card for the project on the `research` page.
3. [Optional] If you would like to add a more detailed writeup as a standalone page, e.g., `/research/my-project`, create a new markdown file under `research/my-project/index.md`, and then update your `projects.yaml` with
```
link : /research/my-project
```
This should make the card on the Research page link to your detailed writeup.
---

### 👥 Adding a New Team Member

To add a new team member:

1. Create a new Markdown file in the `_members` directory.  
   Example: `_members/jane-doe.md`. You should be able to follow the template given by other files in the `_members` directory

2. Commit and open a PR with your addition.

See the full documentation:  
https://greene-lab.gitbook.io/lab-website-template-docs/basics/team-members


---

### 📝 Adding a New Blog Post

To add a new blog post:

1. Create a new Markdown file in the `_posts` directory.  
   Example: `_posts/2025-10-01-new-results.md`. You should be able to follow the template given by other posts in the `_posts` directory.

3. Commit your changes and open a PR for review.

See the full documentation:  
https://greene-lab.gitbook.io/lab-website-template-docs/basics/blog-posts


---

## 🧭 Additional Resources

- 📘 Full template documentation: [https://greene-lab.gitbook.io/lab-website-template-docs/](https://greene-lab.gitbook.io/lab-website-template-docs/)
- 🐙 Original GitHub repo: [https://github.com/greenelab/lab-website-template](https://github.com/greenelab/lab-website-template)
- 🧩 Configuration guide: [https://greene-lab.gitbook.io/lab-website-template-docs/configuration/](https://greene-lab.gitbook.io/lab-website-template-docs/configuration/)

---

## 📄 License

This website is derived from the [Greene Lab Website Template](https://github.com/greenelab/lab-website-template)  
and distributed under the same open-source license.

---

*Maintained by The Predictive Modeling in Medicine Lab at The University of Texas at Austin.*
