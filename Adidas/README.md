#  📋Adidas Project

## About

In this project, I analyzed and cleaned data from an Adidas Dataset using pivot tables. I then created an example Dashboard within Excel for essential findings.

## Tools and Technologies

- Data Set : [Adidas Dateset](https://www.kaggle.com/datasets/heemalichaudhari/adidas-sales-dataset)
- Excel: Analysis and Dashboard

**Dashboard**

<img width="1371" alt="image" src="https://github.com/KevinWongSF/Portfolio/assets/136656858/2352fab4-84e7-485a-b528-00d09e8052ea">

## Setup

### Create Pivot Tables

To materialise models in dbt and Snowflake, run `dbt run` in termimal.

<img width="825" alt="Screenshot 2023-02-27 at 11 19 35 AM" src="https://github.com/KevinWongSF/Portfolio/assets/136656858/5fed3e00-ccaf-4139-82e0-13a42501c5a0">

<img width="825" alt="Screenshot 2023-02-27 at 11 19 35 AM" src="https://github.com/KevinWongSF/Portfolio/assets/136656858/d0a396b8-d35c-48c9-8db5-f2a3720a5c0e">

### Snapshots

Snapshots are created using a snapshot block with configs onto a SELECT statement.

Here's an example of what a snapshot looks like:



<img width="611" alt="image" src="https://github.com/KevinWongSF/Portfolio/assets/136656858/2bce2289-da87-4c94-aae6-fdfd73f1a4ba">

Snapshot automatically includes the columns `dbt_scd_id`, `dbt_updated_at`, `dbt_valid_from` and `dbt_valid_to`. In the first snapshot, `dbt_valid_to` is `null` because this column contains date of the next most recent changes or snapshot. 

<img width="1136" alt="image" src="https://user-images.githubusercontent.com/81607668/221782810-89766268-0725-4b95-a121-974423892382.png">

Let's say I make a change in id=3176 and ran `dbt snapshot` again. You'll see that `dbt_valid_to` contains the current timestamped and the next line represents id 3176 as well with a null `dbt_valid_to`.

<img width="833" alt="image" src="https://user-images.githubusercontent.com/81607668/221783996-15275e80-e3ac-4fb8-84c1-2882b061f585.png">

***

### Documentation

I ran `dbt docs serve` to open into website.

<img width="1360" alt="image" src="https://user-images.githubusercontent.com/81607668/222343062-d9465f5e-0802-4ed6-8432-b6aa36afd371.png">
