# Form

Allow users to enter data.

### Text input
| Class | Example |
| -- | -- | 
| input |<div class="db"><div class="form"><label>Cluster Name<i class="fa fa-question-circle"></i></label><input type="text" class="form-control" placeholder="Required" /></div>|
| input disabled |<div class="db"><div class="form"><label class="disabled">User Name<i class="fa fa-question-circle"></i></label><input type="text" class="form-control" placeholder="Required" disabled/></div>|
| input error |<div class="db"><div class="form"><label>Cluster Name<i class="fa fa-question-circle"></i></label><input type="text" class="form-control error" value="DuplicatedName"/><span class="errormessage">Error messages.</span></div>|

**When to use**

* Use in forms to take input from users. 

**Interaction**

* Required and optional 
* Hint: appear on the right side of the input field to provide more context.
* Autofocus


### Select

| Class | Example |
| -- | -- | 
| Select |<div class="db"><div class="form"><label>Databricks Runtime Version<i class="fa fa-question-circle"></i></label><Select defaultValue="lucy"><Option value="jack">3.4 beta (GPU, Scala 2.11) </Option><Option value="lucy">3.4 beta (Scala 2.11)</Option><Option value="disabled" disabled>Disabled</Option><Option value="Yiminghe">yiminghe</Option></Select></div>|
| Select disabled |<div class="db"><div class="form"><label>Databricks Runtime Version<i class="fa fa-question-circle"></i></label><Select defaultValue="lucy" disabled><Option value="jack">3.4 beta (GPU, Scala 2.11) </Option><Option value="lucy">Lucy</Option><Option value="disabled" disabled>Disabled</Option><Option value="Yiminghe">yiminghe</Option></Select></div>|
| Select disabled |<div class="db"><div class="form"><label>Databricks Runtime Version<i class="fa fa-question-circle"></i></label><Select defaultValue="lucy" class="error"><Option value="jack">3.4 beta (GPU, Scala 2.11) </Option><Option value="lucy">Lucy</Option><Option value="disabled" disabled>Disabled</Option><Option value="Yiminghe">yiminghe</Option></Select><span class="errormessage">Error messages.</span></div>|


**When to use**

* Select a single or multiple options from a list in a drop menu. Use when you have 6-15 options.
* single-select: select one from a list.
* multi-select: allow users to select multiple options.

**Interaction**

* Default value
* Type a head.
* Group options into sections.


### Checkboxes

| Class | Example |
| -- | -- | 
| Checkbox |<div class="db"><div class="form"><input type="checkbox" id="spotInstance" name="subscribe" value="newsletter"><label for="spotInstance" class="inlineLabel">Use spot instance</label></div>|
| Checkbox disabled |<div class="db"><div class="form"><input type="checkbox" id="spotInstance" name="subscribe" value="newsletter" disabled><label for="spotInstance" class="inlineLabel">Use spot instance</label></div>|


**When to use**

* Allow users to select multiple options, each option is independent of all other options. E.g., autoscaling and auto-termination.
* Turn an option on or off, e.g., Do not show me again.

**Interaction**

* Check and uncheck.
* Use positive and active wording for checkbox labels. 
* Default value 


### Radio button

| Class | Example |
| -- | -- | 
| Radio Button |<div class="db"><div class="form"><input type="radio" id="contactChoice1" name="contact" value="email" checked><label for="contactChoice1" class="inlineLabel">Link</label><input type="radio" id="contactChoice2" name="contact" value="phone"><label for="contactChoice2" class="inlineLabel">Unlink</label></div>|
| Radio Button disabled |<div class="db"><div class="form"><input type="radio" id="contactChoice1" name="contact1" value="email" checked disabled><label for="contactChoice1" class="inlineLabel">Link</label><input type="radio" id="contactChoice2" name="contact1" value="phone" disabled><label for="contactChoice2" class="inlineLabel">Unlink</label></div>|

**When to use**

* Select a single option from a set of options.
* All options are visible 

**Interaction**

* Select one deselect the other   
* Default value 


### Switch / Toggle

**When to use**

* On or off option, e.g., enable and disable 

**Interaction**

* Turn on and turn off.  


### Text Area

| Class | Example |
| -- | -- | 
| Text Area |<div class="db"><div class="form"><div class="form"><label>Spark Config<i class="fa fa-question-circle"></i></label><textarea name="textarea"></textarea></div>|

**When to use**

* Todo

**Interaction**

* Todo

### Styles for the form

```less
.form{

	.text-basic;
		
	label{
		font-weight: @font-weight-bold;
		color: @text-tertiary-color;
		display: block;
		margin-bottom: @spacing-small;

		.fa{
			margin-left: @spacing-small;
		}
	}

	input, select, textarea {
		border: 1px solid @border-dark;
		border-radius: @border-radius-base;
		height: @height-item;
		width: @width-item-base;
		box-shadow: inset @box-shadow;
		padding: @spacing-small @spacing-base;

		&::placeholder {
		  color: @text-tertiary-color;
		}

		&:focus { 
		    border-color: @blue-200;
		    outline: 0px;
		    .box-shadow(0px; 1px; 3px; @blue-200; @disabled-opacity-small);
		}

        &.disabled, &[disabled], &.disabled:hover {
        	background-color: @gray-200;
        	cursor: not-allowed;
            opacity: @disabled-opacity-base;
        }

        &[type=checkbox], &[type=radio]{
        	width:auto;
        	height: auto;
        	margin-right: @spacing-small;
        }

        &[type=radio]{
        	display: inline-block;
        }
	}

	textarea{
		width: @width-item-max;
		height: @height-textarea;
	}

	.error{

        background-color: @red-100;

        &:focus { 
		    border-color: @red-200;
		    outline: 0px;
		    .box-shadow(0px; 1px; 3px; @red-200; @disabled-opacity-small);
		}
     }

     .errormessage{
     	.text-error;
     	margin-left: @spacing-base;
     }

     .inlineLabel{
     	color: @text-basic-color;
     	font-weight: @font-weight-base;
     	display:inline-block;
     	margin-right: @spacing-large;
     }

}
```

### References

[https://uxdesign.cc/design-better-forms-96fadca0f49c](https://uxdesign.cc/design-better-forms-96fadca0f49c)

