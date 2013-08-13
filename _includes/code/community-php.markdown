```php
$id = SteamId::create('demomenz');
$stats = $id->getGameStats('tf2');
$achievements = $stats->getAchievements();
```