clinton.judy.io
===============

My personal site and resume. It is a single static HTML page.

The entire site conforms to the hResume microformat spec, so it is machine
parsable. The markup uses HTML5 and CSS3, and the layout is responsive from
phone widths up.

Build
-----

There is no build step. The site is plain HTML, CSS, and JavaScript.
`index.html` is the whole page. Edit it and reload the browser.

GitHub Pages serves the files exactly as they appear in this repo. The
`.nojekyll` file turns off server-side Jekyll processing.

Development
-----------

The tooling is optional. It gives you a local server and browser livereload.

Install Ruby 4.0.6. [mise](https://mise.jdx.dev) reads `.ruby-version`:

    mise install

Install the gems:

    bundle install

Start the local server and the livereload watcher together. `Procfile`
defines both processes, so use a process manager such as
[overmind](https://github.com/DarthSim/overmind) or `foreman`:

    overmind start

Open <http://localhost:4000>.

To run the processes separately, use two terminals:

    bundle exec ruby -run -e httpd . -p 4000
    bundle exec guard

`Guardfile` lists the watched paths. Guard reloads the browser when you
change `index.html`, `css/`, or `assets/`.

Layout
------

    index.html        the entire page
    css/custom.css    site-specific overrides
    assets/css/       theme stylesheets
    assets/js/        theme scripts
    assets/plugins/   vendored libraries (jQuery, Bootstrap, Modernizr)
    assets/images/    photos, logos, and backgrounds
    assets/docs/      the downloadable resume PDF
    CNAME             the custom domain for GitHub Pages

Deployment
----------

Push to `master`. GitHub Pages publishes the site to the domain in `CNAME`.

History
-------

I wrote the first version of this site in 2012 to solve three problems:

- I needed a resume, quickly.
- I wanted a working example of my information architecture, interface
  prototyping, and HTML5/CSS3/JS skills.
- I wanted to get better at microformats.

I gave myself a full week and finished in about 32 hours. I have redesigned
and rewritten it since then, but the goals have not changed. A great resume
is never boring, and the aesthetics must never get in the way of the content.

### - Clinton Judy
