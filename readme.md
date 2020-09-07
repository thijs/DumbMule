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