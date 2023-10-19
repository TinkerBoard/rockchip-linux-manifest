# rockchip-linux-manifest

This is the manifest project used to download the Tinker OS Debian and Yocto Linux code base for the Tinker Board series.

For more information, please go to the TinkerBoard wiki.

    https://github.com/TinkerBoard/TinkerBoard/wiki

Please refer to the following URL to install Docker Engine on Ubuntu.

    https://docs.docker.com/engine/install/ubuntu/

Please refer to the following URL to install Repo. 

    https://source.android.com/setup/develop#installing-repo

Please refer to the following URL to understand how to download the code base using repo.

    https://source.android.com/setup/build/downloading

The code base has branches for different products and manifests for different releases.

To check out the latest code base for a product, please run the following command and use the branch name for that product as REVISION.

    $ repo init -u https://github.com/TinkerBoard/rockchip-linux-manifest.git -b REVISION

To check out the code base for a specific release, please run the following command and use the branch name for that product as REVISION and the manifest as NAME.xml.

    $ repo init -u https://github.com/TinkerBoard/rockchip-linux-manifest.git -b REVISION -m NAME.xml

Here REVISON is the manifest branch for the product and NAME.xml is the manifest file for the release. Regarding the branches and manifests for each project, please refer to the following release table.

To download the code base source tree to your working directory from the repositories as specified in the default manifest, run:

    $ repo sync

To build the image, go to to the directory where you have downloaded the code base and run the script as the following. This will take a while to install the necessary packages on the host and build the Docker image.

    $ ./docker_builder/docker-builder-run.sh

Once the above is done, you are in the shell of the newly started Docker container. You can start to run commands as usual. You can then run the commands to build the image. The images will be saved in the directory IMAGE.

## Tinker Board 3N
### Tinker OS Debian
|Product|Debian version|Release|Branch|Manifest|Comment|
|-|-|-|-|-|-|
|Tinker Board 3N|Debian 11|latest|linux5.10-rk356x|default.xml|
|Tinker Board 3N|Debian 11|1.0.7|linux5.10-rk356x-tinker_board_3n-debian_11-1.0.7|default.xml|Since there are some fixes need for building, please use the default manifest for this branch to download the code base for this release.|

To build the image, please run the following commands.

    ​$ ./build.sh rockchip_rk3568_tinker_board_3n_debain_defconfig
    $ VERSION=release ./build.sh

### Tinker OS Yocto
|Product|Yocto project version|Release|Branch|Manifest|
|-|-|-|-|-|
|Tinker Board 3N|Yocto 4.0|latest|linux5.10-rk356x|

To build the image, please run the following commands.

    $ ./build.sh rockchip_rk3568_tinker_board_3n_yocto_defconfig
    $ ./build.sh



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
|Tinker Board (S) (R2.0)|Debian 10|latest|linux4.4-rk3288-tinker_board-3.0.16|
|Tinker Edge R|Debian 10|latest|linux4.4-rk3399pro|
|Tinker Edge R|Debian 10|2.0.5|linux4.4-rk3399pro|tinker_edge_r-debian-2.0.5.xml|
|Tinker Board 2/2S|Debian 10|latest|linux4.19-rk3399-debian10|
|Tinker Board 2/2S|Debian 10|2.1.6|linux4.19-rk3399-debian10|tinker_board_2-debian_10-2.1.6.xml|
|Tinker Board 2/2S|Debian 10|2.1.11|linux4.19-rk3399-debian10|tinker_board_2-debian_10-2.1.11.xml|
