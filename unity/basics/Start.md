# Start

Start is an optional function in Unity that you can put on a game object, and everything in that function will be exacuted when your game starts. This allows you to do some things when your game starts, that you only want to be done once. 

Take this:

``` csharp
private void Start() {
  Debug.Log("This will be done once at the start of your game!");
} 
```
That was the start function! If you don't need it, you don't have to put it in your game!