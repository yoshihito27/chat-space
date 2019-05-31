## members table

|Column|Type|Options|
|------|----|-------|
|user|references|null: false, foreign_key: true|
|group|references|null: false, foreign_key: true|

### Association
- belongs_to :group
- belongs_to :user

## users table

|Column|Type|Options|
|------|----|-------|
|name|string|index:true, null: false, unique:true|
|mail|string|null:false|

## Assosiation

- has_many :groups, through: members
- had_many :messeages
- has_many :members
