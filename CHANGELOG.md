1.0.7 (2012-10-04)
==================
- Used for traffic light controllers from 2012.

1.0.8 (2013-09-24)
==================
Extensions for coordination support. Adds commands/statuses needed for
coordination between TLCs

- M0012 Activate/Deactivate many inputs
- M0013 Request many signals groups to green/red

1.0.9 (2013-10-07)
==================
Extensions for coordination support

- M0012 The object type  was incorrectly set to "Signal group". It should have
  been "Traffic controller"

1.0.10 (2013-09-24)
==================
Extensions for coordination support

- M0013 Fix separator between command chunks

1.0.11-1.0.12 (draft)
=====================
Not released. Improved traffic counting. Moved to separate branch
"improved_traffic_counting".

1.0.13 (2017-06-26)
===================
"RSMP++", extensions by the City of Copenhagen.

The SXL additions was initiated by the City of Copenhagen to enable more
flexible traffic management using the RSMP protocol.

The extension focuses on these elements:

- Ability to read list of configured time plans
- Ability to read and modify offset times
- Ability to read and modify green times
- Ability to read and modify time tables
- Ability to read and modify cycle time
- Ability to get predicted time-to-green / time-to-red
- Ability to force input

1.0.14 (2017-10-30)
===================
Improved traffic counting (S0205-S0208)

The old traffic data statuses, S0201-S0204, may cause excessive amount of
network traffic if subscriptions are established for each detector logic. The
new traffic data statuses contains data from all detector logics in the same
status message.
