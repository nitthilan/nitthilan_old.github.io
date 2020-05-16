# nitthilan.github.io
Learning to learn. What could happen if we can create machines which work like us. Plan to document this journey of what I learn


List of issues faced:
=====================
https://github.com/nitthilan/nitthilan.github.io
https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet

- https://github.com/fastlane/fastlane/issues/6203
- http://stackoverflow.com/questions/25151736/jekyll-2-2-0-error-address-already-in-use-bind2
- https://help.github.com/articles/setting-up-your-github-pages-site-locally-with-jekyll/#step-4-build-your-local-jekyll-site
- http://jekyllrb.com/docs/frontmatter/
- https://jekyllrb.com/docs/themes/#overriding-theme-defaults

Commands used:
==============
- bundle exec jekyll serve --watch --port 8000 --detach
- bundle exec jekyll serve --watch --port 8000 --detach
- pkill -f jekyll
- bundle exec jekyll build --watch => Autogeneration
- bundle exec jekyll build
- bundle exec jekyll build --drafts => to build drafts folder
bundle exec jekyll build
git add . 
git commit -m "New posts added"
git push -u origin master

bundle update
pkill -f jekyll
bundle exec jekyll serve --watch --port 8000 --incremental --detach


alias run_rsync='rsync -azP --progress --stats --exclude ".*/" --exclude ".*" --exclude "tmp/" //Users/kannappanjayakodinitthilan/Documents/myfolder/project_devan/aws_workspace/source/website/nitthilan.github.io njayakodi_dg@134.121.66.109:/local/data/nitthilan/source_code/website/'

run_rsync; fswatch -o Users/kannappanjayakodinitthilan/Documents/myfolder/project_devan/aws_workspace/source/website/nitthilan.github.io | while read f; do run_rsync; done


Fix for ffi:

brew reinstall libffi
