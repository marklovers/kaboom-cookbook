# shadow() - Give your objects a shadow that follows it

Apply this component to a game object for a shadow that:

* follows the object
* respects platforms, holes, etc.
* Gets subtly larger and smaller depending on how close the object is

It works by always "falling" until it hits a solid object (ie "the ground").

## Requires

* A sprite called "shadow"
* A layer named "effects" that's "on top of" the floor (though you could edit the component to be anything you'd like)

## Parameters

* None

## Example

```.js

"P": () => [
  k.sprite("player"),
  k.solid(),
  shadow(),
  (etc.)
  
```
