# tippitytappity-design

tippitytappity is a program to practice typing


## Data model

```mermaid
classDiagram
  ExampleParent <|-- ExampleChild
  class ExampleParent{
        - name: string
        - email: string
        - password: string
        + login(user: string, pass: string) boolean
        + get_email() string
  }
  class ExampleChild{
        - badges vector~string~
        - body_to_type: string
        - correct_letter_counter: int
        - correct_input: bool
        - current_index: int
        - start_timer: datetime
        - duration: duration

        + add_badge(title: string)
        + get_badges() vector~string~
        + start_timer() void
        + get_duration() duration
        + is_correct() bool
        + calculate_wpm() int
  }
```
