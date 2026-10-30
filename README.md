# DeepZoom public repository

- Read the DeepZoom blog: [https://blog.deepzoom.com](https://blog.deepzoom.com)

- Report bugs and issues: [https://github.com/jaybo/deepzoom-blog/issues](https://github.com/jaybo/deepzoom-blog/issues)

- Join the discussion forum: [https://github.com/jaybo/deepzoom-blog/discussions](https://github.com/jaybo/deepzoom-blog/discussions)




### Using dev vs poduction DeepZoom

# Host for embedded DeepZoom iframes in posts. Switch to test the staging site:
# deepzoom_host: "https://deepzoom-test.azurewebsites.net"
deepzoom_host: "https://www.deepzoom.com"


### Drafts

_config.yml:  add the following to view future posts
future: true

Then in your _config.yml, make sure future posts are shown:
future: true
The draft: true flag doesn't do anything by itself in Jekyll — it's a signal to you (and optionally to your templates). If you want it visually marked, you could add a banner in a custom layout checking {% if page.draft %}.

### Thenes and styling

Use assets/css/main.scss. Jekyll compiles it into /assets/css/main.css on every build, both locally and on GitHub Pages, so the main.css you see in _site is generated output and isn't kept in the repo anymore.

main.scss contains only your customizations. The rest of the stylesheet comes from the theme set in _config.yml (remote_theme: mmistakes/minimal-mistakes@4.24.0, with minimal_mistakes_skin: contrast). To change the site's look, edit main.scss: theme variables like $sans-serif go above the @import "minimal-mistakes" line, and ordinary CSS rules go below it.

### Testing

Ubuntu -20.04 (WSL)
/mnt/d/devGit/deepzoom-blog$     bundle exec jekyll serve --force_polling
