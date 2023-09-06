============
New vehicles
============

Odoo Fleet manages all vehicles and the accompanying documentation that comes with vehicle
maintenance and driver's records.

All vehicles are organized on the main :guilabel:`Fleet` dashboard. Each vehicle has its own
*vehicle form*, which is displayed as a card in the kanban view. Every vehicle form is displayed in
its current corresponding kanban stage.

To add a new vehicle to the fleet, click the :guilabel:`Create` button, and a blank vehicle form
will load. Enter the vehicle information in the vehicle form, then click :guilabel:`Save`.

Vehicle form fields
===================

- :guilabel:`Model`: Select the vehicle's model from the drop-down menu. If the model is not listed,
  type in the model name and click either :guilabel:`Create` or :guilabel:`Create and Edit`.
- :guilabel:`License Plate`: Enter the vehicle's license plate number in this field.
- :guilabel:`Tags`: Select any tags from the drop-down menu, or type in a new tag. There is no limit
  on the amount of tags that can be selected.

.. note::
   The :guilabel:`Model` is the only required field on the new vehicle form. When a model is
   selected, other fields will appear on the vehicle form. If some of the fields do not appear, this
   may indicate there is no model selected.

Driver
------

- :guilabel:`Driver`: Select the driver from the drop-down menu, or type in a new driver and click
  either :guilabel:`Create` or :guilabel:`Create and Edit`.
- :guilabel:`Mobility Card`: If the selected driver has a mobility card listed on their employee
  card in the *Employees* application, the mobility card number will appear in this field. If there
  is no mobility card listed and one should be added, :doc:`edit the employee card
  </applications/hr/employees/new_employee>` in the *Employees* application.
- :guilabel:`Future Driver`: If the next driver for the vehicle is known, select the next driver
  from the drop-down menu, or type in the next driver and click either :guilabel:`Create` or
  :guilabel:`Create and Edit`.
- :guilabel:`Plan To Change Car`: If the current driver set for this vehicle plans to change their
  vehicle, either because they are waiting on a new vehicle that is being ordered, or this is a
  temporary vehicle assignment and they know which vehicle they will be driving next, check this
  box. If the current driver does not plan to change their vehicle and use this current vehicle, do
  not check this box.
- :guilabel:`Assignment Date`: Select the date the vehicle will be available for another driver
  using the drop-down calendar module. If this field is blank, this indicates the vehicle is
  currently available and can be reassigned to another driver. If it is populated, the vehicle will
  not be available to assign to another driver until the date entered.

.. important::
   A driver does *not* have to be an employee, but a driver must be listed in the *Contacts*
   application. When creating a new driver, the driver is added to the *Contacts* application, not
   the *Employees* application.

Vehicle
-------

- :guilabel:`Immatriculation Date`: Select the date the vehicle is acquired using the drop-down
  calendar module.
- :guilabel:`Cancellation Date`: Select the date the vehicle lease will expire, or when the vehicle
  will be no longer available, using the drop-down calendar module.
- :guilabel:`Chasis Number`: Enter the chasis number in the field. This is known in some countries
  as the :abbr:`VIN (Vehicle Identification Number)` number.
- :guilabel:`Last Odometer`: Enter the last known odometer reading in the number field. Using the
  drop-down menu next to the number field, select whether the odometer reading is in kilometers
  :guilabel:`(km)` or miles :guilabel:`(mi)`.
- :guilabel:`Fleet Manager`: Select the fleet manager from the drop-down menu, or type in a new
  fleet manager and click either :guilabel:`Create` or :guilabel:`Create and Edit`.
- :guilabel:`Location`: Type in the location for the vehicle in the field. The most common scenario
  for when this field would be populated is if a company has several office locations. The typical
  office location where the vehicle is located would be the location entered.
- :guilabel:`Company`: Select the company that the vehicle will be used for and associated with from
  the drop-down menu, or type in a new company and click either :guilabel:`Create` or
  :guilabel:`Create and Edit`.

.. image:: new_vehicle/new-vehicle-type.png
   :align: center
   :alt: The new vehicle form, showing the vehicle tax section.

Tax Info tab
------------

Fiscality
~~~~~~~~~

- :guilabel:`Horsepower Taxation`: Enter the amount that is taxed based on the size of the vehicles
  engine. This is determined by local taxes and regulations, and varies depending on the location.
  It is recommended to check with the accounting department to ensure this value is correct.
- :guilabel:`Disallowed Expense Rate`: Enter the amount of non-deductible expenses for the vehicle.
  This amount is not counted towards any deductions on a tax return or as an allowable expense
  when calculating taxable income. It is recommended to check with the accounting department to
  ensure this value is correct.
- :guilabel:`Start Date`: Enter the date these two values will affect the taxes, using the
  drop-down calendar module.

Contract
~~~~~~~~

- :guilabel:`First Contract Date`: Select the start date for the vehicle's first contract using
  the drop-down calendar module. Typically this is the day the vehicle is purchased or leased.
- :guilabel:`Catalog Value (VAT Incl.)`: Enter the MSRP (Manufacturer's Suggested Retail Price) for
  the vehicle at the time of purchase or lease.
- :guilabel:`Purchase Value`: Enter the purchase price or the value of the lease for the vehicle.
- :guilabel:`Residual Value`: Enter the current value of the vehicle.

.. image:: new_vehicle/new-vehicle-tax.png
   :align: center
   :alt: The new vehicle form, showing the vehicle tax section.

Model tab
---------

Model
~~~~~

- :guilabel:`Model Year`: Enter the year the vehicle was manufactured.
- :guilabel:`Transmission`: Select the transmission type from the drop-down menu, either
  :guilabel:`Manual` or :guilabel:`Automatic`.
- :guilabel:`Color`: Enter the color of the vehicle.
- :guilabel:`Seats Number`: Enter how many passengers the vehicle can accommodate.
- :guilabel:`Doors Number`: Enter the number of doors the vehicle has.
- :guilabel:`Trailer Hitch`: Check this box if the vehicle has a trailer hitch.

Engine
~~~~~~

- :guilabel:`Horsepower`: Enter the vehicle's horsepower in this field.
- :guilabel:`Power`: If the vehicle is electric or hybrid, enter the power the vehicle uses in
  kilowatts (kW).
- :guilabel:`Fuel Type`: Select the type of fuel the vehicle uses form the drop-down menu. The
  options are :guilabel:`Diesel`, :guilabel:`Gasoline`, :guilabel:`Hybrid Diesel`, :guilabel:`Hybrid
  Gasoline`, :guilabel:`Plug-in Hybrid Diesel`, :guilabel:`Plug-in Hybrid Gasoline`,
  :guilabel:`CNG`, :guilabel:`LPG`, :guilabel:`Hydrogen`, or :guilabel:`Electric`.
- :guilabel:`CO2 Emissions`: Enter the carbon dioxide emissions the vehicle produces in grams per
  kilometer (g/km).
- :guilabel:`Co2 Standard`: Enter the standard amount of carbon dioxide for a similar sized vehicle.

.. image:: new_vehicle/new-vehicle-model.png
   :align: center
   :alt: The new vehicle form, showing the vehicle tax section.

Note tab
--------

Enter any notes for the vehicle in this section.
