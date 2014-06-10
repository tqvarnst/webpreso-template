# Base code for Red Hat Presentations using PHP cartridge

This is base code for creating Red Hat presentation using PHP cartridge and Reveal.js.

To use this register on www.openshift.com or use OpenShift Enterprise/Origin then follow the below steps.


1. Create a new gear using the metadata/manifest.yml file in this repo like this:

		rhc app create -n <namespace> -a <appname> -t php-5.3 --from-code https://github.com/tqvarnst/webpreso-template.git

		
* Update index.html or another html file with your presentation. *For more tips and tricks see the example.html file* 

* Commit and push to your gear
	
		git commit -a -m "Commit comment" && git push origin
		
* Go to your openshift URL http://<appname>-<namespace>.rhcloud.com to the see the presentation. 

* To print the presentation to a pdf add ?print-pdf (e.g. [http://web-pres0.rhcloud.com?print-pdf](http://web-pres0.rhcloud.com?print-pdf)) to the url in Google Chrome and use the print function in Chrome.

For presentation mode etc it's recommmended to run the presentation locally. Follow the installation instructions [here](php/README.md).


