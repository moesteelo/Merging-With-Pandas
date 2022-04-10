# Merging-With-Pandas

**Practicing different Merging Techniques in Pandas**

## Overview

**Learning how to merge multiple data frames together is an essentail skill to have in the data programming world.** 

## Results 

### Left_merge

**Using the left_merge in the data frames "user_usage" and "user-device" we can merge both data frames on the `how="left"` method**

<img src= "img/left_merge.png" >

### Right_merge

**Using the left_merge in the data frames "user_usage" and "user-device" we can merge both data frames on the `how="right"` method**

<img src= "img/right_merge.png" >

## Difference Between Left_merge and Right_merge

**The difference between the Left_merge and Right_merge data frames is that in the Right_merge method it replaced all the NaN values that were present in the Left_merge method.**

<img src= "img/left-merge-tail.png" > <img src= "img/right-merge-tail.png" >

## Inner_merge 

**The Inner_merge method is the default method the used in Pandas by default. The Inner_method only keeps the common values in both the left and right dataframes for the merged data. In this case only the rows that contain `use_id` values are the common between `user_usage` and `user_device` remain in the merged data.**

<img src= "img/Inner_merge.png" >


## Outer_merge

**The "outer' merge combies all the rows for the left and right dataframes with nan when ther are no matached values in the rows.**

- **The 1st and 2th rows, the rows come from both dataframes as they have the same values of `use_id` to be merged.**

- **The 3rd and 4th rows, the rows come from the left dataframe as the right dataframe doesn't have the common vales of `use_id`.**

- **The 5th and 6th rows, the rows come from the right dataframes as the left dataframe doesn't have the common values of `use_id`.**


## Merge Dataframes with Differnt Column Names 

**Understanding various merge methods allows us to understand that the `on` method can only work if both the right and left dataframes have the same column name. Therefore, we use the `left_on` method and `right_on` to replace the method `on`. Using. the user_device and android_device sinc they both contain common codes in their columns `device` and `Model`.**


<img src= "img/Different-Column names.png" >

## Resources 

- [user_usage]("user_usage.csv")

- [user_device]("user_device.csv")

- [android_device]("android_devices.csv")

- [Article](https://towardsdatascience.com/why-and-how-to-use-merge-with-pandas-in-python-548600f7e738)


