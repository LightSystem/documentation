========
Services
========

To properly maintain a fleet of vehicles, regular maintenance as well as periodic repairs are
needed. Scheduling repairs and managing services for an entire fleet is necessary to ensure all
vehicles are in good working order when they are needed.

.. _services/service-form:

Create a service record
=======================

To log a service, go to the main services dashboard by navigating to :menuselection:`Fleet app -->
Fleet --> Services`. Click the :guilabel:`New` button in the top-left corner, and a new service form
loads.

Fill out the information on the form. The only two fields that are required to be populated are
:guilabel:`Service Type` and :guilabel:`Vehicle`.

The service form automatically saves as data is entered. However, the form can be saved manually at
any time by clicking the :guilabel:`Save manually` option, represented by a :guilabel:`cloud with an
upwards arrow inside` icon.

The fields on the form are:

- :guilabel:`Description`: enter in a short description of the service.
- :guilabel:`Service Type`: select the type of service performed using the drop-down menu, or enter
  a new type of service and click either :guilabel:`Create "service type"` or :guilabel:`Create &
  Edit...` to :ref:`add the service type and configure it <services/new-type>`.

  .. note::
     :guilabel:`Service Types` are **not** pre-configured in Odoo. When logging a service for the
     first time, the *type* of service need to :ref:`first be created <services/new-type>` before
     it can be selected.

- :guilabel:`Date`: using the calendar popover, select the date the service was provided or is
  scheduled to be performed. Navigate to the desired month using the :guilabel:`< > (arrow)` icons,
  then click on the date to select it.
- :guilabel:`Cost`: enter the cost of the service.
- :guilabel:`Vendor`: select the vendor who performed the service using the drop-down menu. If the
  vendor has not already been entered in the system, type in the vendor name and click either
  :guilabel:`Create` to add them, or  :guilabel:`Create and edit...` to :ref:`add and configure the
  vendor <services/new-vendor>`.
- :guilabel:`Vehicle`: select the vehicle that was serviced from the drop-down menu. When the
  vehicle is selected, the :guilabel:`Driver` field is populated, and the unit of measure for the
  :guilabel:`Mileage` field appears.
- :guilabel:`Driver`: the current driver listed for the selected vehicle is populated when the
  :guilabel:`Vehicle` is selected. If the driver needs to be changed, another driver can be selected
  from the drop-down menu.
- :guilabel:`Odometer Value`: enter the odometer reading when the service was done. The units of
  measure will either be in kilometers (:guilabel:`km`) or miles (:guilabel:`mi`). When the
  :guilabel:`Vehicle` is selected, the units of measure is populated. This comes from the vehicle
  form. To change from kilometers to miles, or vice versa, click the :guilabel:`External Link`
  button next to the vehicle selected in the :guilabel:`Vehicle` field. Change the unit of measure,
  then click :guilabel:`Save`. The unit of measure is updated in the :guilabel:`Odometer Value`
  field.
- :guilabel:`Notes`: enter any notes for the repair in the notes tab at the bottom of the service
  form.

.. image:: service/new-service.png
   :align: center
   :alt: Enter the information for a new service. The required fields are Service Type and Vehicle.

.. _services/new-type:

Create service type
-------------------

Service types must be created from a service form, there is no other way to access the list of
service types.

On the :ref:`service form <services/service-form>`, type in the name of the new :guilabel:`Service
Type` in the field. Then, click :guilabel:`Create and edit...` and a :guilabel:`Create Service Type`
form appears.

The service type entered on the service form populates the :guilabel:`Name` field by default. This
field can be modified if desired.

Using the drop-down menu, select the :guilabel:`Category` this new service type falls under, if any.
The two default options to chose form are :guilabel:`Contract` or :guilabel:`Service`. Additional
categories cannot be created.

If the service applies to **only** contracts or services, select the corresponding
:guilabel:`Category`. If the service applies to **both** contracts *and* services, leave this field
blank.

When done, click :guilabel:`Save & Close`.

.. _services/new-vendor:

Create vendor
-------------

When a service is done for the firts time, typically the vendor is not already in the database. It
is best practice to add the full details for a vendor in the databse, so any necessary infomration
is easily retrieved.

On the :ref:`service form <services/service-form>`, type in the name of the new :guilabel:`Vendor`
in the field. Then, click :guilabel:`Create and edit...` and a :guilabel:`Create Vendor` form
appears.

The vendor name entered on the service form populates the :guilabel:`Name` field by default. This
field can be modified if desired.

List of services
================

To view all services logged in the database, including old and new requests, go to
:menuselection:`Fleet application --> Fleet --> Services`. All services appear in a list view,
including all the details for each service.

Each service listed displays the following information:

- :guilabel:`Date`: the date service or repair was performed or is requested to be performed.
- :guilabel:`Description`: a short description of the specific type of service or repair performed
  to clarify the specific service.
- :guilabel:`Service Type`: the service or repair performed. This is selected from a list of
  services that must be configured.
- :guilabel:`Vehicle`: the specific vehicle the service was performed on.
- :guilabel:`Driver`: who the current driver is for the vehicle.
- :guilabel:`Vendor`: the specific vendor who performed the service or repair.
- :guilabel:`Cost`: the total cost for the service or repair.
- :guilabel:`Notes`: any information associated with the service or repair that is documented to add
  clarification.
- :guilabel:`Stage`: the status of the service or repair. Options are :guilabel:`New`,
  :guilabel:`Running`, :guilabel:`Canceled`, or :guilabel:`Done`.

.. image:: service/services.png
   :align: center
   :alt: The full list of services in the Odoo database.

View services
-------------

It is recommended to view the list of services in one of several pre-configured ways to better view
the information presented. In the top right corner of the list, there are several icons that when
clicked, sort the data in different ways.

.. image:: service/views.png
   :align: center
   :alt: The icons in the top right corner than cn be clicked to present the information in
         different ways.

List view
~~~~~~~~~

The default view of the services is the list view. This presents all the services in chronological
order, from oldest to newest, in a list.

The information can be sorted by any column. At the top of each column, hover over the column name.
An arrow appears to the right of the name. Click the arrow to sort the data by that specific column.

The default sorting is descending alphabetical order (A to Z). Click the arrow again to reverse the
order, and go in reverse alphabetical order (Z to A). The one exception to this sorting is the
default :guilabel:`Date` column, which sorts the information in chronological order (January to
December) instead of alphabetical order.

Kanban view
~~~~~~~~~~~

To view services by their stage, click on the :guilabel:`Kanban icon`, which is the second icon in
the top right, and appears as four black squares in a cube.

All the services with the same status appear in the corresponding column, from :guilabel:`Running`
to :guilabel:`Cancelled`. To change the status of a service, simply click and drag the service card
to the desired stage.

Graph view
~~~~~~~~~~

Another way to view the data is in a graph. To view the graph, click the :guilabel:`Graph icon`,
which is the third icon in the top right, and appears as a small graph.

The graph displays the information in a graph where the X axis represents the :guilabel:`Date` and
the Y axis represents the :guilabel:`Cost`. Each column represents a single month, and then is
further organized by vehicle. Each vehicle is represented by a different color, and each month's bar
is divided by each vehicle.

Pivot view
~~~~~~~~~~

The final way to view the service data is in a spreadsheet pivot table. Click on the
:guilabel:`Pivot icon`, which is the last icon in the top right, and appears as a small spreadsheet.

The data presented in the table shows the cost of each service or repair. The rows represent the
vendors, and each vehicle that was serviced by them appears beneath each vendor. The column
represent the different service types performed.

The table can be inserted in a spreadsheet or downloaded. To add the pivot table to a spreadsheet in
Odoo, click :guilabel:`Insert In Spreadsheet` and a pop-up appears. Select the spreadsheet the data
should be added to from the drop-down menu, and click :guilabel:`Confirm`. The spreadsheet then
loads on the screen. The spreadsheets are stored in Odoo's *Documents* application. To download the
table in an `xlsx` format, click the :guilabel:`Download` icon.

.. image:: service/pivot.png
   :align: center
   :alt: Download the pivot table to an xlsx file, or insert the data in a spreadsheet in Odoo's
         Documents application.
