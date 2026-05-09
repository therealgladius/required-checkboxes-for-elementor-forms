=== Required Checkboxes for Elementor Forms ===
Contributors: therealgladius
Donate link: https://www.gladiusagency.com/
Tags: forms, validation, checkbox, required
Requires at least: 5.4
Tested up to: 6.9
Requires PHP: 7.4
Stable tag: 1.0.0
License: GPLv2 or later
License URI: https://www.gnu.org/licenses/gpl-2.0.html

Adds a "Required (at least one)" toggle to checkbox fields in the Elementor Pro Form widget.

== Description ==

The Elementor Pro Form widget does not include a built-in option to require at least one checkbox to be selected in a checkbox field. This plugin adds a simple toggle directly to the form builder UI to fill that gap.

= Features =

* Adds a **Required (at least one)** toggle to the Content tab of every checkbox field in the Form widget
* Server-side validation blocks submissions when no option is selected
* Client-side validation provides instant inline feedback under the field, before the AJAX request fires
* No edits to other plugins required
* No settings page — configuration is per-field in the form builder

= How to use =

1. Edit a form in the Elementor editor
2. Click a checkbox field
3. In the Content tab, toggle **Required (at least one)** on
4. Save and publish

That's it. The form will block submissions where the user hasn't selected at least one option, and the error message will appear right below the field.

= Requirements =

* WordPress 5.4 or later
* PHP 7.4 or later
* Elementor Pro (the free Elementor plugin does not include the Form widget)

== Installation ==

1. Upload the plugin folder to the `/wp-content/plugins/` directory, or install through the WordPress Plugins screen
2. Activate the plugin through the Plugins screen in WordPress
3. Edit a form in the Elementor editor and configure your checkbox fields

== Frequently Asked Questions ==

= Does this work with the free Elementor plugin? =

No. The Form widget is a Pro-only widget. This plugin extends that widget, so Elementor Pro is required.

= Does this affect any other field types? =

No. The toggle only appears on checkbox fields, and the validation only runs on checkbox fields.

= Will it conflict with my existing required checkbox settings? =

No. The plugin checks both its own toggle and the standard `required` flag, so existing setups continue to work.

= Where does the error message appear? =

Directly underneath the checkbox field, before the form is submitted. If JavaScript is disabled, server-side validation still catches the empty submission and displays the error after the AJAX round-trip.

== Screenshots ==

1. The Required (at least one) toggle in the Form builder's Content tab
2. The inline error message displayed when a user attempts to submit with no option selected

== Changelog ==

= 1.0.0 =
* Initial release.

== Upgrade Notice ==

= 1.0.0 =
Initial release.
