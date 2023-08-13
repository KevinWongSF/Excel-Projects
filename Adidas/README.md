#  📋Adidas Project

## About

In this project, I analyzed and cleaned data from an Adidas Dataset using pivot tables. I then created an example Dashboard within Excel for essential findings.

## Tools and Technologies

- Data Set : [Adidas Dateset](https://www.kaggle.com/datasets/heemalichaudhari/adidas-sales-dataset)
- Excel: Analysis and Dashboard
**Clean Dataset**
  
  <img width="1371" alt="image" src="https://github.com/KevinWongSF/Portfolio/assets/136656858/b8f4ba59-b049-47a5-8bb7-ee9a227fcb8d">
  
**Dashboard**

<img width="1371" alt="image" src="https://github.com/KevinWongSF/Portfolio/assets/136656858/2352fab4-84e7-485a-b528-00d09e8052ea">

## Setup

### Create Pivot Tables

Here I created pivot tables to gather information  

<img width="825" alt="Screenshot 2023-02-27 at 11 19 35 AM" src="https://github.com/KevinWongSF/Portfolio/assets/136656858/5fed3e00-ccaf-4139-82e0-13a42501c5a0">

<img width="825" alt="Screenshot 2023-02-27 at 11 19 35 AM" src="https://github.com/KevinWongSF/Portfolio/assets/136656858/d0a396b8-d35c-48c9-8db5-f2a3720a5c0e">



Snapshot automatically includes the columns `dbt_scd_id`, `dbt_updated_at`, `dbt_valid_from` and `dbt_valid_to`. In the first snapshot, `dbt_valid_to` is `null` because this column contains date of the next most recent changes or snapshot. 

<img width="1136" alt="image" src="https://user-images.githubusercontent.com/81607668/221782810-89766268-0725-4b95-a121-974423892382.png">

Let's say I make a change in id=3176 and ran `dbt snapshot` again. You'll see that `dbt_valid_to` contains the current timestamped and the next line represents id 3176 as well with a null `dbt_valid_to`.

<img width="833" alt="image" src="https://user-images.githubusercontent.com/81607668/221783996-15275e80-e3ac-4fb8-84c1-2882b061f585.png">

***

