# README

## Awsome Name

* Chat-Space

### Ruby version
* Ruby  => 2.3.1
* Ruby on Rails => '~> 5.0.0' , '>= 5.0.0.1'

### Database initialization

#### tabel : user  (by gem 'devise')

* t.integer :id
>null: false
* t.string :name
>null: false
* t.string :mail
>null: false
* t.string :password
>null: false
* t.timestamp
>null:false

#### table : chat

* t.integer :id
>null: false
* t.references :user_id
>index: true ,
>foreign_key: true
* t.references :group_id
>index: ture ,
>foreign_key: ture
* t.text :text
* t.string :image_url
* t.timestamp
>null: fales

#### table : group

* t.integer :id
>null: false
* t.srting :group_name
* t.references :user_group.id
>index: ture
>foreign_key: true
* t.timestamp

#### table : user_group

* t.integer :id
* t.references :user_id
>foreign_key: ture
* t.references :group_id
>foreign_key: ture
* t.timestamp

<!-- * System dependencies

* Configuration

* How to run the test suite

* Services (job queues, cache servers, search engines, etc.)

* Deployment instructions

* ... -->
