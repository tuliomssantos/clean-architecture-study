#   SRP Violation Example

![figure10](/images/figure10.png)

This class violates the SRP because those three methods are responsible to three very different actors.

*   The calculatePay() method is specified by the accounting department, which reports to the CFO.
*   The reportHours() method is specified and used by the human resources department, which reports to the COO.
*   The save() method is specified by the database administrators (DBAs), who report to the CTO.

By putting the source code for these three methods into a single Employee class, the developers have coupled each of these actors to the others. This coupling can cause the actions of the CFO’s team to affect something that the COO’s team depends on.


