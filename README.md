# テーブル設計

## userテーブル

| Column | Type      | Options          |
| ------ | --------- | ---------------- |
| email  | string    | nul: false       |
| password  | string    | nul: false       |
| name  | string    | nul: false       |
| profile  | text    | nul: false       |
| occupation  | text    | nul: false       |
| position  | text    | nul: false       |


## prototypesテーブル
| Column | Type      | Options          |
| ------ | ---------- | ---------------------------- |
| title | string    | nul: false       |
| catch_copy | text    | nul: false       |
| concept  | text    | nul: false       |
| user_id  | references | nul: false, foreign_key: true |


## commentsテーブル
| Column | Type      | Options          |
| ------ | ---------- | ---------------- |
| text | text    | nul: false       |
| user_id | references | nul: false, foreign_key: true |
| prototype  | references | nul: false, foreign_key: true |------------------
