---
layout:       default
title:        First Post
---


This is a first post!

{% highlight php startinline %}
$master = new MasterServer(MasterServer::GOLDSRC_MASTER_SERVER);
$servers = $master->getServers();
$randomServer = $servers[array_rand($servers)];
$server = new GoldSrcServer($randomServer[0], $randomServer[1]));
{% endhighlight %}

{% highlight ruby %}
def show
  @widget = Widget(params[:id])
  respond_to do |format|
    format.html # show.html.erb
    format.json { render json: @widget }
  end
end
{% endhighlight %}