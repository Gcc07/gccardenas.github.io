## Task from Evan:
### Create a entity diagram as would be used in a Video Game.(Borrowing insipriation from Terraria Documentation) (C#)
https://docs.tmodloader.net/docs/stable/class_entity.html\
https://docs.tmodloader.net/docs/stable/class_player.html

``` mermaid
classDiagram
class Entity {
        name: string
        health: float
        position: Vector2D
        +DirectionTo(): void
    }

    class Player {
        +deadForGood: bool
        +difficulty: byte
        +Update(): void
    }

    class Non-Playable-Character{
        +ai: array
        +boss: bool
        +defense: int
        +damage: int
        +AI(): void
    } 

    Entity <|-- Player
    Entity <|-- Non-Playable-Character
```
