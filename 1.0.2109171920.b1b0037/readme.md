# Sireum OSATE Plugins 1.0.2109171920.b1b0037 Release

This update site contains the 1.0.2109171920.b1b0037 release of Sireum's OSATE plugins and is only
intended to be used with [Sireum's Phantom tool](https://github.com/sireum/phantom)
or the FMIDE install script (see the
[CASE](https://github.com/sireum/case-env#setting-up-fmide-and-hamr-only)
setup instructions for more information). No other support is offered.

## How to Install the 1.0.2109171920.b1b0037 Sireum OSATE Plugins Using Phantom

Install [Sireum](https://github.com/sireum/kekinian#installing) and then run the following:

```batch
$SIREUM_HOME/bin/sireum hamr phantom -u --features "org.sireum.aadl.osate.cli.feature.feature.group=https://raw.githubusercontent.com/sireum/osate-update-site/master/1.0.2109171920.b1b0037;org.sireum.aadl.osate.hamr.feature.feature.group=https://raw.githubusercontent.com/sireum/osate-update-site/master/1.0.2109171920.b1b0037"
```

## Resolving Potential Version Issues

The Sireum OSATE plugins use the version of Sireum installed at ``$SIREUM_HOME/bin/sireum.jar``
which may no longer be compatible with this version of the plugins. If that is the case and
you still want to use this version of the plugins then you will need to build the
b1b0037 version of Sireum and then run Phantom as follows:

* Windows:

  ```batch
  git clone https://github.com/sireum/kekinian Sireum
  cd Sireum
  git checkout b1b0037
  git submodule update --init --recursive
  bin\build.cmd
  bin\sireum hamr phantom -u --features "org.sireum.aadl.osate.cli.feature.feature.group=https://raw.githubusercontent.com/sireum/osate-update-site/master/1.0.2109171920.b1b0037;org.sireum.aadl.osate.hamr.feature.feature.group=https://raw.githubusercontent.com/sireum/osate-update-site/master/1.0.2109171920.b1b0037"
  ```

* Linux:

  ```bash
  git clone https://github.com/sireum/kekinian Sireum
  cd Sireum
  git checkout b1b0037
  git submodule update --init --recursive
  bin/build.cmd
  bin/sireum hamr phantom -u --features "org.sireum.aadl.osate.cli.feature.feature.group=https://raw.githubusercontent.com/sireum/osate-update-site/master/1.0.2109171920.b1b0037;org.sireum.aadl.osate.hamr.feature.feature.group=https://raw.githubusercontent.com/sireum/osate-update-site/master/1.0.2109171920.b1b0037"
  ```

* macOS:

  ```bash
  git clone https://github.com/sireum/kekinian Sireum
  cd Sireum
  git checkout b1b0037
  git submodule update --init --recursive
  bin/build.cmd
  bin/sireum hamr phantom -u --features "org.sireum.aadl.osate.cli.feature.feature.group=https://raw.githubusercontent.com/sireum/osate-update-site/master/1.0.2109171920.b1b0037;org.sireum.aadl.osate.hamr.feature.feature.group=https://raw.githubusercontent.com/sireum/osate-update-site/master/1.0.2109171920.b1b0037"
  ```

