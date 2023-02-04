# Note for Rustlings Exercise

### enums3:

`match enums`: Reuse of parameter

```rust
match message{
        Message::ChangeColor((x, y, z)) => self.change_color((x , y, z)),
        Message::Move(point) => self.move_position(point),
        Message::Echo(string)=> self.echo(string),
        _ => self.quit(),
    }
```
