RadonX
===========

Getting Started
---------------

To get started with RadonX, you'll need to get
familiar with [Git and Repo](http://source.android.com/source/using-repo.html).

To build RadonX for OnePlus One USE :

    repo init -u git://github.com/RadonX-ROM/paradox_manifest.git -b lollipop_bacon

To port a MSM8226 device USE :

    repo init -u git://github.com/AOSParadox/local_aosparadox.git -b lollipop_msm8226

To port a MSM8974 device USE :

    repo init -u git://github.com/AOSParadox/local_aosparadox.git -b lollipop_msm8974

Then to sync up:

    repo sync -c -j5

When everything is synced do
    
    . build/envsetup.sh && lunch full_yourdevice-userdebug

Setup CCACHE and build using
    
    make -j8 otapackage

