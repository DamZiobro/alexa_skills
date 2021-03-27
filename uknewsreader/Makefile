#
# Makefile
# damian, 2021-03-23 14:49
#

requirements:
	sudo npm install -g ask-cli || true
	touch $@

configure:
	ask configure
	touch $@

new:
	ask new
	touch $@

copy-assets:
	cp skill-package/assets/en-US_largeIcon.png skill-package/assets/en-GB_largeIcon.png
	cp skill-package/assets/en-US_smallIcon.png skill-package/assets/en-GB_smallIcon.png
	cp skill-package/interactionModels/custom/en-US.json skill-package/interactionModels/custom/en-GB.json


deploy: requirements configure new copy-assets
	ask deploy

dialog: 
	ask dialog

all: deploy dialog

