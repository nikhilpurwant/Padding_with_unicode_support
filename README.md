# Padding_with_unicode_support - Unicode support for Pipy Package "Padding"


> Note - The original author of [this package](https://pypi.org/project/Padding) is [Peio Popov](peio@peio.org) - I have added unicode support to it with a small change.


[Padding](https://pypi.org/project/Padding) is a popular Python package that facilitates developers apply standardized padding while performing cryptographic opeations.

You can find the complete documentation [here](https://pypi.org/project/Padding/#description).

This module however does not support padding when you are using Unicode character set (and hence the `utf-8` encoding)

I have made a small change to add this support. The API does not change.


How to use it?

>I have also reached out to the original author - if they implement `utf-8` encoding - I will update this description. And you can use it just by installing with `pip`

But for now

1. Install with `pip install Padding`
2. For Testing - replace the contents of `site-packages/Padding.py` with contents of `Padding.py` provided here.
3. Later you can add `Padding.py` as part of your codebase itself so that you don't have to manually update.

> Tip - If you are always going to use English character set (that can be represented only by ASCII encoding) - you do not have to use this version. But let's say your plaintext involves señor (ñ) or characters from Indian script Devanagari (e.g. अ), you can use this improved version.

