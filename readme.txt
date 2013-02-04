=== Subpage as Expandible Text Shortcode ===
Contributors: HBJitney LLC
Tags: navigation, pages, jquery, effect, text, embedded content
Requires at least: 3.4.1
Tested up to: 3.5.1
Stable tag: trunk
License: GPLv3

Add [subpages_expand] to any parent page. All child pages' titles are shown as links that expand to content when clicked

== Description ==

Intended users: editors, authors, contributors

This plugin will allow you to display the content of subpages as expandable links.

Simply add [subpages_expand] to any parent page. The titles of each of the subpages will be displayed there as clickable links. When the user clicks the link, it will expand, displaying the content of that child page.

Clicking the title again will collapse the content.

== Installation ==
If you have a single file (ending in ".zip"), then use the *Upload* method. If you have multiple files, use the *Files* method. If you're installing from WordPress directly, just hit the big 'Install Plugin' button.
= Upload =
1. From the plugins, add new screen, choose upload
1. Navigate to where the .zip file is located and select it
1. Make sure to *activate* the plugin once it is installed

= Files =
1. Upload the entire directory (not just the files) to the `/wp-content/plugins/` directory
1. Activate the plugin through the 'Plugins' menu in WordPress

== Frequently Asked Questions ==

= Q. Does this work on posts? =

**A.** No, only on pages

= Q. I added the shortcode and nothing happened! =

**A1.** Make sure you spelled it correctly

**A2.** Make sure you added the shortcode to a **page**, not a **post**.

**A3.** Make sure your page has sub-pages.

**A4.** Verify that your parent page and all child pages are published (not draft or pending)

= Q. My page has more than one subpage, but only one is showing up! When I click the link the other subpages are in the text that appears. =

**A.** You have an HTML error in one of your pages. If you have mismatched `div` tags, the child pages after that can get "trapped" in the first child's content.

= Q. Error 324 (net::ERR_EMPTY_RESPONSE) =

**A.** This error usually occurs when you try to have this shortcode on a child page.
You cannot nest this shortcode (i.e., have it on a parent page and one of the child pages).

= Q. It takes a long time for the page to display. =

**A.** The time it takes for the page to display is the time it takes for **all** of the subpages' content to
load. If you have subpages with lots of content (or javascript that loads in content), it will take time for
WordPress to load that page.

== Screenshots ==
1. Shortcode in parent post

2. Public view showing each subpage's title with one expanded

== Changelog ==

1.09a Not all child page links were displaying. Added additional FAQs that came up.

1.09 Fixed "Undefined variable: content" bug; cleaned up code

1.07 Fixed bug where shortcodes in the child pages weren't rendering

1.05a Corrected spelling/grammar errors in documentation (no functionality change)

1.05 Fixed issue with missing subpages

1.03 Expanded readme with information about an issue; added screenshots to zip

1.01 Released with a debug fix, some formatting for the titles and code cleanup

0.90 CSS change to title cursor

0.70 Initial

== Upgrade Notice ==

= 1.09a =
Bugfix: not all of the child pages were displaying
