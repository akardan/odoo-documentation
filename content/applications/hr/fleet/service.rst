========
Services
========

To properly maintain a fleet of vehicles, regular maintenance as well as periodic repairs are
needed. Scheduling repairs and managing servicing for an entire fleet is necessary to ensure
all vehicles are in good working order for when they are needed.

Easily viewing and understanding repair costs is critical to know exactly how much a vehicle costs
to stay in good working order and be part of a fleet. Odoo's *Fleet* application allows for easy
management of repairs and services, and provides visibility to a critical component of fleet
management.

List of services
================

To view all services logged in the database, including old and new requests, go to
:menuselection:`Fleet application --> Fleet --> Services`. All services appear in a list view,
including all the details for each service.

Each service listed displays the following information:

- :guilabel:`Date`: The date service or repair was performed or is requested to be performed.
- :guilabel:`Description`: A short description of the specific type of service or repair performed
  to clarify the specific service.
- :guilabel:`Service Type`: The service or repair performed. This is selected form a list of
  services that must be configured.
- :guilabel:`Vehicle`: The specific vehicle the service was performed on.
- :guilabel:`Driver`: Who the current driver is for the vehicle.
- :guilabel:`Vendor`: The specific vendor who performed the service or repair.
- :guilabel:`Cost`: The total cost for the service or repair.
- :guilabel:`Notes`: Any information associated with the service or repair that is documented to add
  clarification.
- :guilabel:`Status`: The status of the service or repair. Options are :guilabel:`New`,
  :guilabel:`Running`, :guilabel:`Canceled`, or :guilabel:`Done`.

Sort services
-------------

It is recommended to sort or group the list of services to better view the information presented.

Sort by column
~~~~~~~~~~~~~~

One way to sort the list is by a specific column of information. At the top of each column, hover
next to the column name. An arrow will appear to the right of the name. Click the arrow to sort the
data by that specific column.

The default sorting is descending alphabetical order (A to Z). Click the arrow again to reverse the
order, and go in reverse alphabetical order (Z to A).

The one exception to this sorting is the :guilabel:`Date` column, which sorts the information in
chronological order (January to December) instead of alphabetical order. Click the arrow again to
reverse the order (December to January).

Sort by grouping
~~~~~~~~~~~~~~~~

Another common organization method is to group the data by a value. To organize by grouping, go to
on :menuselection:`Group By --> Add Custom Group` and then select the value to group by from the
drop-down list. Once the value has been selected, click :guilabel:`Apply`. The data vill be grouped
by the value seleced.

Two common values to group services by are :guilabel:`Stage` and :guilabel:`Vehicle`. Grouping the
services by stage will organize the list and present all the services with the same status together,
from :guilabel:`Running` to :guilabel:`Cancelled`. Grouping by vehicle will organize all the
services by the specific vehicle. This allows more visibility on the service for each specific
vehicle, and shows the total repair cost by vehicle, as well as the breakdown of the individual
repairs and services.

Create a service record
=======================

To log a service,