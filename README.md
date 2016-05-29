# SceneScape Common Scenes and Templates

These auto-generated scenes and templates are available to all
SceneScapes.  

## Common Scenes

The common scenes are available to be displayed at any point in the
SceneScape folder hierarchy, by simply entering that scene name at the
end of the address to a particular point in the SceneScape folder
hierarchy.  For example, to render a default scene called "googlemap"
that presents a map of all scenes in the PAX (Portrait of America at
the Crossroads) SceneScape, use:

```
    http://www.scenescape.com/pax/googlemap
```

If no scene is included, then the "default" common scene is used, so
the following two addresses produce the same view:


```
    http://www.scenescape.com/pax
    http://www.scenescape.com/pax/default
```

The following default scenes are currently available:

| Scene name |  Description |
| ------------- | ----------------------------------- |
| default  | Incorporates the scenelisting template (below) to  render a listing view of all scenes under a certain point in the SceneScape folder hierarchy |

## Creating Your Own Default Scene

Note that it's typically beneficial to create a default scene in each
(or many) of the folders of your SceneScape hierarchy, to provide
properties, such as a title.  For example, leveraging the scenelisting
template, such as "default.scene" file may be as simple as the
following:

```
<scene stage="listing">
  <sceneprops>
    <title>Portrait of America at the Crossroads</title>
  </sceneprops>

  {% insert t_scenelisting() %}
</scene>
```

## 

## Common Templates

These common templates can be inserted into any scene by inserting
them into a SceneScape script using an insert instruction like:

```
    {% insert t_scenelisting() %}
```

(The 't_' prefix identifies it as a template.)

The following common templates are currently available:

| Template name | Arguments | Description |
| ------------- | ------------- | ----------------------------------- |
| scenelisting | none | Produces a listing view of all scenes under a certain point in the SceneScape folder hierarchy |

