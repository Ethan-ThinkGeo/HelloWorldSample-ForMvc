# Hello World Sample for Mvc

### Description
This sample shows you how to get started building your first application with the Map Suite Web for Mvc 10.0.0.

Please refer to [Wiki](http://wiki.thinkgeo.com/wiki/map_suite_web_for_mvc) for the details.

![Screenshot](https://github.com/ThinkGeo/HelloWorldSample-ForMvc/blob/master/Screenshot.png)

### Requirements
This sample makes use of the following NuGet Packages

[MapSuite 10.0.0](https://www.nuget.org/packages?q=ThinkGeo)

### About the Code

```csharp

 @{Html.ThinkGeo().Map("Map1", 600, 500)
                                        .MapBackground(new GeoSolidBrush(GeoColor.FromHtml("#E5E3DF")))
                                        .CurrentExtent(-131.22, 55.05, -54.03, 16.91)
                                        .MapUnit(GeographyUnit.DecimalDegree)
                                        .CustomOverlays(overlays =>
                                        {
                                            overlays.WorldMapKitWmsWebOverlay();

                                        })
                                        .Render();
    }

```

### Getting Help

[Map Suite web for Mvc Wiki Resources](http://wiki.thinkgeo.com/wiki/map_suite_web_for_mvc)

[Map Suite web for Mvc Product Description](https://thinkgeo.com/ui-controls#web-platforms)

[ThinkGeo Community Site](http://community.thinkgeo.com/)

[ThinkGeo Web Site](http://www.thinkgeo.com)

### Key APIs
This example makes use of the following APIs:

- [ThinkGeo.MapSuite.Mvc.WorldMapKitWmsWebOverlay](http://wiki.thinkgeo.com/wiki/api/thinkgeo.mapsuite.mvc.worldmapkitwmsweboverlay)

### About Map Suite
Map Suite is a set of powerful development components and services for the .Net Framework.

### About ThinkGeo
ThinkGeo is a GIS (Geographic Information Systems) company founded in 2004 and located in Frisco, TX. Our clients are in more than 40 industries including agriculture, energy, transportation, government, engineering, software development, and defense.
