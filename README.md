# SpaceONE Developer Guides

Welcome to the SpaceONE Developer Guides!

# Test in local

To test the generated document.

~~~bash
mkdocs serve --dev-addr=0.0.0.0:80
~~~

Open web browser with http://localhost

# Build and upload

Build document then upload to spaceone-dev.github.io

~~~bash
cd ..
git clone https://github.com/spaceone-dev/spaceone-dev.github.io
cd spaceone-dev.github.io
mkdocs gh-deploy --config-file ../developer/mkdocs.yml --remote-branch master
~~~
