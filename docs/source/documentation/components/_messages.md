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

<div class="message message-red is-active">
<div class="message-icon">
  {% icon 'exclamation-mark-triangle', style='filled' %}
</div>
<div class="message-content">
  You don't have enough credits for that.
</div>
<button class="message-close" aria-label="Close">
  {% icon 'x' %}
</button>
</div>
&nbsp;

#### message Actions
Sometimes it can be useful to provide a follow-up action or contextual link to a user within an message. Place a `btn-link` element in a trailing position to your message copy.

<div class="message message-yellow is-active">
<div class="message-content">
  You don't have enough credits to perform that action.
  <a class="btn-link">Get more credits.</a>
</div>
<button class="message-close" aria-label="Close">
  {% icon 'x' %}
</button>
</div>
&nbsp;

<div class="message message-green is-active">
<div class="message-icon">
  {% icon 'check-circle', style='filled' %}
</div>
<div class="message-content">
   You successfully invited 4 members to the feature layer  <a class="btn-link">2019 Franchise Location Sales Map</a>
</div>
<button class="message-close" aria-label="Close">
  {% icon 'x' %}
</button>
</div>
&nbsp;

#### Auto-dismissal
It's recommended to use an explicit close button. If you decide to auto-dismiss messages, ensure the duration of the message's visibility is long enough for a user to read it. Don't place any follow-up actions in an auto-dismissable message.

<div class="message message-yellow is-active">
<div class="message-icon">
  {% icon 'exclamation-mark-triangle', style='filled' %}
</div>
<div class="message-content">
  You don't have enough credits for that.
</div>
</div>
&nbsp;