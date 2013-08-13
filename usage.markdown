---
layout:      default
title:       Usage
---
<script type="text/javascript">
  var languages = ['java', 'php', 'ruby'];

  function displayCode(codeBlock, codeLanguage) {
    $.each(languages, function f(i, language) {
      var codeBlockId = '#' + codeBlock + '-' + language;
      var codeBlockLinkId = '#'  + codeBlock + '-' + language + '-link';
      if(language == codeLanguage) {
        $(codeBlockId).show();
        $(codeBlockLinkId).addClass('language-selected');
      } else {
        $(codeBlockId).hide();
        $(codeBlockLinkId).removeClass('language-selected');
      }
      $(codeBlockId + ' > div').effect('highlight', { color: '#99c9ff' }, 2000);
    });
  }

  $(function() {
    $('#simple-query').load('{{site.baseurl}}/code/simple-query');
    $('#master-query').load('{{site.baseurl}}/code/master-query');
    $('#rcon').load('{{site.baseurl}}/code/rcon');
    $('#community').load('{{site.baseurl}}/code/community');
  });
</script>

<section id="usage-simple-query">
## Querying game servers
<ul class="nav nav-tabs" id="usage-simple-query-selector">
  <li class="active"><a href="#usage-simple-query-java">Java</a></li>
  <li><a href="#usage-simple-query-php">PHP</a></li>
  <li><a href="#usage-simple-query-ruby">Ruby</a></li>
</ul>

<div id="usage-simple-query-content" class="tab-content">
  <div class="tab-pane active" id="usage-simple-query-java">
{% include code/master-query-java.markdown %}
  </div>
  <div class="tab-pane" id="usage-simple-query-php">
{% include code/master-query-php.markdown %}
  </div>
  <div class="tab-pane" id="usage-simple-query-ruby">RUBY</div>
</div>

<script>
$('#usage-simple-query-selector a').click(function (e) {
  e.preventDefault();
  $(this).tab('show');
});
</script>

</section>

<div id="simple-query"></div>

## Querying master servers
<div id="master-query"></div>

## Controlling game servers using RCON
<div id="rcon"></div>

## Getting information from the Steam Community
<div id="community"></div>
