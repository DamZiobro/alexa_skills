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

deploy: requirements configure
	ask deploy

dialog: 
	ask dialog

all: deploy dialog
