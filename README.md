DOC: https://www.cssscript.com/demo/advanced-animated-dropdown-menu/#installation


Getting Started
Installation
Usage
Utilities
Animations
Usage of Animations & Types

dropdowneasy
Documentation
ads via Carbon
Your new development career awaits. Check out the latest listings.
ADS VIA CARBON
Dropdown Easy: Advanced Animated Dropdown Menu Examples
Installation
Including "dropdown.js" file at your html file is enough to use Dropdown Easy at your project.
<script src="dropdown.js"></script>
Usage
You must have a container element to open dropdown menu when container triggered. The container element must have "dropdown" as class, and the dropdown menu itself must have "dropdown-menu" as class. Then you can fill and stylize "dropdown-menu" as you want. Here's the structure:
<element class="dropdown">
    <element class="dropdown-menu">
        ...
    </element>
</element>
Note: Container element must be at the fore to dedect the clicking, otherwise menu doesn't opens.

Then you can utilitize and stylize the dropdown menu as you want. Like the example below:
<div class="dropdown fade@0.1s-ease-in secondary-click">
    <div class="dropdown-menu">
        <ul>
            <li>Copy</li>
            <li>Paste</li>
            <li>Cut</li>
            <li>Delete</li>
        </ul>
    </div>
</div>
Utilities
You can add utilities easily by adding them as classes. For example, you can add "dont-dismiss-at-tap" class to the container element to prevent dropdown menu from dismissing when you tap on it.
dont-dismiss-at-tap
The function of the "dont-dismiss-at-tap" class is to prevent dropdown menu from dismissing when you click/tap to the areas inside "dropdown-menu".
Includes "dont-dismiss-at-tap".
Copy
Paste
Cut
Delete
Doesn't include "dont-dismiss-at-tap".This menu will close anyways when you tap/click.
dismiss-button
The function of "dismiss-button" is giving an element a dismiss button function in "dropdown-menu", so it's only useful when "dont-dismiss-at-tap" class is enabled; also different than other utilities, the "dismiss-button" class must be added to an element in "dropdown-menu".
Includes a "dismiss-button" element.Close this "dont-dismiss-at-tap" by the button below.

Close
dismiss-while-scrolling
The function of the "dismiss-while-scrolling" class is to dismiss the dropdown menu when you scroll the page.
Includes "dismiss-while-scrolling".Scroll and it'll gone.
secondary-click
The "secondary-click" class lets you replace your dropdown menu with context menu in dropdown, so you must use secondary button of your mouse to open it.
Includes "secondary-click".Hellooo
fixed-pos
The "fixed-pos" class lets you fix the position of dropdown menu at the position it opened.
Includes "fixed-pos".Look it stays still when you scroll.
Animations
Usage of Animations & Types
You can add menus opening&closing animations. There is 6 types of animations and you can customize the transition duration and curve as you want. Syntax is almost same as CSS, you can use CSS timing-functions. Here's the syntax:
<element class="dropdown [animationType]@[duration]s-[timing-function]...">
    <element class="dropdown-menu">
        ...
    </element>
</element>
Known Issue: cubic-bezier isn't working right now, will be fixed at next releases.

Default duration value is 0.2s, default timing-function is "ease".
scaling
Transition between 0%-100% scale.
"scaling" transitionHellooo
scaling-bouncy
Transition between 0%-100% scale with bouncy effect.
"scaling-bouncy" transitionHellooo
Note: When durations get higher it gets less visible. Recommended with faster durations.
scaling-blur
Transition between 0%-100% scale and 30px-0px blur.
"scaling-blur" transitionHellooo
Recommended duration is 0.3s
scaling-fade
Transition between 0%-100% scale and 0%-100% opacity.
"scaling-fade" transitionHellooo
fade
Transition between 0%-100% opacity.
"fade" transitionHellooo
fade-blur
Transition between 0%-100% opacity and 30px-0px blur.
"fade-blur" transitionHellooo
Recommended duration is 0.3s
