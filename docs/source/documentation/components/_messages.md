<div class="panel panel-gray leader-1 trailer-1">
<mark class='label label-blue'>Calcite Web 2.0 Update</mark>
<p class='leader-half trailer-0 font-size--1'>
The dom structure of messages has changed. To migrate your messages, follow the structure below for arranging your elements.
</p>
</div>

messages are used to inform users of state changes, errors, or successful actions. messages are only visible if they have the `is-active` class. Without as `is-active` class, the message will be set to `display: none;`

Calcite Web does not manage class assignment, invocation, or dismissal logic for messages - you will have to write your own JavaScript handlers for this.

An message can consist of up to three children - `message-icon`, `message-content`, and `message-close`. At a minimum, an message must contain an `message-content` child.  

#### Example
It's recommended to pair a status icon with your message. Pairing an message status with an icon helps reinforce the intent of the message, and ensures accessibility.
<div class="column-17">
 
  <div class="column-8">
  <div class="panel panel-white">
 <h5 class="font-size-1">My great form</h5>
<h6 class="avenir-bold font-size--3 light-gray">SECTION 1</h6>

<label>
  First Name
  <input type="text"  value="Tom" required>
</label>
<label>
  Last Name
  <input type="text"  value="Wafflestein" required>
</label>
 <div class="message is-active">
 <div class="message-icon">
  {% icon 'information', style='filled' %}
</div>
  <div class="message-content">
  Manage your members' licenses on this page. <a class="btn-link font-size--1">Show more.</a>
  </div>
  <button class="message-close" aria-label="Close">
    {% icon 'x' %}
    </button>
    </div>
<label class="toggle-switch clearfix">
  <span class="toggle-switch-label left font-size--1">Enable Two-Factor Authentication</span>
  <input type="checkbox" class="toggle-switch-input" checked>
  <span class="toggle-switch-track right"></span>
</label>





<h6 class="avenir-bold leader-2 font-size--3 light-gray">SECTION 2</h6>


   Upload profile photo
    <div class="message is-active">
 <div class="message-icon">
  {% icon 'information', style='filled' %}
</div>
  <div class="message-content">
 This will be used throughout ArcGIS online as your avatar
  </div>
  <button class="message-close" aria-label="Close">
    {% icon 'x' %}
    </button>
    </div>
 
  <input type="file">


&nbsp;
  <fieldset class="fieldset-checkbox">
    <legend>Email Preferences (optional)</legend>
    <label>
      <input type="checkbox"> Weekly Newsletter
    </label>
    <label>
      <input type="checkbox"> Monthly Newsletter
    </label>
    <label>
      <input type="checkbox"> All Emails
    </label>
  </fieldset>
  <fieldset class="fieldset-radio">
    <legend>How did you hear about us? (optional)</legend>
    <label>
      <input type="radio" name="source" value="friend">Friend
    </label>
    <label>
      <input type="radio" name="source" value="event">Sponsored Event
    </label>
    <label>
      <input type="radio" name="source" value="other">Other
    </label>
  </fieldset>
  <label>

<h6 class="avenir-bold leader-2 font-size--3 light-gray">DANGER ZONE</h6>
   <div class="message message-red is-active">
 <div class="message-icon">
  {% icon 'information', style='filled' %}
</div>
  <div class="message-content">
 These settings are potentially dangerous. Proceed with caution!
  </div>
    </div>
<label class="toggle-switch toggle-switch-destructive clearfix">
  <span class="toggle-switch-label left font-size--1">Disable Two-Factor Authentication</span>
  <input type="checkbox" class="toggle-switch-input" >
  <span class="toggle-switch-track right"></span>

 
</label>








<h6 class="avenir-bold leader-2 font-size--3 light-gray">FORM EXAMPLES</h6>
<label>
  First Name
  <input type="text" value="Tom" required>
</label>
 <div class="message is-active">
  <div class="message-content">
  Some kind of dismissable message with no icon
  </div>
  <button class="message-close" aria-label="Close">
    {% icon 'x' %}
    </button>
    </div>
<label>
  Address
  <input type="text" value="123 Main St." required>
</label>

<label>
  First Name
  <input type="text"  value="Tom" required>
</label>

<label>
  Current Password
  <input type="text" required placeholder="Enter your current password">

</label>
<label>
 Something Else
  <input type="text"value="Tom" required>
</label>

  <button type="submit" class="btn">Submit</button>
</form>
</div>
 </div>
  <div class="column-1 tablet-first-column">&nbsp;
</div>
  <div class="column-8 tablet-first-column">
  <div class="panel panel-white">
 <h5 class="font-size-1">My great form</h5>
<h6 class="avenir-bold font-size--3 light-gray">SECTION 1</h6>

<label>
  First Name
  <input type="text"  value="Tom" required>
</label>

<label>
  Last Name
  <input type="text"  value="Wafflestein" required>
</label>
&nbsp;
<label class="toggle-switch clearfix">
  <span class="toggle-switch-label left font-size--1">Enable Two-Factor Authentication</span>
  <input type="checkbox" class="toggle-switch-input" checked>
  <span class="toggle-switch-track right"></span>
</label>





<h6 class="avenir-bold leader-2 font-size--3 light-gray">SECTION 2</h6>


   Upload profile photo
    <div class="message is-active">
 <div class="message-icon">
  {% icon 'information', style='filled' %}
</div>
  <div class="message-content">
 This will be used throughout ArcGIS online as your avatar
  </div>
  <button class="message-close" aria-label="Close">
    {% icon 'x' %}
    </button>
    </div>
 
  <input type="file">
  <div class="input-error-message is-success is-active">
 <div class="message-icon">
  {% icon 'check-circle', style='filled' %}
</div>
  <div class="message-content">
Successfully uploaded
</div>
  </div>

&nbsp;
  <fieldset class="fieldset-checkbox">
    <legend>Email Preferences (optional)</legend>
    <label>
      <input type="checkbox"> Weekly Newsletter
    </label>
    <label>
      <input type="checkbox"> Monthly Newsletter
    </label>
    <label>
      <input type="checkbox"> All Emails
    </label>
  </fieldset>
  <fieldset class="fieldset-radio">
    <legend>How did you hear about us? (optional)</legend>
    <label>
      <input type="radio" name="source" value="friend">Friend
    </label>
    <label>
      <input type="radio" name="source" value="event">Sponsored Event
    </label>
    <label>
      <input type="radio" name="source" value="other">Other
    </label>
  </fieldset>
  <label>

<h6 class="avenir-bold leader-2 font-size--3 light-gray">DANGER ZONE</h6>
   <div class="message message-red is-active">
 <div class="message-icon">
  {% icon 'information', style='filled' %}
</div>
  <div class="message-content">
 These settings are potentially dangerous. Proceed with caution!
  </div>
    </div>
<label class="toggle-switch toggle-switch-destructive clearfix">
  <span class="toggle-switch-label left font-size--1">Disable Two-Factor Authentication</span>
  <input type="checkbox" class="toggle-switch-input" checked >
  <span class="toggle-switch-track right"></span>

 
</label>








<h6 class="avenir-bold leader-2 font-size--3 light-gray">FORM EXAMPLES</h6>
   <div class="message message-red is-active">
 <div class="message-icon">
  {% icon 'information', style='filled' %}
</div>
  <div class="message-content">
 Please correct the errors below to proceed.
  </div>
    </div>
<label>
  First Name
  <input type="text" value="Tom" required>
</label>
<label>
  Address
  <input type="text" value="123 Main St." required>
</label>

<label>
  First Name
  <input type="text" class="input-success" value="Tom" required>
</label>

<label>
  Current Password
  <input type="text" required placeholder="Enter your current password" class="input-error">
  <div class="input-error-message is-active">
 <div class="message-icon">
  {% icon 'information', style='filled' %}
</div>
  <div class="message-content">
Your current password is incorrect
  </div>
  </div>
</label>
<label>
 Something Else
  <input type="text"value="Tom" required>
</label>

  <button type="submit" class="btn">Submit</button>
</form>
</div>
  </div>




  
</div>
&nbsp;