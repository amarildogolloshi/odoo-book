.. _openerp-search:

.. index::
   single: Search Box
   single: Advance Search
   single: Save Search
   single: Quick Filters

Search & Advance Search on List
===============================
Search in OpenERP is similar to spotlight in Mac OS, you can search anything in OpenERP depending on where you are. You can get the search control in all the views except Form View, where you can perform search on the related contents. 

.. image:: images/searchbox.png

Search Box in OpenERP

Lets say if you are on the Product list, when you enter some search criteria in to the search box, it give you all the possibilities related to to that string. As an example you can see that we can search for all product where name contains "computer" or browse the all the product who belongs to the "computer" category.

.. note::
	If you enter two search criteria in search box, apply one after other, it will apply ``and`` operator between those criteria.
	
Quick Filters
-------------
Enter search criteria in to the search box always performs quick filters. Some of the document have defined ``Filters`` to filter the data effectively. Like searching for the all the product which can be sold it will be difficult to derived using advance filters. All those basic search criteria can be defined as filters during the development and we can use those quickly from the advance search options.

To get the advance search options, click on the down-arrow on search box appear on the right side. On click on that you will be able to see all the possible advance filters available for products. 

.. image:: images/search-advance.png

Search Box in OpenERP with Advance Options

Filters
~~~~~~~
We can see that some of the predefine criteria listed under the ``Filters`` options such as Service, Product, Consumable, To Purchase, Can be Sold, Etc.., On click on filters predefined criteria applied on the list and it filters accordingly.
If you select multiple filters, like the quick text filters, it will apply ``and`` operator between those selected advance filters.


Group By
~~~~~~~~
Data can be grouped in List, Kanban, or Groups Views. In List view you can have a flexibility to have unlimited levels of grouping while other views there is a limitations with grouping. Grouping is applied based on series of clicks performed on the group options. Like among two groups options ``Category`` and ``Default Unit of Measure Type`` available but it will apply first depends on what you select first. 

* Product by Category and Default Unit of Measure Type - If you select first ``Category`` and then ``Default Unit of Measure Type``
* Product by Default Unit of Measure Type and Category  - If you select first ``Default Unit of Measure Type`` and then ``Category``

.. image:: images/product-search-group.png

Apply Filters and Group

From above image "Apply Filters and Group" you can understand that we have select all Stock-able Products which can be Sold Group By Category.

Advance Search
--------------
To perform more advance search which are not available with Quick Search or Filters like select product whose Sale price in between 50 to 500. We can perform these kind of search with advance search and save them using Save advance search option.
While working with advance search we can define search operator and conditions between two conditions. If you add more then one conditions in single search it always be treated with ``OR`` operator. 

So, If you want to apply ``AND`` operator while working with Advance Search after each advance search option, apply and perform advance search again.

.. image:: images/advance-search.png

Apply Advance filters

Save Current Filter
-------------------
When you done with the advance search, If you don't want to lost that complex search criteria you can save those filters using Save current filters options available under Advance Search.

.. image:: images/save-search.png

Apply Filters and Group

It will save all the applied criteria along with the group by options. An interesting thing is while saving the filters you can choose scope of those filters from the available scopes as below.

* Share with all Users : If you check this options whatever search you have perform and save that will be available to all the users who have access on that document. 
* Use by Default : If you check this options next time when you open product list it will apply this filter by default.

.. warning::
	If you select wrong options while Saving Custom Filters, You can still change options of filters, from Manage Filters. You have to enter in to debug mode to get the Manage Filters option. 