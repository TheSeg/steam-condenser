{% highlight java %}
SteamId id = SteamId.create("demomenz");
GameStats stats = id.getGameStats("tf2");
List<GameAchievement> achievements = stats.getAchievements();
{% endhighlight %}