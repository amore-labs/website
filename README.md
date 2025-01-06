# OpenML-labs website

### Adding yourself to the team members

You must add yourself to [people.yml](https://github.com/openml-labs/website/blob/main/people/people.yml) and indicate your name, position, a short description and a picture.
Resizing your portrait picture to 160x200 and compressing it into WebP format with [squoosh](https://squoosh.app/) is strongly recommended.

### Adding publications and softwares

You can add publications here: [publications.yml](https://github.com/openml-labs/website/blob/main/research/publications.yml) and softwares here:
[softwares.yml](https://github.com/openml-labs/website/blob/main/software/software.yml)

### Adding a blog post

Blog posts in the form of a Jupyter notebook can be added to the `notebooks` folder. However, you must add a "raw" cell at the top of the notebook and fill it with the following content:

```
---
title: Example of jupyter notebook for Quarto
topic: Example
author: Alexis Cvetkov-Iliev
date: 08-03-2023
format:
  html:
    code-fold: false
---
```

The `topic` field is used to group similar posts into sections. In each section, the most recent posts are on top. Note that Quarto won't run again the code, so you must run everything before adding the notebook. An example of blog post is given [here](https://github.com/openml-labs/website/blob/main/notebooks/example.ipynb).

### Important notes
- For the blog post notebooks
  - The `date` field must be in the format `mm-dd-yyyy` , not `dd-mm-yyyy`
  - Convert the images to WebP format before adding them to the notebook
    - On mac, you can use ` for image in *.png; do magick "$image" "${image%.png}.webp";done` to convert all the images in the folder to WebP format. Replace `*.png` with the appropriate file extension if needed.