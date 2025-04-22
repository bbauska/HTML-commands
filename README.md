# HTML-commands
HTML - HyperText Markup Language commands.

<?xml version="1.0" encoding="iso-8859-1"?>
<!DOCTYPE HTML PUBLIC "-//W3C//DTD HTML 4.01 Transitional//EN"> 

<html>
<head>

<!--

TO DO: define thead & tbody for the tables below

TO ADD:

from
   http://www.w3.org/TR/html4/struct/text.html#h-9.4

   9.4 Marking document changes: The INS and DEL elements

<P>
  A Sheriff can employ <DEL>3</DEL><INS>5</INS> deputies.
</P>

-->


<title>HTML: Commands</title>
</head>

<body>

<h2>Remarks:</h2> <ul> <li> An attribute value must be quoted if it
contains any character other than letters (A-Za-z), digits, hyphens, and
periods; use quotes if in doubt.

<br>

Here is an example:

<blockquote>
<code>
&lt;a href=&quot;http://www.math.uh.edu&quot;
name=&quot;start&quot;&gt;Dept. of Math.&lt;/a&gt; </code> </blockquote>

<li>
NONE in the &quot;value&quot; field below means that one can use the
attribute without a value.

</ul>

<br>

<h2>HTML commands:</h2>


<dl>

<dt><code>
<b>&lt;a&gt;</b>, <b>&lt;/a&gt;</b>
</code>
  <dd>	<ul>
	  <li> purpose: anchor, for links and labels
	  <li> example: <code>
	  &lt;a href=&quot;http://www.math.uh.edu&quot;
	    name=&quot;start&quot;&gt;Dept. of Math.&lt;/a&gt;
	 </code>
	  <li> attributes:
		<table border="1"  cellpadding="1">
	    <tr><th> Attribute <th> Values <th> Meaning <th> Remarks
	    <tr><td align="center"> <code> href </code><td> URL <td> address of link <td>  &nbsp;
	    <tr><td align="center"> <code> name </code><td> text  <td>
	    	    label of this position in the file <td> &nbsp;
	    <tr><td align="center" valign="top" rowspan="5"> <code>target</code>
	      <td valign="top" align="left"> name_of_frame 
	      <td valign="top"> frame in which the link should be rendered
	      <td align="left" valign="top" rowspan="5">

			<ul>
			
			<li> These items <b>might be case-sensitive</b>!

			<li> If the named frame does not exist, the link is
			rendered in a new window (unless overridden by the
			user).

			<li> <code>_self </code> is useful for overriding a
			BASE TARGET

			</ul>

	    <tr> <td align="left"> <code>_blank </code>
		<td> renders the link in a new, unnamed window

	    <tr> <td align="left"> <code>_parent</code>
		<td> renders the link in the immediate FRAMESET parent

	    <tr> <td align="left"> <code>_top</code>
		<td> renders the link in the full, unframed window

	    <tr> <td align="left"> <code>_self</code>
		<td> renders the link in the current frame
		  
	      </table>
	</ul>


<!--
          _blank renders the link in a new, unnamed window 
          _self renders the link in the current frame (useful for overriding a BASE TARGET) 
          _parent renders the link in the immediate FRAMESET parent 
          _top renders the link in the full, unframed window 


	    <tr><td> target <td> name of frame <td> frame in which the link
  should be rendered <td> e.g., used with FRAMESET
	    <tr><td> target <td> _blank <td> renders the link in a new,
	    unnamed window  <td> these four values are <strong>case-sensitive</strong>!
	    <tr><td> target <td> _parent <td> renders the link in the
  immediate FRAMESET parent <td> &nbsp; 
	    <tr><td> target <td> _top <td> renders the link in the full,
  unframed window <td> &nbsp;
	    <tr><td> target <td> _self <td> renders the link in the current
  frame <td> useful for overriding a BASE TARGET


	    <tr><td  align="center" valign="top"> <code>target</code>
	      <td valign="top"> <ol>
	      	    <li>name of frame
		    <li><code>_blank </code>
		    <li><code>_parent</code>
		    <li><code>_top</code>
		    <li><code>_self</code>
		  </ol>
	    <td valign="top">  <ol>
	      	    <li>frame in which the link should be rendered
	      	    <li>renders the link in a new, unnamed window
	      	    <li>renders the link in the immediate FRAMESET parent
	      	    <li>renders the link in the full, unframed window
	      	    <li>renders the link in the current frame
		  </ol>
	    <td valign="top">  <li>These items <b>might be case-sensitive</b>!
		<li> If the named frame does not exist, the link is rendered
		in a new window (unless overridden by the user).
		<li> <code> _self 
		</code>
		useful for overriding a BASE TARGET
	
-->	


<br><dt><code>
<b>&lt;img&gt;</b>
</code>
  <dd>	<ul>
	  <li>purpose: inline image
	  <li> example: <code>
	  &lt;img src=&quot;../picture.jpg&quot;
	    height=&quot;20%&quot; alt=&quot;campus map&quot;&gt;
	 </code>
	  <li> attributes:
		<table border="1">
	         <tr><th> Attribute <th> Values <th> Meaning <th> Remarks
		 <tr><td align="center"> <code> src </code><td> URL <td> source file <td> &nbsp;
		 <tr><td align="center"> <code> height </code><td> number, percentage <td> pixel size, %
  of page height<td> &nbsp;
		 <tr><td align="center"> <code> width </code><td> number, percentage <td> pixel size, %
  of page width <td> &nbsp; 
		 <tr><td align="center"> <code> alt </code><td> text <td> show if no image <td> &nbsp;
		 <tr><td align="center"> <code> align </code><td>
		 <code>top</code>, <code>middle</code>,
		 <code>bottom</code>, <code>left</code>, <code>right</code>
		 <td>
  &nbsp;<td> deprecated, use <code>&lt;br clear&gt;</code> instead
		 <tr><td align="center"> <code> border </code><td> number  <td> size in pixels <td>
  border=&quot;0&quot; means no border
	       </table>
	</ul>


<br><dt><code>
<b>&lt;br&nbsp/&gt;</b>
</code>
  <dd>	<ul>
	  <li>purpose: line break
	  <li> attributes:
		<table border="1">
		 <tr><th> Attribute <th> Values <th> Meaning <th> Remarks
		 <tr><td align="center"> <code> clear </code><td> <code>
		 left</code>, <code>all</code>, <code>right</code>, NONE
		 <td> clear floating objects <td> &nbsp;
	      </table>
	</ul>


<br><dt><code>
<b>&lt;p&gt;</b>, <b>&lt;p/&gt;</b>
</code>
  <dd>	<ul>
	  <li>purpose: new paragraph
	  <li>attributes:
		<table border="1">
		 <tr><th> Attribute <th> Values <th> Meaning <th> Remarks
		 <tr><td align="center"> <code> align </code><td>
		 <code>left</code>, <code>center</code>,
		 <code>right</code>, <code>justify</code>
		  <td> &nbsp; <td> deprecated; horizontal alignment
	      </table>
	</ul>

<br><dt><code>
<b>&lt;hr /&gt;</b>
</code>
  <dd>	<ul>
	  <li>purpose: horizontal rule
	  <li> example: <code>
	  &lt;hr noshade size=&quot;2&quot; width=&quot;50%&quot;
  align=&quot;center&quot;&nbsp;/&gt; </code>
	  <li> attributes:
		<table border="1">
		 <tr><th> Attribute <th> Values <th> Meaning <th> Remarks
		 <tr><td align="center"> <code> noshade </code><td> &nbsp; <td> solid line <td>&nbsp;
		 <tr><td align="center"> <code> size </code><td> number <td> height in pixels <td>&nbsp;
		 <tr><td align="center"> <code> align </code><td>
		 <code>center</code>, <code>left</code>, <code>right</code>
		 <td> &nbsp;<td> &nbsp;
		 <tr><td align="center"> <code> width </code><td> number, percentage <td> pixels, % of page-width<td> &nbsp;
	      </table>
	</ul>


<br><dt> <b>fonts & co.</b>
  <dd>	<ul>
	  <li>purpose: use a particular font, select size, heading etc.
	  <li> tags:
		<table border="1">
		 <tr><th> Tag and endtag <th> Effect, Meaning  <th> Remarks
  		 <tr><td align="center"> <code> &lt;font&gt;, &lt;/font&gt;
		   		 </code><td> &nbsp;<td> see <a
				 href="#fonts">below</a>

  		 <tr><td align="center"> <code> &lt;pre&gt;, &lt;/pre&gt;
		   		 </code><td> <pre> preformated 
        text </pre>
				 <td valign="top">
				       creates a separate paragraph
				       <br>
				       spaces and line-breaks matter
		 <tr><td align="center"> <code> &lt;h1&gt;, &lt;/h1&gt;
		   		 </code><td> <h1>level-one heading</h1> <td
				 valign="top" rowspan=2>
				 headings create a separate paragraph
				 <br>
				  levels go from 1 (largest) to 6 (smallest)
		 <tr><td align="center"> <code> &lt;h6&gt;, &lt;/h6&gt;
		   		 </code><td> <h6>level-six heading</h6> 
		 <tr><td align="center"> <code> &lt;i&gt;, &lt;/i&gt;
		   		 </code><td> <i>italic</i> text <td>&nbsp; 
		 <tr><td align="center"> <code> &lt;b&gt;, &lt;/b&gt;
		   		 </code><td> <b>bold</b> text <td>&nbsp; 
		 <tr><td align="center"> <code> &lt;tt&gt;, &lt;/tt&gt;
		   		 </code><td> <tt>teletype</tt> text <td>&nbsp; 
		 <tr><td align="center"> <code> &lt;em&gt;, &lt;/em&gt;
		   		 </code><td> <em>emphasis</em> <td>&nbsp;
		 <tr><td align="center"> <code> &lt;strong&gt;, &lt;/strong&gt; </code><td>
		 		 <strong>strong emphasis</strong><td>&nbsp;
		 <tr><td align="center"> <code> &lt;cite&gt;, &lt;/cite&gt; </code><td>
		 		 <cite>citation</cite><td>&nbsp; 
		 <tr><td align="center"> <code> &lt;big&gt;, &lt;/big&gt;
		   		 </code><td> <big>big</big> text <td>&nbsp;
		 <tr><td align="center"> <code> &lt;small&gt;,
		   		 &lt;/small&gt; </code><td> <small>small</small> text
				 <td>&nbsp;
		 <tr><td align="center"> <code> &lt;sub&gt;, &lt;/sub&gt;
		   		 </code><td> <sub>subscript</sub> <td>&nbsp;
		 <tr><td align="center"> <code> &lt;sup&gt;, &lt;/sup&gt;
		   		 </code><td> <sup>superscript</sup> <td>&nbsp;
		 <tr><td align="center"> <code> &lt;u&gt;, &lt;/u&gt;
		   		 </code><td> <u>underline</u> <td>
				 deprecated; use <code> cite </code> or <code> strong
				 </code>
		 <tr><td align="center"> <code> &lt;s&gt;, &lt;/s&gt; </code><td> 
		 		 <s>strike-through</s> text <td> deprecated 
		 <tr><td align="center"> <code> &lt;strike&gt;, &lt;/strike&gt; </code><td>
		 		 <s>strike-through</s> text <td> better
		 		 supported than  &lt;s&gt;; deprecated 
		 <tr><td align="center"> <code> &lt;code&gt;, &lt;/code&gt; </code><td> <code>
		 		 computer code </code> <td> use it to
		 		 stress the <em>meaning</em> of the text
		 <tr><td align="center"> <code> &lt;del&gt;, &lt;/del&gt; </code><td>
		 		 <del>deleted</del> text <td> not
		 		 implemented yet; preferred to
		 		 &lt;strike&gt;
<!--  		 <tr><td align="center"> <code> &lt;&gt;, &lt;/  &gt; </code><td>  <td> &nbsp; -->
<!--  		 <tr><td align="center"> <code> &lt; &gt;, &lt;/  &gt; </code><td> <td> &nbsp; -->
	      </table>
	</ul>

<p>

<dt><code> <a name="fonts"><b>&lt;font&gt;</b></a>, <b>&lt;/font&gt;</b>
</code>
  <dd>	<ul>
	  <li> purpose: change font size, color, type etc.
	  <li> example: <code>
	  &lt;font size=&quot;+1&quot;
	  color=&quot;red&quot;&gt<font  size="+1"color="red">larger red words</font>&lt;/font&gt;
	 </code>

	 <li> remark: a better way to achive this is using <a
	  href="http://www.htmlhelp.com/reference/css/" target="TEMP">style sheets</a>

	  <li> attributes:
		<table border="1">
	    <tr><th> Attribute <th> Values <th> Meaning <th> Remarks

	    <tr><td align="center" rowspan="2"> <code> size </code><td >
	    <code> 1, ..., 7 </code> <td> specifies size to be used <td>
	    default starting size is 3

	    <tr><td align="center"> <code>-3, ..., +3 </code><td>
	        changes size from that previously in use <td>  &nbsp;

	    <tr><td align="center"> <code>color</code> <td> <code> <font
	    color="red">red</font>, <font color="#FF00FF">#FF00FF</font>
	    </code> <td> value or word to describe color <td>

	     Color attribute values give a color definition. The value can
	     be any hexadecimal number, specified according to the sRGB
	     color space, or one of sixteen color names. Hexadecimal
	     numbers must be prefixed by a &quot;#&quot; character. <a
	     href="colors.html" target="TEMP">Here</a> is a list of
	     colors.

	     <tr><td align="center"> <code>face</code> <td> &nbsp; <td>
	     specifies list of fonts to be used (in order of preference)
	     <td> the browser will use the first one available from the
	     list 

	      </table>
	</ul>





<br><dt> <a name="lists"><b>lists</b></a>
  <dd>
	<ul>

	  <li> there are three types of lists:
		<ul>
		  <li> ordered lists: &nbsp; <code>&lt;ol&gt;,
		  &lt;/ol&gt;</code>
		    
		    <br> the elements of the list are introduced by &nbsp;
		      <code>&lt;li&gt;</code> (list item)

		    <br> the end tag &nbsp; <code>&lt;/li&gt;</code>
		      is <b>not optional</b> 

		    <br> to change the current label to 30, use
		    <code>&lt;li value=&quot;30&quot;&gt;</code>
		    
		  <li> unordered lists: &nbsp; <code>&lt;ul&gt;,
		     &lt;/ul&gt;</code>

		    <br>
		     the elements of the list are introduced by &nbsp;
		     <code>&lt;li&gt;</code> (list item)

		    <br> the end tag &nbsp; <code>&lt;/li&gt;</code> is
		     <b>not optional</b>
				    
		    
		  <li> definition lists: &nbsp; <code>&lt;dl&gt;,
		  &lt;/dl&gt;</code>

		    <br>
		    the elements of the list are pairs
		    <em>term-definition</em> introduced by
		    <ul>
		    <li> <code>&lt;dt&gt;</code> (definition term)

		    <li> <code>&lt;dd&gt;</code> (definition definition)

		    </ul>

		    the end tags &nbsp; <code>&lt;/dt&gt;</code> and &nbsp;
		     <code>&lt;/dd&gt;</code> are <b>not optional</b>

		</ul>

	  <li> lists can be nested

	  <li> examples:

<br><br>

<table border="1"  cellpadding="5">
<tr> <th> Type of list <th width="50%"> How it looks <th> HTML code

<tr>
  <th valign="top" align="center"> Ordered List

  <td valign="top" align="left">

	<ol>
	  <li> first item
	  <li> second item
	  <li value="33"> third item, but we want it to have label 33
	  <li> next item; note the label
	</ol>

  <td valign="top" align="left">
  <pre>
 &lt;ol&gt;
   &lt;li&gt; first item &lt;/li&gt;
   &lt;li&gt; second item &lt;/li&gt;
   &lt;li value=&quot;33&quot;&gt; third item, but we want it to have label
   33 &lt;/li&gt;
   &lt;li&gt; next item; note the label &lt;/li&gt;
 &lt;/ol&gt; </pre>

<tr>
  <th valign="top" align="center"> Unordered List

  <td valign="top" align="left">

	<ul>
	  <li> first item 
	  <li> second item
	</ul>

  <td valign="top" align="left">
  <pre>
 &lt;ul&gt;
   &lt;li&gt; first item &lt;/li&gt;
   &lt;li&gt; second item &lt;/li&gt;
 &lt;/ul&gt; </pre>

<tr>
  <th valign="top" align="left"> Definition List

  <td valign="top" align="left">

	<dl>
	  <dt> Texas
	     <dd> state of US
	  <dt> Houston
	     <dd> city in Texas
	</dl>

  <td valign="top" align="left">
  <pre>
 &lt;dl&gt;
   &lt;dt&gt; Texas &lt;/dt&gt;
     &lt;dd&gt; state of US &lt;/dd&gt;
   &lt;dt&gt; Houston &lt;/dt&gt;
     &lt;dd&gt; city in Texas &lt;/dd&gt;
 &lt;/dl&gt; </pre>

<tr>
  <td valign="top" align="center"> Nested lists

  <td valign="top" align="left">

<ul>
<li> cities:
 <ol>
 <li> Athens
 <li> Sparta
 </ol>
<li> continents:
<ul>
 <li> Africa
 <li> America
 <li> Asia
 <li> Europa
</ul>
</ul>

  <td valign="top" align="left">
<pre>
&lt;ul&gt;
  &lt;li&gt; cities:
     &lt;ol&gt;
       &lt;li&gt; Athens &lt;/li&gt;
       &lt;li&gt; Sparta &lt;/li&gt;
     &lt;/ol&gt;
  &lt;/li&gt;
  &lt;li&gt; continents:
     &lt;ul&gt;
       &lt;li&gt; Africa &lt;/li&gt;
       &lt;li&gt; America &lt;/li&gt;
       &lt;li&gt; Asia &lt;/li&gt;
       &lt;li&gt; Europa &lt;/li&gt;
    &lt;/ul&gt;
&lt;/ul&gt; </pre>
</table>

<br>



</ul>


<br><dt> <a name="tables"><b>tables</b></a> <dd>
	<ul>
	<li>simplified example (from <A target="TEMP"
  		HREF="http://www.htmlhelp.com/reference/html40/tables/table.html">
  		HTML 4.0 Reference</A>):



<br><br>


<TABLE border="1">
	<thead>
              <TR>
                <TH ROWSPAN=2>Character</TH>
                <TH ROWSPAN=2>Entity</TH>
                <TH ROWSPAN=2>Decimal</TH>
                <TH ROWSPAN=2>Hex</TH>
                <TH COLSPAN=3>Rendering in Your Browser</TH>
              </TR>
	      <TR>
                <TH>Entity</TH>
                <TH>Decimal</TH>
                <TH>Hex</TH>
              </TR>
	</thead>
	<tbody>
              <TR>
                <TD>non-breaking space</TD>
                <TD>&amp;nbsp;</TD>
                <TD>&amp;#160;</TD>
                <TD>&amp;#xA0;</TD>
                <TD>&nbsp;</TD>
                <TD>&#160;</TD>
                <TD>&#xA0;</TD>
              </TR>
	      <TR>
	         <TD>quotation mark = APL quote</TD>
		 <TD>&amp;quot;</TD>
		 <TD>&amp;#34;</TD>
		 <TD>&amp;#x22;</TD>
		 <TD>&quot;</TD>
		 <TD>&#34;</TD>
		 <TD>&#x22;</TD>
	      </TR>
	      <TR>
	         <TD>ampersand</TD>
		 <TD>&amp;amp;</TD>
		 <TD>&amp;#38;</TD>
		 <TD>&amp;#x26;</TD>
		 <TD>&amp;</TD>
		 <TD>&#38;</TD>
		 <TD>&#x26;</TD>
	      </TR>
	      <TR>
		 <TD>less-than sign</TD>
		 <TD>&amp;lt;</TD>
		 <TD>&amp;#60;</TD>
		 <TD>&amp;#x3C;</TD>
		 <TD>&lt;</TD>
		 <TD>&#60;</TD>
		 <TD>&#x3C;</TD>
	      </TR>
	      <TR>
		 <TD>greater-than sign</TD>
		 <TD>&amp;gt;</TD>
		 <TD>&amp;#62;</TD>
		 <TD>&amp;#x3E;</TD>
		 <TD>&gt;</TD>
		 <TD>&#62;</TD>
		 <TD>&#x3E;</TD>
	      </TR>
	</tbody>
</TABLE>

<br>

	<li> the HTML code that produced it:

<pre>
&lt;TABLE border=&quot;1&quot;&gt;
    &lt;THEAD&gt;
     &lt;TR&gt;
       &lt;TH ROWSPAN=2&gt;Character&lt;/TH&gt;
       &lt;TH ROWSPAN=2&gt;Entity&lt;/TH&gt;
       &lt;TH ROWSPAN=2&gt;Decimal&lt;/TH&gt;
       &lt;TH ROWSPAN=2&gt;Hex&lt;/TH&gt;
       &lt;TH COLSPAN=3&gt;Rendering in Your Browser&lt;/TH&gt;
     &lt;/TR&gt;
     &lt;TR&gt;
       &lt;TH&gt;Entity&lt;/TH&gt;
       &lt;TH&gt;Decimal&lt;/TH&gt;
       &lt;TH&gt;Hex&lt;/TH&gt;
     &lt;/TR&gt;
    &lt;/THEAD&gt;
    &lt;TBODY&gt;

     &lt;TR&gt;
       &lt;TD&gt;non-breaking space&lt;/TD&gt;
       &lt;TD&gt;&amp;amp;nbsp;&lt;/TD&gt;
       &lt;TD&gt;&amp;amp;#160;&lt;/TD&gt;
       &lt;TD&gt;&amp;amp;#xA0;&lt;/TD&gt;
       &lt;TD&gt;&amp;nbsp;&lt;/TD&gt;
       &lt;TD&gt;&amp;#160;&lt;/TD&gt;
       &lt;TD&gt;&amp;#xA0;&lt;/TD&gt;
     &lt;/TR&gt;

  etc.

    &lt;/TBODY&gt;
 &lt;/TABLE&gt;

</pre>

	<li> ingredients:

	  <ul>

	     <li> <code>&lt;table&gt;, &lt;/table&gt;</code>: encloses the
	     table

	     <li> <code>&lt;thead&gt;, &lt;/thead&gt;</code>: encloses the
	     table head; this helps the browser display the head on each
	     page, if the table is longer.

	     <li> <code>&lt;tfoot&gt;, &lt;/tfoot&gt;</code>: encloses the
	     footer of the table; it must precede the <code>&lt;tbody&gt;</code>

	     <li> <code>&lt;tbody&gt;, &lt;/tbody&gt;</code>: encloses the
	     body of the table

	     <li> <code>&lt;tr&gt;, &lt;/tr&gt;</code>: table row

	     <li> <code>&lt;th&gt;, &lt;/th&gt;</code>: table header cell;
	     used within <code>&lt;tr&gt</code>

	     <li> <code>&lt;td&gt;, &lt;/td&gt;</code>: table data cell;
	     used within <code>&lt;tr&gt</code>

	  </ul>

	<li> arguments of <code>&lt;th&gt;</code>&nbsp; and &nbsp; 
	<code>&lt;td&gt;</code>:

		<table border="1">
	         <tr><th> Attribute <th> Values <th> Meaning <th> Remarks
		 <tr><td  align="center"> <code> colspan </code><td> number
		 		 <td> columns spanned by the cell<td> &nbsp;
		 <tr><td align="center"> <code> rowspan </code><td> number
		 		 <td> rows spanned by the cell <td> &nbsp;
		 <tr><td align="center"> <code> align </code><td> <code> center
		 		 </code>, <code> left </code>, <code> right
				 </code>, <code> justify </code> <td>
				  horizontal alignment <td> &nbsp; 
		 <tr><td align="center"> <code> valign </code><td> <code> top
		 		 </code>, <code> bottom </code>, <code> middle
				 </code> <td> vertical alignment <td> &nbsp;
		 <tr><td align="center"> <code> nowrap </code><td> &nbsp;
		 		 <td> suppress word wrap <td> &nbsp;
	       </table>


	<li> the example with more <a href="tables.html"
	target=_self>features</a>.

	</ul>



</dl>

<b>To be added:</b>
<ul>
<li> more about table arguments
<li> <code> &lt;center&gt;</code>
<li> <code> &lt;basefont&gt; </code>
<li> <code> &lt;blockquote&gt;</code>, <code> &lt;q&gt;</code>
<li> <code> &lt;base&gt; </code>
<li> <code> &lt;address&gt;</code>
<li> forms
<li> frames
</ul>
</body>
</html>

<!-- 

<P><IMG SRC="toronto.jpg" ALIGN=left ALT="" TITLE="Toronto's CN
          Tower">Toronto is the largest city in Canada and the fourth largest in North
          America.</P>
          <BR CLEAR=left>
          <P>The city is highly multicultural, with over 80 ethnic communities from
          Africa, Asia, and Europe...

          <MAP NAME=mymap>
          <AREA HREF="/reference/" ALT="HTML and CSS Reference" COORDS="5,5,95,195">
          <AREA HREF="/design/" ALT="Design Guide" COORDS="105,5,195,195">
          <AREA HREF="/tools/" ALT="Tools" COORDS="205,5,295,195">
          </MAP>
          <IMG SRC="sitemap.gif" ALT="Site map" USEMAP="#mymap" WIDTH=300
  HEIGHT=200>


<br><dt><code>
<b>&lt; &gt;, &lt;/  &gt;</b>
</code>
  <dd>	<ul>
	  <li>purpose: 
	  <li>attributes:
		<table border="1">
		 <tr><th> Attribute <th> Values <th> Meaning <th> Remarks
		 <tr><td align="center"> <code> </code><td>  <td> <td> 
		 <tr><td align="center"> <code> </code><td>  <td> <td> 
		 <tr><td align="center"> <code> </code><td>  <td> <td> 
		 <tr><td align="center"> <code> </code><td>  <td> <td> 
	      </table>
	</ul>

-->

