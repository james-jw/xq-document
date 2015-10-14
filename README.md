# xq-document
Module for generating html from xqdoc <code>http://www.xqdoc.org/1.0</code> documentations.

<h3>Methods</h3>
<pre>
xqdoc-to-html($xqdoc as element(xqdoc:xqdoc))) as element(div)
</pre>

<h3>Dependencies</h3>
<pre>
git@github.com:james-jw/xq-bootstrap.git
</pre>

<h6>Installing Dependencies</h6>
Clone this repo as well as any dependencies into the same directory

<h3>Examples</h3>
Using BaseX's inspection module, you can quickly create html documentation. For example: <br />

<pre>
import module namespace inspect = "http://basex.org/modules/inspect";
import module namespace document = 'xq-document';
let $xqdoc := inspect:xqdoc('c:\path-to-xquery-module.xqm')
return document:xqdoc-to-html($xqdoc) 
</pre>

Happy Documenting!
