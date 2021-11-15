# RecyclerView for displaying lists of data

## Create dynamic lists with RecyclerView

RecyclerView makes it easy to efficiently display large sets of data. You supply the data and define how each item looks, and the RecyclerView library dynamically creates the elements when they're needed.

## Key classes

different classes work together to build your dynamic list.

* RecyclerView is the ViewGroup that contains the views corresponding to your data.
* Each individual element in the list is defined by a view holder object.
* the RecyclerView requests those views, and binds the views to their data, by calling methods in the adapter.
* The layout manager arranges the individual elements in your list

## Steps for implementing your RecyclerView

1. decide what the list or grid is going to look like.

2. Design how each element in the list is going to look and behave. 

3. Define the Adapter that associates your data with the ViewHolder views.


## Plan your layout

The items in your RecyclerView are arranged by a LayoutManager class.

* LinearLayoutManager arranges the items in a one-dimensional list.

* GridLayoutManager arranges all items in a two-dimensional grid: If the grid is arranged vertically or horizontally

* StaggeredGridLayoutManager is similar to GridLayoutManager, but it does not require that items in a row have the same height  or items in the same column have the same width 

## Implementing your adapter and view holder

you need to implement your Adapter and ViewHolder.

When you define your adapter, you need to override three key methods:

* onCreateViewHolder(): RecyclerView calls this method whenever it needs to create a new ViewHolder.

* onBindViewHolder(): RecyclerView calls this method to associate a ViewHolder with data

* getItemCount(): RecyclerView calls this method to get the size of the data set. 

