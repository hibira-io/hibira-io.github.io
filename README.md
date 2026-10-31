# hibira-io.github.io

The organization's GitHub Pages site, served at **https://demos.hibira.io**
(Settings → Pages → Custom domain). Its custom domain also applies to every
project site in hibira-io, so they are served under it:

- https://demos.hibira.io/examples/ — live demos ([hibira-io/examples](https://github.com/hibira-io/examples))
- https://demos.hibira.io/godot/ — Godot playground ([hibira-io/godot](https://github.com/hibira-io/godot))

The root page only redirects to the demos. `robots.txt` and `sitemap.xml`
at the root cover every project site: add a project's URL to `sitemap.xml`
when it starts publishing Pages. Link to demos.hibira.io, never to
hibira-io.github.io: Chrome flags that host as a lookalike of hibira.io.

The DNS record (`demos` CNAME → `hibira-io.github.io`, DNS only) is managed
in hibira-io/pusher-server (`infra/demo.tf`).
