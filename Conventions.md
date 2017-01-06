# Conventions

### Naming
|Type|Example|Rule|
|----|-------|----|
|Variable|`var flySpeed = 1.4f;`|lowerCamelCase|
|Field (local)|`private Vector3 coor;`|lowerCamelCase|
|Field (global)|`public int Port { get; set; }`|UpperCamelCase|
|Field (bool)|`public bool IsRunning { get; set; }`|*Is*Upper(/Lower)CamelCase|
|Constant|`private const DOWNFORCE = 4;`|CAPS|
|Backingfield|`private int _port;`|*_*lowerCamelCase|
|Parameter|`private void StartServer(int port) { }`|lowerCamelCase|
|Method|`private void StartServer() { }`|UpperCamelCase|
|Function (bool)|`public bool IsEnabled() { }`|*Is/Has/...*UpperCamelCase|
|Function (!bool)|`public IEnumerable<Player> GetPlayers() { }`|*Get*UpperCamelCase|
|Enums|`public Enum EntityType { Player, Armorstand, ... }`|UpperCamelCase|

|Other|
|-----|
|Start interfaces with `I`.|
|Start delegates with `D`.|
|Explicitly type `private`.|
|Explicitly type `{}` even on singleline if/loops.|
|Use `var` instead of explicit declaration.|
|Use object initializer where possible.|
|Use first letter of type for anonymous lambda functions. `Players.Find(p => p.UUID == ...)`|
|Do no indent `case` in `switch` structures.|

### Spacing
|Position|Space?|Example|
|--------|------|-------|
|Around `()`|No|`StartServer();`|
|Inside `()`|No|`StartServer(address, port);`|
|Around `{}`|Only before|`var minecart = new Entity { Type = EntityType.Minecart };`|
|Inside `{}`|Yes|`public Guid UUID { get; private set; }`|
|Inside `{}` in interpolation|No|`var message = $"{player.Name} died.";`|
|Around `[]`|No|`private float[] values = new[] { };`|
|Inside `[]`|No|`var value = values[42];`|
|Around operators|Yes|`var totalSpeed = playerSpeed * potionEffect;`|
|Around prefix/suffix operators|No|`totalSpeed++;`|
|Around `,`|Only behind|`StartServer(address, port);`|
|Around `.`|No|`Player.Saturation = 5;`|
|Around `?`|No|`SomeEvent?.Invoke();`|
|Around `;`|No|`SomeEvent?.Invoke();`|
|Around keywords|Yes|`if (...)` / `foreach (...)`|

### Wrapping
|Position|Wrap?|`{` in new line?|
|--------|-----|----------------|
|Namespace|Yes|Yes|
|Class/Enum/...|Yes|Yes|
|Public fields|No|No|
|Object initializers|Yes|Only the last|
|If/Try/Loops/...|Yes|No|
|Else/Catch/Finally/...|No|No|
|Methods/Functions/...|Yes|No|

#### Example Code
```csharp
namespace Project
{
  class Player
  {
    public int Health { get; set; }
    
    public Player() {
      [...]
    }
    
    public void ShowInventory() {
      var inventory = new Inventory {
        Slots = 9,
        Title = "Inventory"
      };
      if (!Player.IsMoving) {
        try {
          [...]
        } catch {}
      } else {
        [...]
      }
    }
    
  }
}
```

