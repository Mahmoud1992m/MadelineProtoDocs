---
title: "stats.broadcastStats"
description: "Channel statistics."
nav_exclude: true
image: https://docs.madelineproto.xyz/favicons/android-chrome-256x256.png
redirect_from: /API_docs/constructors/stats_broadcastStats.html
---
# Constructor: stats.broadcastStats  
[Back to constructors index](/API_docs/constructors/index.html)



[Channel statistics](https://core.telegram.org/api/stats).

### Attributes:

| Name     |    Type       | Required | Description |
|----------|---------------|----------|-------------|
|period|[StatsDateRangeDays](/API_docs/types/StatsDateRangeDays.html) | Yes|Period in consideration|
|followers|[StatsAbsValueAndPrev](/API_docs/types/StatsAbsValueAndPrev.html) | Yes|Follower count change for period in consideration|
|views\_per\_post|[StatsAbsValueAndPrev](/API_docs/types/StatsAbsValueAndPrev.html) | Yes|`total_viewcount/postcount`, for posts posted during the period in consideration (`views_per_post`). <br>Note that in this case, `current` refers to the `period` in consideration (`min_date` till `max_date`), and `prev` refers to the previous period (`(min_date - (max_date - min_date))` till `min_date`).|
|shares\_per\_post|[StatsAbsValueAndPrev](/API_docs/types/StatsAbsValueAndPrev.html) | Yes|`total_viewcount/postcount`, for posts posted during the period in consideration (`views_per_post`). <br>Note that in this case, `current` refers to the `period` in consideration (`min_date` till `max_date`), and `prev` refers to the previous period (`(min_date - (max_date - min_date))` till `min_date`)|
|reactions\_per\_post|[StatsAbsValueAndPrev](/API_docs/types/StatsAbsValueAndPrev.html) | Yes|
|views\_per\_story|[StatsAbsValueAndPrev](/API_docs/types/StatsAbsValueAndPrev.html) | Yes|
|shares\_per\_story|[StatsAbsValueAndPrev](/API_docs/types/StatsAbsValueAndPrev.html) | Yes|
|reactions\_per\_story|[StatsAbsValueAndPrev](/API_docs/types/StatsAbsValueAndPrev.html) | Yes|
|enabled\_notifications|[StatsPercentValue](/API_docs/types/StatsPercentValue.html) | Yes|Percentage of subscribers with enabled notifications|
|growth\_graph|[StatsGraph](/API_docs/types/StatsGraph.html) | Yes|Channel growth graph (absolute subscriber count)|
|followers\_graph|[StatsGraph](/API_docs/types/StatsGraph.html) | Yes|Followers growth graph (relative subscriber count)|
|mute\_graph|[StatsGraph](/API_docs/types/StatsGraph.html) | Yes|Muted users graph (relative)|
|top\_hours\_graph|[StatsGraph](/API_docs/types/StatsGraph.html) | Yes|Views per hour graph (absolute)|
|interactions\_graph|[StatsGraph](/API_docs/types/StatsGraph.html) | Yes|Interactions graph (absolute)|
|iv\_interactions\_graph|[StatsGraph](/API_docs/types/StatsGraph.html) | Yes|IV interactions graph (absolute)|
|views\_by\_source\_graph|[StatsGraph](/API_docs/types/StatsGraph.html) | Yes|Views by source graph (absolute)|
|new\_followers\_by\_source\_graph|[StatsGraph](/API_docs/types/StatsGraph.html) | Yes|New followers by source graph (absolute)|
|languages\_graph|[StatsGraph](/API_docs/types/StatsGraph.html) | Yes|Subscriber language graph (pie chart)|
|reactions\_by\_emotion\_graph|[StatsGraph](/API_docs/types/StatsGraph.html) | Yes|
|story\_interactions\_graph|[StatsGraph](/API_docs/types/StatsGraph.html) | Yes|
|story\_reactions\_by\_emotion\_graph|[StatsGraph](/API_docs/types/StatsGraph.html) | Yes|
|recent\_posts\_interactions|Array of [PostInteractionCounters](/API_docs/types/PostInteractionCounters.html) | Yes|



### Type: [stats.BroadcastStats](/API_docs/types/stats.BroadcastStats.html)


### Example:

```
$stats_broadcastStats = ['_' => 'stats.broadcastStats', 'period' => StatsDateRangeDays, 'followers' => StatsAbsValueAndPrev, 'views_per_post' => StatsAbsValueAndPrev, 'shares_per_post' => StatsAbsValueAndPrev, 'reactions_per_post' => StatsAbsValueAndPrev, 'views_per_story' => StatsAbsValueAndPrev, 'shares_per_story' => StatsAbsValueAndPrev, 'reactions_per_story' => StatsAbsValueAndPrev, 'enabled_notifications' => StatsPercentValue, 'growth_graph' => StatsGraph, 'followers_graph' => StatsGraph, 'mute_graph' => StatsGraph, 'top_hours_graph' => StatsGraph, 'interactions_graph' => StatsGraph, 'iv_interactions_graph' => StatsGraph, 'views_by_source_graph' => StatsGraph, 'new_followers_by_source_graph' => StatsGraph, 'languages_graph' => StatsGraph, 'reactions_by_emotion_graph' => StatsGraph, 'story_interactions_graph' => StatsGraph, 'story_reactions_by_emotion_graph' => StatsGraph, 'recent_posts_interactions' => [PostInteractionCounters, PostInteractionCounters]];
```  
