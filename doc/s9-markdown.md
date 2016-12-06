# Markdown Example

* You can write slides in markdown, if you prefer

# Code Example

<pre>
<code data-trim contenteditable class="javascript">
function linkify( selector ) {
  if( supports3DTransforms ) {

    var nodes = document.querySelectorAll( selector );

    for( var i = 0, len = nodes.length; i &lt; len; i++ ) {
      var node = nodes[i];

      if( !node.className ) ) {
        node.className += ' roll';
      }
    };
  }
}
</code>
</pre>

# Another Code Example

<% coderay :lang => 'ruby', :line_numbers => :inline do %> 
  puts 'Hallo Welt!   
<% end %> 
