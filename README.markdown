Flickr Sidebar for Octopress
============================

Description:
------------
This plugin adds Flickr photos to the Octopress sidebar, with a few configurable options. It does 
not require Flickr API access as it uses their [badge script](http://www.flickr.com/badge.gne).

Files:
------

Place `flickr.html` in `source/_includes/custom/asides/`. Optionally copy the contents of  
`_styles.scss` to `sass/custom` for some basic styling (centered photos with 20px top margin). 

Configuration:
--------------

Add `custom/asides/flickr.html` to `default_asides:` in your `_config.yml`. If you want photos at
the top of the sidebar, add it to the beginning of the list.

Add the Flickr sidebar configuration options to your `_config.yml` at the bottom of "3rd Party 
Settings". You'll need your Flickr user id, which is different from your username. An easy way to
find your user id is [idgettr.com](http://idgettr.com).

```yaml
# Flickr Badge
flickr_user:			# user id (not username)
flickr_count:			# number of photos to show (example: 3)
flickr_display:			# random or latest
flickr_size:			# t (thumbnail), s (small square), m (medium)
flickr_source:			# user, user_tag, all, all_tag
flickr_tag:				# tagname - set if flickr_source is set to user_tag or all_tag
```

The `flickr_source:` setting can be:

* user (all user's public photos)
* user_tag (user's tagged photos),
* all (everyone's public photos)
* all_tag (all public photos tagged with tag)

Example/Demo
------------

See the bottom of the sidebar at [technokracy.net](http://technokracy.net), or the source
[on Github](https://github.com/chronon/octopress/tree/technokracy).
