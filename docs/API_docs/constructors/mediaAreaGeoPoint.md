---
title: "mediaAreaGeoPoint"
description: "Represents a geolocation tag attached to a story."
nav_exclude: true
image: https://docs.madelineproto.xyz/favicons/android-chrome-256x256.png
---
# Constructor: mediaAreaGeoPoint  
[Back to constructors index](/API_docs/constructors/index.html)



Represents a geolocation tag attached to a [story](https://core.telegram.org/api/stories).

### Attributes:

| Name     |    Type       | Required | Description |
|----------|---------------|----------|-------------|
|coordinates|[MediaAreaCoordinates](/API_docs/types/MediaAreaCoordinates.html) | Yes|The size and position of the media area corresponding to the location sticker on top of the story media.|
|geo|[GeoPoint](/API_docs/types/GeoPoint.html) | Optional|Coordinates of the geolocation tag.|



### Type: [MediaArea](/API_docs/types/MediaArea.html)


### Example:

```
$mediaAreaGeoPoint = ['_' => 'mediaAreaGeoPoint', 'coordinates' => MediaAreaCoordinates, 'geo' => GeoPoint];
```  
