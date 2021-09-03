## bevents

### Installing support for events

The script that adds support for events can be found at the root of bevents
named as `installEventsSupport`. This script needs to be performed as superuser.

You can run the installation script based on your backbone environment. The only information that is not possible to be
passed through the current environment is the release type (since `BBASE_VERSION` is resolved for the actual version). Therefore, it needs to be specified (`stable`, `beta`, `alpha`)
in case this information is not provided `stable` is used by default, for instance:
```bash
sudo ./installEventsSupport --release-type "alpha" --core-config $BACKBONE_CORE_CONFIG --backbone-root $BACKBONE_ROOT --backbone-dev-root $BACKBONE_DEV_ROOT
```
Note: The `--backbone-dev-root` is optional. It should only be used for development purposes.

More details about the installation script can be found under the help:
```bash
./installEventsSupport --help
```
