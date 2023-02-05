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

### hashmaps3

`reference`: &*

```rust

let team1 = Team{
    name: team_2_name.clone(),
    goals_scored: 0, 
    goals_conceded: 0};

let team2 = Team{
    name: team_1_name.clone(), 
    goals_scored: 0, 
    goals_conceded: 0};
  
  
let value1 = scores.entry(team_1_name.to_string()).or_insert(team1);
(*value1).goals_scored += team_1_score;
(*value1).goals_conceded += team_2_score;

let value2 = scores.entry(team_2_name.to_string()).or_insert(team2);
(*value2).goals_scored += team_2_score;
(*value2).goals_conceded += team_1_score;
```




