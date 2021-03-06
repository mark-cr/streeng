ExpressionEngine String Operations
====

Perform common operations on strings in ExpressionEngine. All parameters are optional.

Parameters:

	allowed="p|span|a" - pass "none" to strip all tags or a | delimited list of allowed tags (defaults = allow al)
	find="string1" - string to find (default = false)
	replace="string2" - string to replace found string (default = "")
	trim="left" - left, right, or both (default = "both")
	encode="yes" - HTML encode the string (default = "no")
	decode="yes" - HTML decode the string (default = "no")
	capitalize="yes" - capitalize the first character of the string (default = "no")
	title="yes" - capitalize the first character of every word (default = "no")
	lower="yes" - convert the string to lower case (default = "no")
	upper="yes" - convert the string to upper case (default = "no")
	characters="10" - number of characters to truncate the string to (default = unlimited)
	words="10" - number of words to truncate the string to (default = unlimited)
	append="..." - if truncated append this to the end of the string (default = "&hellip;")
	slug="yes" - convert the string to a slug (default = "no")
	separator="_" - separator for slug (default = "-")
	repeat="3" - number of times to repeat the string, great for prototyping (default = 0)

Usage:

	{exp:streeng allowed="p" title="yes" repeat="2" find=" a " replace=" my "}  <p><b>This</b> is a <a href="#">test</a>.</p>{/exp:streeng}

	<p>This Is My Test.</p>
	<p>This Is My Test.</p>
	<p>This Is My Test.</p>