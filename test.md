## Better than VMs

A common method for distributing applications and sandbox their
execution is to use virtual machines, or VMs. Typical VM formats are
VMWare's vmdk, Oracle Virtualbox's vdi, and Amazon EC2's ami. In
theory these formats should allow every developer to automatically
package their application into a "machine" for easy distribution and
deployment. In practice, that almost never happens, for a few reasons:

  * *Size*: VMs are very large which makes them impractical to store
     and transfer.
  * *Performance*: running VMs consumes significant CPU and memory,
    which makes them impractical in many scenarios, for example local
    development of multi-tier applications, and large-scale deployment
    of cpu and memory-intensive applications on large numbers of
    machines.
  * *Portability*: competing VM environments don't play well with each
     other. Although conversion tools do exist, they are limited and
     add even more overhead.
  * *Hardware-centric*: VMs were designed with machine operators in
    mind, not software developers. As a result, they offer very
    limited tooling for what developers need most: building, testing
    and running their software. For example, VMs offer no facilities
    for application versioning, monitoring, configuration, logging or
    service discovery.
