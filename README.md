# EulerBallistic
LGPL library for small arms ballistic calculations based on point-mass (3 DoF) plus spin drift.
The fork of py_ballisticcalc.exts that can be used as side-package

### Table of contents
* **[Installation](#installation)**
  * [Latest stable](#latest-stable-release-from-pypi)

* **[Usage](#usage)**

* **[Contributors](#contributors)**
* **[About project](#about-project)**

# Installation

```shell
pip install EulerBallistic
```

# Usage
**See [Original README](Example.ipynb) for detailed illustrations of all features and usage.**


# About project

The library provides trajectory calculation for ballistic projectiles including air rifles, bows, firearms, artillery, and so on.

The 3DoF model that is used in this calculator is rooted in public C code of [JBM's calculator](https://jbmballistics.com/ballistics/calculators/calculators.shtml), ported to C#, optimized, fixed and extended with elements described in Litz's _Applied Ballistics_ book and from the friendly project of Alexandre Trofimov and then ported to Go.

This Python3 implementation has been expanded to support multiple ballistic coefficients and custom drag functions, such as those derived from Doppler radar data.

**[The online version of Go documentation is located here](https://godoc.org/github.com/gehtsoft-usa/go_ballisticcalc)**.

**[C# version of the package is located here](https://github.com/gehtsoft-usa/BallisticCalculator1), and [the online version of C# API documentation is located here](https://gehtsoft-usa.github.io/BallisticCalculator/web-content.html)**.

## Contributors
**This project exists thanks to all the people who contribute.**

<a href="https://github.com/o-murphy/py_ballisticcalc/graphs/contributors"><img height=32 src="https://contrib.rocks/image?repo=o-murphy/py_ballisticcalc" /></a>

Special thanks to:
- **[David Bookstaber](https://github.com/dbookstaber)** - Ballistics Expert\
*For help understanding and improving the functionality*
- **[Nikolay Gekht](https://github.com/nikolaygekht)** \
*For the sources code on C# and GO-lang from which this project firstly was forked*

[//]: # (## Sister projects)

[//]: # ()
[//]: # (* **Py-BalCalc** - GUI App for [py_ballisticcalc]&#40;https://github.com/o-murphy/py_ballisticcalc&#41; solver library and profiles editor)

[//]: # (* **eBallistica** - Kivy based mobile App for ballistic calculations)

[//]: # ()
[//]: # (* <img align="center" height=32 src="https://github.com/JAremko/ArcherBC2/blob/main/resources/skins/sol-dark/icons/icon-frame.png?raw=true" /> [ArcherBC2]&#40;https://github.com/JAremko/ArcherBC2&#41; and [ArcherBC2 mobile]&#40;https://github.com/ApodemusSylvaticus/archerBC2_mobile&#41; - Ballistic profile editors)

[//]: # (  - *See also [a7p_transfer_example]&#40;https://github.com/JAremko/a7p_transfer_example&#41; or [a7p]&#40;https://github.com/o-murphy/a7p&#41; repo to get info about the ballistic profile format*)

## RISK NOTICE

The library performs very limited simulation of a complex physical process and so it performs a lot of approximations. Therefore, the calculation results MUST NOT be considered as completely and reliably reflecting actual behavior or characteristics of projectiles. While these results may be used for educational purpose, they must NOT be considered as reliable for the areas where incorrect calculation may cause making a wrong decision, financial harm, or can put a human life at risk.

THE CODE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE MATERIALS OR THE USE OR OTHER DEALINGS IN THE MATERIALS.
