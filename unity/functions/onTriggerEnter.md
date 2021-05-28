# onTriggerEnter

`onTriggerEnter` is the event on which two objects touch

``` csharp
void OnTriggerEnter(Collider other) {
  // ...
}
```

Even though it's a function, the second the game object touches another, the function is invoked, and the data is sent to the variable, called other, and the data is contains is:

- Tag
- Name
- ect.

The way to get this data is by doing:

``` csharp
void OnTriggerEnter(Collider other) {
  // ..
  Debug.Log(other.name + ":" + other.tag);
}
```

Then it should print out the info! You can use the info in if statment in any way, but the ths example we will kill the player when the enemy touches them:

``` csharp
void OnTriggerEnter(Collider other) {
  if (other.tag == "Player") {
    Destroy(other);
  } 
}
```