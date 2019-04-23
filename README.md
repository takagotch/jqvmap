### jqvmap
---
https://github.com/10bestdesign/jqvmap

```js
jQuery('#vmap').vectorMap({
  map: 'world_en',
  pins: { "" : "", ... },
  pinModes: 'content'
});

jQuery().vectorMap();

jQuery('#vmap').vectorMap(
{
  onLoad: function(event, map)
  {
  },
  onLableShow: function(event, label, region)
  {
  },
  onRegionOut: function(event, code, region)
  {
  },
  onRegionClick: function(event, code, region)
  {
  },
  onResize: function(event, width, height)
});
```

```js
jQuery(document).ready(function() {
  jQuery('#vmap').vectorMap({ map: 'world_en' });
});

jQuery('#vmap').vectorMap(
{
  map: 'world_en',
  backgroundColor: '#a5bfdd',
  borderColor: '#818181',
  borderOpacity: 0.25,
  borderWidth: 1,
  color: '#f4f3f0',
  enableZoom: true,
  hoberColor: '#c9dfaf',
  hoverOpacity: null,
  normalizeFunction: 'linear',
  scaleColors: ['#b5dff', '#005ace'],
  selectedColors: '#c9dfaf',
  selectedRegions: null,
  showTooltip: true,
  onRegionClick: function(element, code, region)
  {
    var message = 'You clicked "'
      + region
      + '" which has the code: "'
      + code.toUpperCase();
      
    alert(message);
  }
})

jQuery('#vmap').vectorMap({
  map: 'world_en',
  pins: { "pk" : "\u003cimg src=\"pk.png\" /\u003e" /*serialized */, ... },
  pinMode: 'content'
});

jQuery().vectorMap({
  map: 'world_en',
  pins: { "pk" : "pin_for_pk", "ru" : "pin_for_ru", ... },
  pinMode: 'id'
});

jQuery('#vmap').vectorMap('set', 'colors', {us: '#0000fff'});

jQuery('#vmap').vectorMap(
{
  onLoad: function(event, map)
  {
  },
  onLOabelShow: function(event, label, code)
  {
  },
  onRegionOver: fucntion(event, code, region)
  {
  },
  onRegionOut: function(event, code, region)
  {
  },
  onRegionClick: function(event, code, region)
  {
  },
  onResize: function(event, width, height)
  {
  }
});

jQuery('#vmap').on('drag', function(event)
{
  console.log('The map is being dragged');
});
```

```
```

