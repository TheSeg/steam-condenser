---
layout:      default
title:       Usage
---
<section id="usage-simple-query">
## Querying game servers
<ul class="nav nav-tabs" id="usage-simple-query-selector">
  <li class="active"><a href="#usage-simple-query-java">Java</a></li>
  <li><a href="#usage-simple-query-php">PHP</a></li>
  <li><a href="#usage-simple-query-ruby">Ruby</a></li>
</ul>

<div id="usage-simple-query-content" class="tab-content">
<div class="tab-pane active" id="usage-simple-query-java">
{% capture simplequeryjava %}
{% include code/simple-query-java.markdown %}
{% endcapture %}
{{ simplequeryjava | unindent | markdownify }}
</div>
<div class="tab-pane" id="usage-simple-query-php">
{% capture simplequeryphp %}
{% include code/simple-query-php.markdown %}
{% endcapture %}
{{ simplequeryphp | unindent | markdownify }}
</div>
<div class="tab-pane" id="usage-simple-query-ruby">
{% capture simplequeryruby %}
{% include code/simple-query-ruby.markdown %}
{% endcapture %}
{{ simplequeryruby | unindent | markdownify }}
</div>
</div>

</section>

<section id="usage-master-query">
## Querying master servers

<ul class="nav nav-tabs" id="usage-master-query-selector">
  <li class="active"><a href="#usage-master-query-java">Java</a></li>
  <li><a href="#usage-master-query-php">PHP</a></li>
  <li><a href="#usage-master-query-ruby">Ruby</a></li>
</ul>

<div id="usage-master-query-content" class="tab-content">
<div class="tab-pane active" id="usage-master-query-java">
{% capture masterqueryjava %}
{% include code/master-query-java.markdown %}
{% endcapture %}
{{ masterqueryjava | unindent | markdownify }}
</div>
<div class="tab-pane" id="usage-master-query-php">
{% capture masterqueryphp %}
{% include code/master-query-php.markdown %}
{% endcapture %}
{{ masterqueryphp | unindent | markdownify }}
</div>
<div class="tab-pane" id="usage-master-query-ruby">
{% capture masterqueryruby %}
{% include code/master-query-ruby.markdown %}
{% endcapture %}
{{ masterqueryruby | unindent | markdownify }}
</div>
</div>

</section>

<section id="usage-rcon">
## Controlling game servers using RCON
<ul class="nav nav-tabs" id="usage-rcon-selector">
  <li class="active"><a href="#usage-rcon-java">Java</a></li>
  <li><a href="#usage-rcon-php">PHP</a></li>
  <li><a href="#usage-rcon-ruby">Ruby</a></li>
</ul>

<div id="usage-rcon-content" class="tab-content">
<div class="tab-pane active" id="usage-rcon-java">
{% capture rconjava %}
{% include code/rcon-java.markdown %}
{% endcapture %}
{{ rconjava | unindent | markdownify }}
</div>
<div class="tab-pane" id="usage-rcon-php">
{% capture rconphp %}
{% include code/rcon-php.markdown %}
{% endcapture %}
{{ rconphp | unindent | markdownify }}
</div>
<div class="tab-pane" id="usage-rcon-ruby">
{% capture rconruby %}
{% include code/rcon-ruby.markdown %}
{% endcapture %}
{{ rconruby | unindent | markdownify }}
</div>
</div>

</section>

<section id="usage-community">
## Getting information from the Steam Community
Getting the Steam Community profile of Valve's [Adrian Finol](http://steamcommunity.com/id/demomenz) and his <abbr title="Team Fortress 2">TF2</abbr> achievements.
<ul class="nav nav-tabs" id="usage-community-selector">
  <li class="active"><a href="#usage-community-java">Java</a></li>
  <li><a href="#usage-community-php">PHP</a></li>
  <li><a href="#usage-community-ruby">Ruby</a></li>
</ul>

<div id="usage-community-content" class="tab-content">
<div class="tab-pane active" id="usage-community-java">
{% capture communityjava %}
{% include code/community-java.markdown %}
{% endcapture %}
{{ communityjava | unindent | markdownify }}
</div>
<div class="tab-pane" id="usage-community-php">
{% capture communityphp %}
{% include code/community-php.markdown %}
{% endcapture %}
{{ communityphp | unindent | markdownify }}
</div>
<div class="tab-pane" id="usage-community-ruby">
{% capture communityruby %}
{% include code/community-ruby.markdown %}
{% endcapture %}
{{ communityruby | unindent | markdownify }}
</div>
</div>

</section>


<script>
$('#usage-simple-query-selector a,#usage-master-query-selector a,#usage-rcon-selector a,#usage-community-selector a').click(function (e) {
  e.preventDefault();
  $(this).tab('show');
});
</script>
