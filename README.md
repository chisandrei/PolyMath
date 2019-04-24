# PolyMath

[![Project Status: Active – The project has reached a stable, usable state and is being actively developed.](http://www.repostatus.org/badges/latest/active.svg)](http://www.repostatus.org/#active)
[![Build Status](https://travis-ci.org/PolyMathOrg/PolyMath.svg?branch=master)](https://travis-ci.org/PolyMathOrg/PolyMath)
[![Build status](https://ci.appveyor.com/api/projects/status/3tvarh2xi22max8h?svg=true)](https://ci.appveyor.com/project/SergeStinckwich/polymath-88bea)
[![License](https://img.shields.io/badge/license-MIT-blue.svg)](https://raw.githubusercontent.com/PolyMathOrg/PolyMath/master/LICENSE)

<img width="1675" alt="Screenshot 2019-04-24 at 11 12 57" src="https://user-images.githubusercontent.com/327334/56652094-66eb7780-6682-11e9-9753-101be18df67c.png">

You can load the code in a fresh Pharo 7.0 image with:

```Smalltalk
Metacello new
        repository: 'github://PolyMathOrg/PolyMath:development/src';
        baseline: 'PolyMath';
        load
```

We have **797** green tests !
 
PolyMath is a Pharo project, similar to existing scientific libraries like NumPy, SciPy for Python or SciRuby for Ruby. PolyMath already provide the following basic functionalities:
- complex and quaternions extensions,
- random number generators,
- fuzzy algorithms,
- KDE-trees,
- Didier Besset's numerical methods,
- Ordinary Differential Equation (ODE) solvers.

A book about PolyMath called "Numerical Methods" is available online: https://github.com/SquareBracketAssociates/NumericalMethods/releases/tag/snapshot-2016-01-17

Some documentation (to be cleaned and reorganized) about PolyMath is available on the Wiki here: 
https://github.com/PolyMathOrg/PolyMath/wiki

Natalia wrote some explanation about benchmarking PolyMath in the Pharo For Enterprise Book: https://github.com/SquareBracketAssociates/PharoForTheEnterprise-english/blob/ae40e7ab6f7651f6e7c271869eb1efc4e531e774/ComparingSolutions/ComparingSolutions.pier

## Install PolyMath

To install PolyMath on your Pharo image you can just execute the following script:

```Smalltalk
    Metacello new
        githubUser: 'PolyMathOrg' project: 'PolyMath' commitish: 'master' path: 'src';
        baseline: 'PolyMath';
        load
```

To add PolyMath to your baseline just add this:

```Smalltalk
    spec
    	baseline: 'PolyMath'
    	with: [ spec repository: 'github://PolyMathOrg/PolyMath:master/src' ]
```

Note that you can replace the #master by another branch as #development or a tag as #v1.0.0, #v1.? or #v1.2.? .


## How to contribute to PolyMath

We welcome submissions! A google group exists for this project at http://groups.google.com/group/polymath-project
