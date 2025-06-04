# OpenML-labs website

### Adding yourself to the team members

You must add yourself to [people.yml](https://github.com/openml-labs/website/blob/main/people/people.yml) and indicate your name, position, a short description and a picture.
Resizing your portrait picture to 160x200 and compressing it into WebP format with [squoosh](https://squoosh.app/) is strongly recommended.

### Adding publications and software

You can add publications here: [publications.yml](https://github.com/openml-labs/website/blob/main/research/publications.yml) and softwares here:
[softwares.yml](https://github.com/openml-labs/website/blob/main/software/software.yml)

The picture used in the gallery will be matched based on the name in the `yaml` file.
For example, this entry:
```yaml
amlb:
  title: "AMLB: An AutoML Benchmark"
  authors:
    - P. Gijsbers
  ...
```
Will use image `images/papers/amlb.webp` or `.png`.

### Adding a blog post

Blog posts in the form of a Jupyter notebook can be added to the `notebooks` folder. However, you must add a "raw" cell at the top of the notebook and fill it with the following content:

```
---
title: Example of jupyter notebook for Quarto
topic: Example
author: Alexis Cvetkov-Iliev
date: 2025-06-30
format:
  html:
    code-fold: false
preview: Text that is displayed on the blog overview page.
image: amlb/amlb-boat-or-car.webp # image in the images/blogs subdirectory
---
```

The `topic` field is used to group similar posts into sections. In each section, the most recent posts are on top. Note that Quarto won't run again the code, so you must run everything before adding the notebook. An example of blog post is given [here](https://github.com/openml-labs/website/blob/main/notebooks/example.ipynb).
The `date` is in year-month-day format.
