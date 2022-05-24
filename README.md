# WCSNG UCSD Group Webpage

### Updates

#### July 21
1. Fix research and publication pages. It looks asthetically better now. Some links are fixed. Added paper pdf from the server.
2. Update news- ECCV paper, mmNets paper, and Blubble 
3. Team members- alumni page, New SRIP students


### Document
Note: one time change in `_config.yml`, when you want to host the webpage at `wcsng.github.io/wcsng`.
```
baseurl: "/wcsng"
```

Clone the repository. Install Jekyll. Run webpage on local server.
```
bundle exec jekyll serve
```

This command builds the webpage in the `_site` folder with all the html, CSS, and files for your localserver. Use:
```
bundle exec jekyll build
```
to build the webpage in the `_site` that can be used for your webserver. Just add, commit, and push the content to Github OR copy it to your webserver.


How to edit the contents:

Directory `_Data` 
* `publist.yml` to add new paper index (title, abstract, authors, link).
* `research_list` six research categories details
* `students.yml` for masters students, `colaborations` and `alumni`
* `team_member.yml` for PhDs
* `news.yml`
* `pictures` add all jpg image list

Directory `_pages`:
A standard template for all pages
```
title: "WCSNG - Research"
layout: gridlay
excerpt: "WCSNG -- Research"
sitemap: false
permalink: /research/
```
* Dir `Research`: One page each for each research topics (6 of them)
* `team.md`: ALumni and interns
* `home`: Logo and first page items. Slider photos.

Directory `_includes`: to updata html files for header ("WCSNG @ UC San Diego"), footer, analytics, and news

Directory `_layouts`: `homelay.html` has "Welcome to WCSNG" message. Other files not useful.

## Installing Jekyll on Ubuntu

```
sudo apt-get install ruby-full build-essential zlib1g-dev

echo '# Install Ruby Gems to ~/gems' >> ~/.bashrc
echo 'export GEM_HOME="$HOME/gems"' >> ~/.bashrc
echo 'export PATH="$HOME/gems/bin:$PATH"' >> ~/.bashrc
source ~/.bashrc

gem install jekyll bundler
```

Now check the `Gemfile.lock` file for the correct version number of the bundler and install it. For example, if file says it was `BUNDLED WITH 2.0.2`, then run:

```
gem i bundler -v 2.0.2
``` 

Install all required gems:

```
bundle install
```


## Copyright and Source

Forked from **Allan Lab Website** `https://github.com/mpa139/allanlab`. Code released under the MIT License.

<!--This is the website of our academic research group at Leiden University.

This website is powered by Jekyll and some Bootstrap, Bootwatch. We tried to make it simple yet adaptable, so that it is easy for you to use it as a template. Plese feel free to copy and modify for your own purposes.  You don't have to link to us or mention us (but of course we appreciate it).

Go to *aboutwebsite.md*  to learn how to copy and modidy this page for your purpose. -->
