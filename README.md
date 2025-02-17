Moneta (https://moneta.misas.us)
===


What is Moneta?
---
**Moneta** is a digital currency, also known as crypto currency which enables instant payments to anyone, anywhere in the world. Moneta uses peer-to-peer technology to operate with no central authority: managing transactions and issuing money are carried out collectively by the network. Moneta Core is the name of the open source software which enables the use of this currency.

For more information, as well as an immediately useable, binary version of
the Moneta Core software, see [https://moneta.misas.us](https://moneta.misas.us).

The project is a fork of Bitcoin/Litecoin, it's based on the same proven and reliable core, but with major differences:
* Bigger total supply of **21,000,000,000** for a longer production, a more factual value, and availability for real transactions
* Higher incentives for miners:
    * **500** Monete per block award instead of 50
    * Lottery reward block of **5000** Monete for every mined block multiple of 5000. This is an exclusive feature of Moneta
    * **No Halving**. Miners are always rewarded the full amount
    * Easier technical adoption than many other digital currency
* Transaction fees as **5x cheaper** than Litecoin. Making the transactions very affordable for the consumers
* Built on the very reliable and proven Bitcoin blockchain
* Ability to turn off transaction fees for private economy implementations (for private implementations, contact the development team)


Who is behind Moneta?
---------------------
[Michael Montuori](https://github.com/mmontuori) is the main developer behind Moneta. Michael has over 30 years of experience. His public credentials are listed in his [public resume](https://registry.jsonresume.org/mmontuori).

Other developers, contributors, and testers:
* Pino Caci


License
-------
Moneta Core is released under the terms of the MIT license. See [COPYING](COPYING) for more
information or see https://opensource.org/licenses/MIT.


Development Process
-------------------
The `master` branch is regularly built and tested, but is not guaranteed to be
completely stable. [Tags](https://github.com/mmontuori/moneta/tags) are created
regularly to indicate new official, stable release versions of Moneta Core.

The contribution workflow is described in [CONTRIBUTING.md](CONTRIBUTING.md)
and useful hints for developers can be found in [doc/developer-notes.md](doc/developer-notes.md).

The developer [mailing list](https://groups.google.com/u/1/g/moneta-coin)
should be used to discuss complicated or controversial changes before working
on a patch set.

Developer IRC can be found on Freenode at #moneta-dev.


Testing
-------
Testing and code review is the bottleneck for development; we get more pull
requests than we can review and test on short notice. Please be patient and help out by testing
other people's pull requests, and remember this is a security-critical project where any mistake might cost people
lots of money.

### Automated Testing

Developers are strongly encouraged to write [unit tests](src/test/README.md) for new code, and to
submit new unit tests for old code. Unit tests can be compiled and run
(assuming they weren't disabled in configure) with: `make check`. Further details on running
and extending unit tests can be found in [/src/test/README.md](/src/test/README.md).

There are also [regression and integration tests](/test), written
in Python, that are run automatically on the build server.
These tests can be run (if the [test dependencies](/test) are installed) with: `test/functional/test_runner.py`

The Travis CI system makes sure that every pull request is built for Windows, Linux, and macOS, and that unit/sanity tests are run automatically.

### Manual Quality Assurance (QA) Testing

Changes should be tested by somebody other than the developer who wrote the
code. This is especially important for large or high-risk changes. It is useful
to add a test plan to the pull request description if testing the changes is
not straightforward.


Translations
------------
We only accept translation fixes that are submitted through [Bitcoin Core's Transifex page](https://www.transifex.com/projects/p/bitcoin/).
Translations are converted to Moneta periodically.

Translations are periodically pulled from Transifex and merged into the git repository. See the
[translation process](doc/translation_process.md) for details on how this works.

**Important**: We do not accept translation changes as GitHub pull requests because the next
pull from Transifex would automatically overwrite them again.
