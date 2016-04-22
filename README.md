jQuery plugin creating customizable input radio buttons

###DEMO: http://marioiliev.com/demos/radio-buttons/

#	Initialize the plugin (two options):
	1. Call the plugin on element containing radio buttons - $(selector).customRadio();
	2. Add "data-radio-custom" tag on <div> containing radio buttons and the plugin will run with the default options

#	Radio button text:
	If no additional paramters are specified, the plugin will take the radio input value text
	Available options for "text:" are: 'empty', 'value', 'title' or custom 'data' type value. 
	Example: $(selector).customRadio({text: 'data-custom-title'});

#	Disable radio buttons:
	$(selector).customRadio({disabled: true});
	- the <label> wrapper gets "disabled" class selector

#	To destroy the plugin:
	$(selector).customRadio({destroy: true});

#	Styling:
	Each radio button is wrapped in <label> element with the following class selectors:
	"radio_btn"
	"selected" (when button is clicked)
	"radio_#"  ("#" is uniqe number for each radio button)
	
	"customClass:" You can add custom class selector: 
	-	$(selector).customRadio({customClass: 'myclass'});

	Each Label contains <span> with the text of the radio button
