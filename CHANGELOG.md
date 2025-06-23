# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## Summary of cpbd-py312 Fork

This fork (`cpbd-py312`) was created on 2025-06-23 to provide Python 3.12+ compatibility for the original `cpbd` package. The main changes include:

1. **Version 1.0.0**: Initial fork with Python 3.12 support, modernized dependencies, and removal of Python 2 code
2. **Version 1.0.1**: Updated documentation and restricted to Python 3.12+ only
3. **Version 1.0.2**: Fixed PyPI description display issue and updated author information
4. **Version 1.0.3**: Relaxed Python requirement to >=3.8 to allow broader compatibility

The package is now available on PyPI as `cpbd-py312` and can be installed with `pip install cpbd-py312`.

## [1.0.3] - 2025-06-23 - cpbd-py312

### Changed
- Changed minimum Python requirement from >=3.12 to >=3.8 (allowing Python 3.8+)
- This allows users with Python 3.8, 3.9, 3.10, and 3.11 to install the package
- Note: While the package allows Python 3.8+, it has been specifically tested with Python 3.12

## [1.0.2] - 2025-06-23 - cpbd-py312

### Fixed
- Fixed PyPI description by using README.md instead of README.rst
- Updated author information to nawta

## [1.0.1] - 2025-06-23 - cpbd-py312

### Changed
- Updated project description and documentation to reflect fork status
- Initially limited Python version support to 3.12+ only (removed untested 3.8-3.11)
- Updated homepage URL to https://github.com/nawta/python-cpbd-py312
- Updated PyPI package description to clarify this is a Python 3.12+ compatible fork

## [1.0.0] - 2025-06-23 - cpbd-py312

### Added
- Forked as `cpbd-py312` for Python 3.12+ compatibility
- Initial fork created specifically for Python 3.12 support
- `pyproject.toml` for modern Python packaging (PEP 517/518)
- `imageio` dependency for image reading (replacing deprecated scipy.ndimage)
- Command line interface improvements
- Comprehensive README.md documentation
- CHANGELOG.md to track version history

### Changed
- Package name changed from `cpbd` to `cpbd-py312` to indicate Python 3.12+ compatibility
- Replaced deprecated `scipy.ndimage.imread` with `imageio.v2.imread`
- Updated minimum dependency versions:
  - matplotlib >= 3.5.0 (was >= 2.0.0)
  - numpy >= 1.21.0 (was >= 1.11.1)
  - scikit-image >= 0.19.0 (was >= 0.12.3)
  - scipy >= 1.7.0 (was >= 0.18.1)
  - imageio >= 2.9.0 (new dependency)
- Modernized packaging configuration
- Updated code to use Python 3 syntax exclusively

### Removed
- Python 2.7, 3.5, and 3.6 support
- `__future__` imports and Python 2 compatibility code
- Legacy Python 2/3 compatibility shims
- Deprecated scipy.ndimage.imread usage

### Fixed
- Compatibility issues with Python 3.12
- Deprecated API warnings from scipy
- Import errors with modern Python versions

## [1.0.7] - Previous Release

### Notes
- Last version supporting Python 2.7
- Original implementation details preserved