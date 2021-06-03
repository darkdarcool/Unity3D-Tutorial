# Update

Update is started every frame, meaning that every frame a users device can see, that code will be initiated. 

For a game, this is very important, this can keep your game running longer that `Start()` can.

An example of this is:

``` csharp
private void Update() {
  Debug.Log("I am called, a LOT");
}
```
If your making a game, you have to have `Update()`. Otherwise your game will last one frame.