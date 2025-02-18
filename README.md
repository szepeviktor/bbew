# BB Editing Workflow
A simple editorial workflow for Beaver Builder

<p align="center">
<img alt="A page ready to review" width="600" src="https://github.com/corypina/bbew/blob/master/img/03.ready-for-review.jpg" />
</p>

## Background
This all started when our team migrated a higher ed site over to WordPress. We wanted to allow large handfulls of authorized users to access the Beaver Builder interface to make simple edits when needed. We also wanted to control whether those edits were published, so we needed some kind of approval process. That's where this plugin comes in. We've been using this sucessfully for a few years now (as of June 2019).

## What this does
The gist:
- The admin decides which user role(s) get publishing permission
- Users without permission (but with access to the Builder) will only be able to **Save Draft**
- When those users are ready to submit changes, there's a simple form available to describe the chnanges made
- The admin receives that info via email, and can view the changes before making them live.
- The page is locked from editing until published by Admin

## Setup
1. Install/activate the plugin
2. Set both the admin email and the user roles with publishing permission in the main plugin file ([bbew.php](bbew.php))
3. You're done.


## Notes
- The notices printed to the screen are currently hooked into the *Top Bar* of the **Beaver Builder Theme**. If you're using a different theme, or just want to change this up, the notices are controlled in `includes/notices.bb-editing.php`.

<p align="center">
  <img alt="Describing the changes" width="600" src="https://github.com/corypina/bbew/blob/master/img/04.changes-summary.jpg" />
  <img alt="A page ready to review" width="600" src="https://github.com/corypina/bbew/blob/master/img/03.ready-for-review.jpg" />
  <img alt="Locked for editing" width="600" src="https://github.com/corypina/bbew/blob/master/img/06.locked.jpg" />
  <img alt="Locked for editing" width="600" src="https://github.com/corypina/bbew/blob/master/img/09.viewing-unpublished.jpg" />
</p>
