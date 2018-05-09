# Metrics collection, storing, analysing

## graphite/statsd/grafana setup on new Amazon Linux instance
!! Important !!
https://gist.github.com/mmb/81bc2493371f52fdfdeb

I really want to try it in Amazon - plan to do it very soon!

## Monitoring Windows system metrics with Grafana
https://nbsoftsolutions.com/blog/monitoring-windows-system-metrics-with-grafana

Looks like pretty detailed article how to collect Windows-specific metrics.

## C++ StatsD client
https://github.com/vthiery/cpp-statsd-client

I ended up re-implementing it so that it better fits into our system.

## C Implementation of StatsD
https://github.com/statsite/statsite

It claims to be faster. I really didn't experience slowness yet when pushing metrics via StatsD.
Keeping link to this library for future exploration.

## StatsD vs collectd vs fluentd and Other Daemons You Should Know
https://blog.takipi.com/statsd-vs-collectd-vs-fluentd-and-other-daemons-you-should-know/?utm_source=facebook&utm_medium=post&utm_content=daemons&utm_campaign=java


