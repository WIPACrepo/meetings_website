# meetings_website
meetings.wipac.wisc.edu

## Editing

After cloning the repo, you should set up a local environment:

```bash
./setupenv.sh
. env/bin/activate
mkdocs serve
```

This should start a live preview at [http://localhost:8000](http://localhost:8000).
It should automatically update whenever you save any file in the `docs`
directory.

The Markdown source exists in `docs` and uses [mkdocs](https://www.mkdocs.org/).

### Adding a Page

Add your page in [markdown format](https://www.mkdocs.org/user-guide/writing-your-docs/#writing-with-markdown)
inside the `docs` directory. If adding an image, the url should be relative.

Then insert the new page into the nav bar by editing `mkdocs.yml`.
The `nav:` section is set up as explained
[here](https://www.mkdocs.org/user-guide/writing-your-docs/#configure-pages-and-navigation).

## Publishing

There is a GitHub action configured to deploy any changes to `main`.
Either commit directly to `main` or go through the PR process and your
changes will appear a minute or two after the merge.
