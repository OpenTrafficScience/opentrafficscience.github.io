---
layout: default
---

<script src="https://polyfill.io/v3/polyfill.min.js?features=es6"></script>
<script id="MathJax-script" async src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-mml-chtml.js"></script>

<script>
window.MathJax = {
    chtml: {
        scale: 0.95,
        minScale: 0.9
    },
    svg: {
        scale: 0.95,
        minScale: 0.9
    },
    tex: {
        inlineMath: [['$', '$'], ['\\(', '\\)']],
        displayMath: [['$$', '$$'], ['\\[', '\\]']]
    }
};
</script>

## Knowledge Repository

Built on the foundation of [Xinyu Chen (陈新宇)](https://xinychen.github.io/)'s [Knowledge Repository](https://spatiotemporal-data.github.io/bib/) and guided by his kind mentorship, [Junyi Ji](https://www.jijunyi.com/) developed this repository since early 2026 to document methodology and technology developments that bridge traffic systems with dynamical systems, control theory, and optimization methods. 

### 1st Commit
#### Signal Coordination

Signal coordination is the way to synchronize traffic signals along a corridor (main road) to create a "green wave" that allows vehicles to pass through multiple intersections without stopping. To better understand the dynamics of this system, and partly inspired by this [post](https://www.flickr.com/photos/walkingsf/5800930374), I build a web-based simulator tool called [Signal Puzzle](https://www.opentraffic.science/signal-puzzle) that simulates the dynamics of traffic [near Vanderbilt University](https://maps.app.goo.gl/3pP5rb7BngcB8nkW7). By changing the signal lengths, green split, offset, and the demand (arrival rate and the headway distribution), we can see how the time-space diagrams change.

My observations:
- The red lights act like a "transformer," converting the arrival pattern into a different departure pattern.
- The bidirectional nature of the traffic flow makes the problem more complex, as the signal coordination needs to consider both directions of traffic.

**References**
- [Koonce, P. (2008). Traffic signal timing manual (No. FHWA-HOP-08-024). United States. Federal Highway Administration.](https://rosap.ntl.bts.gov/view/dot/800/dot_800_DS1.pdf)
- [Fischer, E. (2011). Traffic signal timing patterns on Oakland's Broadway [Photograph]. Flickr.](https://www.flickr.com/photos/walkingsf/5800930374/)