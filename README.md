# rockchip-linux-manifest

For more information, please go to TinkerBoard wiki.

    https://github.com/TinkerBoard/TinkerBoard/wiki

Please refer to the following URL to install Docker Engine on Ubuntu.

    https://docs.docker.com/engine/install/ubuntu/

Please refer to the following URL to install Repo. 

    https://source.android.com/setup/develop#installing-repo

Please refer to the following URL to understand how to download the AOSP-based source.

    https://source.android.com/setup/build/downloading

To check out the specific branch:

    $ repo init -u https://github.com/TinkerBoard/rockchip-linux-manifest.git -b REVISION

To check out the specific release:

    $ repo init -u https://github.com/TinkerBoard/rockchip-linux-manifest.git -b REVISION -m NAME.xml

Here REVISON is the manifest branch or revision (use HEAD for default) and NAME.xml is the initial manifest file. Regarding the branches and manifest for each project, please refer to the following release table.

To download the Android source tree to your working directory from the repositories as specified in the default manifest, run:

    $ repo sync

|Product|Debian version|Release|Branch|Manifest|
|-|-|-|-|-|
|Tinker Board (S) (R2.0)|Debian 10|latest|linux4.4-rk3288-tinker_board|
|Tinker Board (S) (R2.0)|Debian 10|3.0.11|linux4.4-rk3288-tinker_board|tinker_board-debian-3.0.11.xml|
|Tinker Board (S) (R2.0)|Debian 10|3.0.13|linux4.4-rk3288-tinker_board|tinker_board-debian-3.0.13.xml|
|Tinker Board (S) (R2.0)|Debian 10|3.0.16|linux4.4-rk3288-tinker_board|tinker_board-debian-3.0.16.xml|
|Tinker Board (S) (R2.0)|Debian 10|latest|linux4.4-rk3288-tinker_board-3.0.13|
|Tinker Board (S) (R2.0)|Debian 10|3.0.13.1|linux4.4-rk3288-tinker_board-3.0.13|tinker_board-debian-3.0.13.1.xml|
|Tinker Board (S) (R2.0)|Debian 10|3.0.13-2|linux4.4-rk3288-tinker_board-3.0.13|tinker_board-debian-3.0.13-2.xml|
|Tinker Board (S) (R2.0)|Debian 10|3.0.13-3|linux4.4-rk3288-tinker_board-3.0.13|tinker_board-debian-3.0.13-3.xml|
|Tinker Board (S) (R2.0)|Debian 10|3.0.13-4|linux4.4-rk3288-tinker_board-3.0.13|tinker_board-debian-3.0.13-4.xml|
|Tinker Board (S) (R2.0)|Debian 10|3.0.13-5|linux4.4-rk3288-tinker_board-3.0.13|tinker_board-debian-3.0.13-5.xml|
|Tinker Board (S) (R2.0)|Debian 10|3.0.13-6|linux4.4-rk3288-tinker_board-3.0.13|tinker_board-debian-3.0.13-6.xml|
