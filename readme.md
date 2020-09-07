# SimpleMule; an X4 Foundations MOD

### Based on [Mules-and-Warehouses-Extended](https://github.com/Misunderstood-Wookiee/Mules-and-Warehouses-Extended)

I use Mules-and-Warehouses-Extended (MWEx) in my own games. However, I
found the setup for DistribMules and SupplyMules for a warehouse too
complex and prone to errors. I had issues, for example, with Mules
bringing wares from one station and then bringing it back again
because two-way trade was enabled.

This MOD started out in the simplest form: bring products (the stuff
the station produces) from one station to another.

Later I added support for two-way trade and selecting your own list of
wares to transport.

## Setup

Setup is fairly simple. Select SimpleMule as your Mule type from the
**default behaviour menu**.

* **Select your source station**
* **Select your target station**

These two are mandatory (source and target station), the rest is
optional.

By default the SimpleMule should work for **products** to be moved
from source to station, and **resources** that the source needs and
that are available at the target will be moved back, as **two-way
trade** is on by default.

The other opions are:

* **Add / Remove Wares (products by default)**

This option enables you to manually select wares that you want moved
from source to target. If **Only Selected Wares** is enabled, only
wares on this list will be moved from source to target, otherwise they
are added to the list of products produced at the station.

* **Add / Remove Wares for return run**

This does the same as above, but for the wares to move from target
back to source. This list is added (unless **Only Selected Wares** is
enabled) to the list of resources the source wants and are available
at the target.

* **Only Selected Wares**

See above.

* **Two-way trade**

If enabled, the SimpleMule will also move stuff back from the target
to the source. See above also.

* **Allow Energy Cells**

By default Energy Cells are excluded from being moved.

* **Allow Food and Meds**

By default Food and Meds are excluded from being moved.

* **Fill Cargo Percentage**

The percentage of the cargo hold where the SimpleMule stops looking
for more trades. The SimpleMule will try to find more trades to load
if the cargo fill percentage is lower than this setting, but it
doesn't stop the cargo run. So this is the preferred minimum cargo
fill percentage.

* **Keep Resource at Target**

If a ware is also a resource at the target station, this setting will
keep x times the hourly consumption of that ware at the target
station. The example I run into most is stations that produce Food and
have a habitat. The habitat needs food, so it's both a resource and a
product for that station. With this setting set to 1, the SimpleMule
will always leave 1 hour's worth of Food at the target station. At 2,
2 hour's worth. Etc.
