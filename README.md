# exchars

## Purpose
I got tired of downloading the whole PwnTools suite when I only use the cyclic functionality. This is meant to just generate random chars, find the position of the chars, and also generate bad char blobs for exploitation purposes.

## Requirements

### Python 3.6+

## Installation

   > python -m pip install .\exchars\

    Processing c:\...\exchars
    Installing build dependencies ... done
    Getting requirements to build wheel ... done
    Preparing metadata (pyproject.toml) ... done
    Building wheels for collected packages: exchars
    Building wheel for exchars (pyproject.toml) ... done
    Created wheel for exchars: filename=exchars-1.0-py3-none-any.whl size=3136 sha256=81ba75fb5c29fa2d823fd4ae93acdd88cb9b0a082b13c71cbdb7ea9a0d357c8e
    Stored in directory: C:\...\AppData\Local\Temp\pip-ephem-wheel-cache-p3h3_j04\wheels\b8\3e\f5\8824831b7c506c206c3d51ea16356c9ca585b4665db17bdcda
    Successfully built exchars
    Installing collected packages: exchars
    Attempting uninstall: exchars
        Found existing installation: exchars 0.1
        Uninstalling exchars-0.1:
        Successfully uninstalled exchars-0.1
    Successfully installed exchars-1.0

## Usage

    >>> from exchars import Chars
    >>> chars = Chars()
    >>> chars.cyclic(100)
    'Aa0Aa1Aa2Aa3Aa4Aa5Aa6Aa7Aa8Aa9Ab0Ab1Ab2Ab3Ab4Ab5Ab6Ab7Ab8Ab9Ac0Ac1Ac2Ac3Ac4Ac5Ac6Ac7Ac8Ac9Ad0Ad1Ad2A'
    >>> chars.find('Ab8Ab9Ac0A')
    54
