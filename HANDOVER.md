# How to update this portfolio

This guide is written for someone with no programming experience.

Everything on the website is edited through the GitHub website in your browser.
You never need to install anything, and you never need to write code.

After you save a change, the website updates itself automatically.
It usually takes about one minute.

---

## 1. The three things you need to know first

**The website address**

`https://student-research-portfolios.github.io/diego-romero/`

**Where the website lives**

All the files are stored in a GitHub repository.
Sign in at [github.com](https://github.com) with the account created for you, and open the repository named `diego-romero`.

**The two folders you will use**

| Folder | What is inside |
|---|---|
| `_projects` | One file per project. This is where all the project text lives. |
| `assets/img` | All the photographs, grouped into one folder per project. |

Everything else in the repository is the design of the site.
You do not need to open those files, and it is best not to change them.

---

## 2. How to change text

1. Open the `_projects` folder.
2. Click the file for the project you want to change, for example `2-automated-food-service-module.md`.
3. Click the pencil icon in the top right corner.
4. Find the text you want to change and type over it.
5. Scroll to the bottom and click the green **Commit changes** button.

That is all.
Wait about a minute, then refresh the website to see the change.

### What the top part of the file means

Every project file begins with a block between two lines of three dashes.
That block holds the short pieces of information that appear on the landing page and at the top of the project page.

```
order: 2
field: Food-Service Automation
title: "Automated Food-Service Module: An Engineering Concept for Improving Service Efficiency"
```

You can change any of the values after the colon.

**Two rules that matter.**

If your text contains a colon followed by a space, put the whole line inside double quotation marks, exactly as the `title` line above does.
Without the quotation marks the site will fail to build.

Never change the spacing at the start of a line.
The indentation is meaningful.

### The rest of the file

Below that block is the body of the page.
Ordinary sentences are just typed normally.
A line that begins with `##` is a section heading.

You will also see blocks that look like this:

```html
<li><strong>Reaction time</strong> 60.0 ± 0.1 minutes per trial.</li>
```

These build the boxes and tables on the page.
You can safely change the words, but leave the pointed brackets and everything inside them exactly as they are.

---

## 3. How to replace a photograph

1. Open `assets/img` and then the folder for that project.
2. Note the exact file name of the photo you want to replace, for example `fig1-analytical-balance.jpg`.
3. Click **Add file** then **Upload files**, and upload your new photo.
4. Rename your new file to exactly the same name as the old one.

Because the name is the same, the page picks the new photo up automatically and you do not need to change any text.

If you would rather use a different file name, upload the photo, then open the project file and replace the old name with the new one wherever it appears.

---

## 4. How to add a Zenodo link or DOI

This is the step you will do after publishing each project on Zenodo.

1. Open the project file in `_projects`.
2. Near the top you will find lines like this:

```
doi: ""
buttons:
  - label: View Full Research Paper
    url: ""
```

3. Paste the Zenodo link between the two quotation marks after `url:`.
4. Paste the DOI between the two quotation marks after `doi:`.
5. Commit the change.

The buttons at the bottom of the project page become active links immediately.
Until you do this, they appear greyed out and say "link pending", which is intentional.

---

## 5. How to add a new project

Adding a project is a matter of copying an existing one.

1. Open the `_projects` folder and open any existing project file.
2. Select all the text and copy it.
3. Go back to the `_projects` folder, click **Add file**, then **Create new file**.
4. Name the file using the next number, for example `4-water-remediation-biochar.md`.
5. Paste in what you copied, then replace the text with the new project's content.
6. Change the `order:` number to the position you want the project to appear in.
7. Create a new folder inside `assets/img` for that project's photographs and upload them.
8. Commit the change.

The new project appears on the landing page automatically.
You do not need to edit the landing page itself.

### Removing the "In preparation" placeholder

The fourth project currently shows on the landing page as a greyed-out card.
That card is defined in the file `_data/upcoming.yml`.
Once the real project page exists, delete the entry from that file so the placeholder disappears.

---

## 6. How to create a portfolio for a different student

This is the part that makes the model reusable.

1. Open the `diego-romero` repository on GitHub.
2. Click the **Use this template** button, then **Create a new repository**.
3. Set the owner to `student-research-portfolios`, make the repository **Public**, and name it after the student, for example `maria-lopez`.
4. In the new repository, open `_config.yml` and change:
   - `student_name` to the new student's name
   - `site_subtitle` and `site_strapline` to describe their projects
   - `baseurl` to `"/maria-lopez"`, matching the new repository name
5. Delete the project files in `_projects` and the image folders in `assets/img`, then add the new student's material.
6. In the repository **Settings**, open **Pages** and set the source to the `main` branch.

The new portfolio is then live at `https://student-research-portfolios.github.io/maria-lopez/`.

The design, layout and structure carry across automatically.
Only the content changes.

### Giving a student control of their own portfolio

Each student's portfolio is a separate repository, so control can be given one student at a time.

1. The student creates their own free GitHub account.
2. Open their repository, then **Settings**, then **Collaborators and teams**.
3. Click **Add people**, enter the student's GitHub username, and choose the **Admin** role.

The student can then edit and manage their portfolio, and the website address stays the same.
Access to their Zenodo records can be shared the same way, from the **Share** button on each record.

---

## 7. If something goes wrong

**The website does not update after a change.**

Open the **Actions** tab in the repository.
A red cross means the site failed to build, which is almost always a punctuation mistake in the block at the top of a project file.
Look for a missing quotation mark, or a line whose indentation was changed.

**You want to undo a change.**

Open the **Commits** history, find the change you want to reverse, and click **Revert**.
Nothing is ever permanently lost.

**A photograph does not appear.**

Check that the file name in the text matches the uploaded file exactly, including whether the extension is `.jpg` or `.png`.
File names are case-sensitive: `Fig1.jpg` and `fig1.jpg` are treated as different files.

---

## 8. What not to change

These files control how the site looks and behaves.
Changing them can break every page at once.

- `_layouts/`
- `assets/css/style.css`
- The `url` and `baseurl` lines in `_config.yml`, unless you are moving the site

If you want a design change rather than a content change, that is a job for whoever maintains the site.

---

## 9. Accounts and where things live

| What | Where |
|---|---|
| Website files and hosting | GitHub organisation `student-research-portfolios`, repository `diego-romero` |
| Published research records | Zenodo, signed in with the same GitHub account |
| Administrator account | GitHub user `researchportfolio-admin` |

There is no hosting bill, no domain renewal and no subscription.
GitHub Pages hosts public project sites free of charge, and Zenodo is operated by CERN as a free open research repository.
