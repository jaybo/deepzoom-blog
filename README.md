# DeepZoom public repository

- Read the DeepZoom blog: [https://blog.deepzoom.com](https://blog.deepzoom.com)

- Report bugs and issues: [https://github.com/jaybo/deepzoom-blog/issues](https://github.com/jaybo/deepzoom-blog/issues)

- Join the discussion forum: [https://github.com/jaybo/deepzoom-blog/discussions](https://github.com/jaybo/deepzoom-blog/discussions)









### Drafts

_config.yml:  add the following to view future posts
future: true

Then in your _config.yml, make sure future posts are shown:
future: true
The draft: true flag doesn't do anything by itself in Jekyll — it's a signal to you (and optionally to your templates). If you want it visually marked, you could add a banner in a custom layout checking {% if page.draft %}.

### Testing

Ubuntu -20.04 (WSL)
/mnt/d/devGit/deepzoom-blog$     bundle exec jekyll serve --force_polling
