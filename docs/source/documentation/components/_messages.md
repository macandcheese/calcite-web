<div class="panel panel-gray leader-1 trailer-1">
<mark class='label label-blue'>Calcite Web 2.0 Update</mark>
<p class='leader-half trailer-0 font-size--1'>
The dom structure of messages has changed. To migrate your messages, follow the structure below for arranging your elements.
</p>
</div>

messages are used to inform users of state changes, errors, or successful actions. messages are only visible if they have the `is-active` class. Without as `is-active` class, the message will be set to `display: none;`

Calcite Web does not manage class assignment, invocation, or dismissal logic for messages - you will have to write your own JavaScript handlers for this.

An message can consist of up to three children - `message-icon`, `message-content`, and `message-close`. At a minimum, an message must contain an `message-content` child.  

#### message Icons
It's recommended to pair a status icon with your message. Pairing an message status with an icon helps reinforce the intent of the message, and ensures accessibility.

<div class="panel">
<label class="toggle-switch">
  <input type="checkbox" class="toggle-switch-input">
  <span class="toggle-switch-track margin-right-1"></span>
  <span class="toggle-switch-label font-size--1">Inline example</span>
</label>
<label class="toggle-switch toggle-switch-destructive clearfix">
  <span class="toggle-switch-label right font-size--1">Confirm account deletion. You cannot recover deleted accounts.</span>
  <input type="checkbox" class="toggle-switch-input">
  <span class="toggle-switch-track left"></span>
</label>
<label class="toggle-switch clearfix">
  <span class="toggle-switch-label left font-size--1">Enable Two-Factor Authentication</span>
  <input type="checkbox" class="toggle-switch-input" checked>
  <span class="toggle-switch-track right"></span>
</label>
    Upload profile photo

<div class="message is-active">
<div class="message-icon">
  {% icon 'information', style='filled' %}
</div>
<div class="message-content">
  This will be visible to other members to help quickly identify content ownership.
</div>
<button class="message-close" aria-label="Close">
  {% icon 'x' %}
</button>
</div>
&nbsp;
    <input type="file">
  </label>


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
  <button type="submit" class="btn">Submit</button>
</form>
</div>