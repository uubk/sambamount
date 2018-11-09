# sambamount
[![CircleCI status](https://img.shields.io/circleci/project/github/uubk/sambamount/master.svg?style=shield)](https://circleci.com/gh/uubk/sambamount/tree/master)
![License](https://img.shields.io/github/license/uubk/sambamount.svg?style=popout)

Add a samba server to `/etc/fstab` and set up local caching.

## Configuration
| Name | Default value | Description |
| ---- | ------------- | ----------- |
| `sambamount_user` | `""` | User for logon |
| `sambamount_password` | `""` | Password for logon |
| `sambamount_share` | `""` | UNC path of share |
| `sambamount_mountpoint` | `""` | local mount point |
| `sambamount_options` | (see defaults/main.yml) | Mount options |
| `sambamount_cache_enable` | `True` | Whether to enable local disk caching for the share |
| `sambamount_cache_limit_run` | `25$` | If free disk space is above this threshold, cache normally |
| `sambamount_cache_limit_cull` | `23%` | If free disk space is below this threshold, start culling the cache |
| `sambamount_cache_limit_stop` | `20%` | If free disk space is below this threshold, stop caching |

## License
GPLv3
