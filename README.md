Navigation menus

Examples of accessible code for navigation menus for both mobile and desktop.

Semantic markup conveys the menu structure to users. Menus coded semantically can easily adapt to different situations, such as small screen displays, screen magnification, and other assistive technology.

Convey the menu structure, typically by using a list. Such structural information allows assistive technologies to announce the number of items in the menu and provide corresponding navigation functionality.

Use an ordered list <ol> when the sequence of the menu items is important.

Identify the menu, ideally using the HTML5 <nav> element to allow users access to the menu directly.

Label menus to make them easier to find and understand. Labels should be short but descriptive, to allow users to distinguish between multiple menus on a web page. Use a heading, aria-label, or aria-labelledby to provide the label.

Use markup to indicate the current item of a menu, such as the current page on a website, to improve orientation in the menu.

Provide an invisible label that is read aloud to screen reader users and used by other assistive technologies to mark the current item which allows custom label text. Remove the anchor <a>, so users cannot interact with the current item. That avoids misunderstandings and emphasizes that the current menu item is active. In the following example, the menu item has the invisible text “Current Page:” and the element is replaced by a with a class current: (To clarify <span> is not a semantic HTML element but can be used when no alternative HTML exists. ARIA attributes can be used to make unsemantic HTML more accessible to screen reader users). <li> <span class="current"> <span class="visuallyhidden">Current Page: </span> Space Bears </span> </li>

Use the aria-current="page" attribute to indicate the current page in the menu. This technique is particularly useful when the anchor <a> cannot be removed from the HTML.

Information above borrowed from [W3C] (https://www.w3.org/WAI/tutorials/menus/structure/)
