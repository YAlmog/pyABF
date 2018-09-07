# The pyABF Project

**The pyABF project simplifies the process of reading data from Axon Binary Format (ABF) files.** It was created with the goal of providing a pythonic API to access the content of ABF files which is so intuitive to use (with a predictive IDE) that documentation is largely unnecessary. Just glance over the code examples and graphs on the [getting started with pyABF](/docs/getting-started) page and you're good to go!

![](/docs/graphics/2017-11-06-aps.png)

### Installation
```bash
pip install --upgrade pyabf
```

### Quickstart
```python
import pyabf
abf = pyabf.ABF("demo.abf")
abf.setSweep(3)
print(abf.sweepY) # displays sweep data (ADC)
print(abf.sweepX) # displays sweep times (seconds)
print(abf.sweepC) # displays command waveform (DAC)
```

## Documenation
* [Getting Started with pyABF](/docs/getting-started)
* [Additional pyABF Documentation](/docs/)
* [Unofficial Guide to the ABF File Format](/docs/advanced/abf-file-format/)
* [pyABF on PyPI](https://pypi.org/project/pyabf/)

## Porting to Other Programming Languages
The pyABF project is not only the location of the pyABF Python module, it serves as a site to aggregate ABF file format and analysis information and strategies. Code is written to be intentionally readable and efforts are taken to write and maintain documentation, making pyABF easy to port to other programming lanaguges. Some efforts to this end have already begin:

* [vsABF](https://github.com/swharden/vsABF) - A .NET library to interface to files in the Axon Binary Format (ABF)
* [phpABF](https://github.com/swharden/phpABF) - A PHP interface to files in the Axon Binary Format (ABF)

## Features
* To see what pyABF can do check out the [getting started](/docs/getting-started) page
* No obscure dependencies (just matplotlib and numpy)
* Actively developed (as of 2018)
* Pythonic API (intended for a predictive IDE)
* Cross-platform, open-source, 100% Python
* Supports 32-bit and 64-bit architectures

![](/docs/graphics/spacer_paired_patch.jpg)
![](/docs/graphics/2017-11-18-multichannel.png)

## Motivation
As a cellular neurophysiologist / electrophysiologist, I have a lot of experience analyzing electrophysiology data with many of the currently-available software options (both free and commercial). None of these options have proven flexible enough for my style of ***exploratory data analysis*** where I pursue scientific discoveries by analyzing data in new and creative ways (necessitating the rapid creation of custom experimental software). I was motivated to create the type of library and documentation I wish I had all along, and will be happy if these efforts chip away at the ABF-reading barrier which separates creative scientists from the ability to analyze their own data. I am a strong proponent of open source software, and hope that the sharing of this project will inspire future scientists and coders as well as promote the collaborative development of software to facilitate scientific discovery and ultimately improve the lives of those who will benefit from medical and scientific advancement.

## Publishing Something Cool?
I'm glad the pyABF project facilitated your research! Consider citing this project by name so it can benefit others too. If your publication was supported by pyABF, let me know about it! I'd love to list it here.

> _"Computational analysis of electrophysiological recordings was performed using custom
> software written for Python 3.7 and the pyABF module."_

## Feature Requests / Unsupported ABF Files
If you have ABF files which are unsupported (or read incorrectly) by this software, chances are it is simply due to a use case I have not run across yet, so I would like to know about it! I can only develop and test this software against ABF files I have access to, so if you're interested in having your ABF file supported send me an email (and the ABF file you are trying to analyze) and I will investigate it. If I come up with a solution I will update the pyabf package so everyone will benefit from the change. I can only develop for (and test against) ABFs I have access to, so I really appreciate your contributions!

**Scott W Harden, DMD, PhD**\
[www.SWHarden.com](http://www.SWHarden.com)\
[SWHarden@gmail.com](mailto:swharden@gmail.com)
