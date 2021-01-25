# Beta-Lambda Network Graphs

Beta-Lambda Network Graphs β-λ are used to show the individual 
latency (λ) & total latency (Λ) vs. the bandwidth for the hops 
of a network path.  

The lowest bandwidth limits (sets) the overall path bandwidth (Β or BW).

In a beta-lambda graph, the vertical axis indicates bandwidth; 
typically on a log10 scale.  When colors are available, the bandwidth is
redundantly indicated by standard colors, below.  These colors should also
be used in network topology diagrams, where the lines (edges) use the same
colors.  A line thickness may also be applied to indicate bandwidth.
Standard colors:

    navy   - 100Tbps+ (not part of resistor colors but the future is close!)
    teal   - 10Tbps   (not part of the resistor colors, but networks are fast 
                         enough that we need this now)
    white  - 1Tbps    (use light cyan/"electric blue" if white doesn't show)
    slate  - 100Gbps
    indigo - 40Gbps   (not part of the resistor colors but a common link 
                         speed so an intermediate color is used speeds)
    violet - 10Gbps
    blue   - 1Gbps
    green  - 100Mbps
    yellow - 10Mbps   (on light backgrounds, use dirty yellow since bright 
                        yellow doesn't show well)
    orange - 1Mbps
    red    - 100kbps
    brown  - 10kps
    black  - 1kbps or unspecified

Yep... the colors come from the Resistor Color Code.  It's the multiplier 
value in kbps (thus gold, silver, & pink can be used to get down to 1 bps)

Each horizontal segment is a network "hop"; the chain of hops is a "path".
The length of each link indicates its latency.  Where large latency variations 
exist; use a log scale.

Vertical(-ish) transitions in the diagram are network switches, hubs, and 
the like.  If not quite vertical then the horizontal component indicates the 
switch-fabric latency.


### Origins
I invented the beta-lambda graph as a way to visualize network paths
for quick comparisons of multiple paths, when working on a high-resiliency
multi-path network protocol in 2020.

