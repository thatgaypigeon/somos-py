# Home

<a name=""><img height="36px" src="https://forthebadge.com/images/featured/featured-built-with-love.svg" align="right" alt="Built With 🧡" /></a>

**`somos-py`** is a [Somos sequence](https://en.wikipedia.org/wiki/Somos_sequence) generator for <sub><img height="17px" src="https://api.iconify.design/skill-icons:python-dark.svg" alt="" hspace="2px" /></sub>Python.

If you don't know about **Somos sequences**, they are a series of [mathematical sequences](https://en.wikipedia.org/wiki/Sequence) generated by a [recurrence equation](https://en.wikipedia.org/wiki/Recurrence_relation). Like the well-known [Fibonacci sequence](https://en.wikipedia.org/wiki/Fibonacci_sequence), the next term is defined by some previous terms. You can read [**below**](#somos-sequences) for more information.

<a name=""><img height="22px" src="https://img.shields.io/github/v/release/thatgaypigeon/somos-py?style=for-the-badge&label=Version" /></a><a href="https://github.com/thatgaypigeon/somos-py/releases/" ><sup><sub><img height="17px" src="https://api.iconify.design/octicon:link-external-16.svg?color=%23ffa724" alt="↗" hspace="6px" /><sup></sub></a>

Check out the [**latest version**](https://github.com/thatgaypigeon/somos-py/release)!

<!-- ---
<p> -->

<a name=""><img height="22px" src="https://img.shields.io/readthedocs/somos?style=for-the-badge&label=Docs" /></a><a href="https://github.com/thatgaypigeon/somos-py/releases/" ><sup><sub><img height="17px" src="https://api.iconify.design/octicon:link-external-16.svg?color=%23ffa724" alt="↗" hspace="6px" /><sup></sub></a>

You can find documentation on my site [**`pigeon.uk.to/somos-py`**](https://pigeon.uk.to/somos-py) or over at [`somos.readthedocs.io`](https://somos.readthedocs.io)!

## Somos sequences <a href="#top"><img align="right" height="24px" src="https://api.iconify.design/octicon:move-to-top-16.svg?color=%23ffa724" /></a>
> *For more information, see [Wikipedia → Somos sequence](https://en.wikipedia.org/wiki/Somos_sequence).*

**Somos sequences** are a series of mathematical sequences generated by a recurrence equation, like the Fibonacci numbers.

They were first described by Michael Somos in September 1989 as [Problem 1470](https://cms.math.ca/wp-content/uploads/crux-pdfs/Crux_v15n07_Sep.pdf#page=19) in [*Crux Mathematicorum* Volume 15, Issue 7](https://cms.math.ca/wp-content/uploads/crux-pdfs/Crux_v15n07_Sep.pdf) and then later in his paper "[Step into the Elliptic Realm](https://www.cut-the-knot.org/arithmetic/algebra/EllipticSeq.shtml)" in January 2000.

### Definition <a href="#top"><img align="right" height="20px" src="https://api.iconify.design/octicon:move-to-top-16.svg?color=%23ffa724" /></a>
For an integer $k$ larger than 1, the Somos-$k$ sequence is defined by the equation:

$$a_{n}a_{{n-k}}=a_{{n-1}}a_{{n-k+1}}+a_{{n-2}}a_{{n-k+2}}+\cdots +a_{{n-(k-1)/2}}a_{{n-(k+1)/2}}$$

when $k$ is odd; or

$$a_{n}a_{{n-k}}=a_{{n-1}}a_{{n-k+1}}+a_{{n-2}}a_{{n-k+2}}+\cdots +(a_{{n-k/2}})^{2}$$

when $k$ is even, with the initial values $a_{i}=1$ for $i < k$.

### Sequence values <a href="#top"><img align="right" height="20px" src="https://api.iconify.design/octicon:move-to-top-16.svg?color=%23ffa724" /></a>
For $k = 2$ or $3$, the generated sequence is all $1$s.

For $k > 3$, the first $k$ terms are all $1$s.

For $k < 7$, all terms are integers. For $k > 8$, terms will eventually become [fractions](https://en.wikipedia.org/wiki/Fraction). The terms at which Somos-$k$ becomes non-integral are (starting at Somos-$8$): 17, 19, 20, 22, 24, 27, 28, 30, 33, 34, 36, 39, ... (sequence [A030127](https://oeis.org/A030127) in the OEIS).

Below are the first 20 terms of Somos sequences 4 to 10.

<dl>
<dt><b>Somos-4</b> (<a href="https://oeis.org/A006720">A006720</a>)</dt>
<dd>1, 1, 1, 1, 2, 3, 7, 23, 59, 314, 1529, 8209, 83313, 620297, 7869898, 126742987, 1687054711, 47301104551, 1123424582771, 32606721084786, ...</dd>

<dt><b>Somos-5</b> (<a href="https://oeis.org/A006721">A006721</a>)</dt>
<dd>1, 1, 1, 1, 1, 2, 3, 5, 11, 37, 83, 274, 1217, 6161, 22833, 165713, 1249441, 9434290, 68570323, 1013908933, ...</dd>

<dt><b>Somos-6</b> (<a href="https://oeis.org/A006722">A006722</a>)</dt>
<dd>1, 1, 1, 1, 1, 1, 3, 5, 9, 23, 75, 421, 1103, 5047, 41783, 281527, 2534423, 14161887, 232663909, 3988834875, ...</dd>

<dt><b>Somos-7</b> (<a href="https://oeis.org/A006723">A006723</a>)</dt>
<dd>1, 1, 1, 1, 1, 1, 1, 3, 5, 9, 17, 41, 137, 769, 1925, 7203, 34081, 227321, 1737001, 14736001, ...</dd>

<dt><b>Somos-8</b></dt>
<dd>1, 1, 1, 1, 1, 1, 1, 1, 4, 7, 13, 25, 61, 187, 775, 5827, 14815, 420514/7, 28670773/91, 6905822101/2275, ...</dd>

<dt><b>Somos-9</b></dt>
<dd>1, 1, 1, 1, 1, 1, 1, 1, 1, 4, 7, 13, 25, 49, 115, 355, 1483, 11137, 27937, 755098/7, ...</dd>

<dt><b>Somos-10</b></dt>
<dd>1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 5, 9, 17, 33, 65, 149, 413, 1473, 7073, 64785, ...</dd>
</dl>

### In popular culture <a href="#top"><img align="right" height="20px" src="https://api.iconify.design/octicon:move-to-top-16.svg?color=%23ffa724" /></a>
**Somos sequences** were discussed by [Dr Harini Desiraju](https://www.sydney.edu.au/science/about/our-people/academic-staff/harini-desiraju.html), a fellow at the University of Sydney, in a [Numberphile](https://www.youtube.com/@numberphile) video from May 2022.

<center>
<a href="https://www.youtube.com/watch?v=p-HN_ICaCyM" title="The Troublemaker Number - Numberphile on YouTube">
<img src="https://img.youtube.com/vi/p-HN_ICaCyM/0.jpg" alt="The Troublemaker Number - Numberphile" href="https://www.youtube.com/watch?v=p-HN_ICaCyM" />
</a>

<a href="https://www.youtube.com/watch?v=p-HN_ICaCyM">The Troublemaker Number - Numberphile</a> on YouTube
</center>

## Uses <a href="#top"><img align="right" height="24px" src="https://api.iconify.design/octicon:move-to-top-16.svg?color=%23ffa724" /></a>
None, really. This is just a small implementation of a bit of number theory. It's purely recreational. :)

If you *do* happen to find a use for this, please let me know!

## External links <a href="#top"><img align="right" height="20px" src="https://api.iconify.design/octicon:move-to-top-16.svg?color=%23ffa724" /></a>
* [*Crux Mathematicorum* Volume 15, Issue 7](https://cms.math.ca/wp-content/uploads/crux-pdfs/Crux_v15n07_Sep.pdf#page=19) at [cms.math.ca](https://cms.math.ca)
* [Somos sequence](https://en.wikipedia.org/wiki/Somos_sequence) at Wikipedia
* [Somos sequences](https://mathworld.wolfram.com/SomosSequence.html) at MathWorld
* [The Somos Sequence Site](https://faculty.uml.edu//jpropp/somos.html) at [uml.edu](https://uml.edu), by *James Propp*
* [The Troublemaker Number - Numberphile](https://www.youtube.com/watch?v=p-HN_ICaCyM) on YouTube
