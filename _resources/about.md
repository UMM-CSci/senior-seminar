---
title: About This Site
order: 11
---

# About This Site

This site uses [Jekyll](https://jekyllrb.com/) and is hosted on [GitHub Pages](https://pages.github.com/). 

| Repository: [{{site.github.repository_nwo}}]({{site.github.repository_url}}) | Current build: [{{ site.github.build_revision | slice:0,7 }}]({{site.github.repository_url}}/commit/{{site.github.build_revision}}) |

## Other Pages

These are some extra pages not in the main navigation:

- [Current schedule for printing]({{site.baseurl}}/current-schedule)

## Contributing

If you want to contribute to this site, fork [the repository]({{site.github.repository_url}}), make your changes, and then make a pull request back to this repo! There are also "Edit on GitHub" buttons throughout the site you can use to quickly edit and make a pull request for a specific page.

There is information on how to run the site locally in the [README]({{site.github.repository_url}}/blob/master/README.md#running-locally).

## Seminars Format

A seminar is a single senior seminar event for a specific semester and year. They are directories stored in the `_seminars` directory. An example would be `_seminars/spring2018`. In that directory is an `index.md` file and all of the PDFs for the seminar.

The `index.md` file contains [YAML front matter](https://jekyllrb.com/docs/front-matter/) that defines papers and slides as well as other data about the seminar. Under that, in the content area is any general text to be displayed in the seminar.

Here is a truncated example of the `index.md` from Spring 2018:

```md
---
title: "Spring 2018"
year: 2018
semester: spring

papers:
  - title: Recent Advancements in Cloud Security
    author: Matt Mitchell
    time: 2018-04-15 3:30 PM
    room: Sci 3610
    slides: mitchellslides.pdf
    pdf: mitchell.pdf
     
  - title: Road Segmentation with Neural Networks
    author: Andy Lau
    time: 2018-04-15 3:00 PM
    room: Sci 3610
    slides: lauslides.pdf
    distinctionpaper: true
    pdf: lau.pdf
     
  - title: Querying Large Databases
    author: Nathan Beneke
    time: 2018-04-15 2:00 PM
    room: Sci 3650
    distinctionslides: true
    slides: benekeslides.pdf
    distinctionpaper: true
    pdf: beneke.pdf
---

The CSci discipline invites you to Spring 2018 Senior Seminar conference...
```

The front matter contains an array of papers named `papers`. The papers don't need to be in a specific order. Each paper in the `papers` array can have these attributes:
- `title` (required) - the title of the paper
- `author` (required) - the author of the paper
- `time` - the date and time they will present at the seminar
- `room` - the room they will present in
- `slides` - the filename of the pdf of the slides from the presentation
- `slidesurl` - the URL to the slides if there isn't a PDF of them
- `distinctionslides` - `true` if the presentation got a distinction (&#x2B50;)
- `pdf` - the filename of the PDF of the paper
- `distinctionpaper` - `true` if the paper got a distinction (&#x2B50;)

## Resources Format

Senior seminar resources are markdown files stored in the `_resources` directory. They have only two things in their [front matter](https://jekyllrb.com/docs/front-matter/):
- `title` - the title of the resource to be displayed in the sidebar and browser tab.
- `order` - an integer that determines where in the sidebar list the resource will be displayed. It is displayed least `order` first.

Here is an example:
```md
---
title: About This Site
order: 10
---

# About This Site

This site uses [Jekyll](https://jekyllrb.com/)...
```
