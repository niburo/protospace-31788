# テーブル設計

## users テーブル

| Column   | Type   | Options     |
| -------- | ------ | ----------- |
| name     | string | not:  null  |
| email    | string | not:  null  |
| password | string | not:  null  |
| profile  | text   | not:  null  |
|occupation| text   | not:  null  |
|position  | text   | not:  null  |


## prototypes テーブル

| Column     | Type          | Options    |
| ---------- | ------------- | ---------- |
| title      | string        | not:  null |
| catch_copy | text          | not:  null |
| concept    | text          | not:  null |
| image      | ActiveStorage | not:  null |
| user       | references    | not:  null |




## comments テーブル

| Column    | Type       | Options    |
| --------- | ---------- | ---------- |
| text      | text       | not:  null |
| user      | references |            |
| prototype | references |            |