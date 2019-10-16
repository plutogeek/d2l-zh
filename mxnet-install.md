## 第一步：安装Anaconda

早期安装的是TensorFlow，使用的前置安装工具是Anaconda。总体感觉是：这个工具很好用！故Anaconda详细安装的步骤省略，这个不太费事。

## 第二步：安装MXNet

起因是从网络上搞到一本李沐大师参与编写的《动手学深度学习》，且更新时间为2019年4月，不可多得。于是，根据书中源码调试要求，想再安装MXNet框架，全面学习一下有关内容。

所以，自然想到使用Anaconda安装MXNet。现在完成安装后，总结来看——安装非常顺利；比较网络上的其他安装记录来看，更为简洁可取。现描述如下：

第1步：打开命令行，运行命令conda create -n mxnet

得到如下提示：

```
Collecting package metadata: done
Solving environment: done
```

## Package Plan ##
```
  environment location: /Users/zxzpc/anaconda3/envs/mxnet

Proceed ([y]/n)? y
按下回车，继续往下操作。接下来的提示如下：

Preparing transaction: done
Verifying transaction: done
Executing transaction: done
#
# To activate this environment, use
#
#     $ conda activate mxnet
#
# To deactivate an active environment, use
#
#     $ conda deactivate
```

第2步：激活mxnet环境

根据上面的提示，运行如下命令：
```
conda activate mxnet
```
正式安装MXNet

命令如下：
```
conda install mxnet
```
接下来的提示如下：
```
Collecting package metadata: done
Solving environment: done
```

```
## Package Plan ##

  environment location: ............./anaconda3/envs/mxnet

  added / updated specs:
    - mxnet

The following packages will be downloaded:

    package                    |            build
    ---------------------------|-----------------
    certifi-2019.6.16          |           py36_0         154 KB
    mkl-2019.4                 |              233       155.2 MB
    numpy-1.14.2               |   py36ha9ae307_0         3.9 MB
    ------------------------------------------------------------
                                           Total:       159.2 MB

The following NEW packages will be INSTALLED:

  _mutex_mxnet       pkgs/main/osx-64::_mutex_mxnet-0.0.40-mkl
  asn1crypto         pkgs/main/osx-64::asn1crypto-0.24.0-py36_0
  blas               pkgs/main/osx-64::blas-1.0-mkl
  bzip2              pkgs/main/osx-64::bzip2-1.0.6-h1de35cc_5
  ca-certificates    pkgs/main/osx-64::ca-certificates-2019.5.15-0
  cairo              pkgs/main/osx-64::cairo-1.14.12-hc4e6be7_4
  certifi            pkgs/main/osx-64::certifi-2019.6.16-py36_0
  cffi               pkgs/main/osx-64::cffi-1.12.3-py36hb5b8e2f_0
  chardet            pkgs/main/osx-64::chardet-3.0.4-py36_1
  cryptography       pkgs/main/osx-64::cryptography-2.7-py36ha12b0ac_0
  ffmpeg             pkgs/main/osx-64::ffmpeg-3.4-h8a2ae75_0
  fontconfig         pkgs/main/osx-64::fontconfig-2.13.0-h5d5b041_1
  freetype           pkgs/main/osx-64::freetype-2.9.1-hb4e5f40_0
  gettext            pkgs/main/osx-64::gettext-0.19.8.1-h15daf44_3
  glib               pkgs/main/osx-64::glib-2.56.2-hd9629dc_0
  graphite2          pkgs/main/osx-64::graphite2-1.3.13-h2098e52_0
  harfbuzz           pkgs/main/osx-64::harfbuzz-1.8.8-hb8d4a28_0
  hdf5               pkgs/main/osx-64::hdf5-1.10.2-hfa1e0ec_1
  icu                pkgs/main/osx-64::icu-58.2-h4b95b61_1
  idna               pkgs/main/osx-64::idna-2.6-py36h8628d0a_1
  intel-openmp       pkgs/main/osx-64::intel-openmp-2018.0.3-0
  jasper             pkgs/main/osx-64::jasper-2.0.14-h636a363_1
  jpeg               pkgs/main/osx-64::jpeg-9b-he5867d9_2
  libcxx             pkgs/main/osx-64::libcxx-4.0.1-hcfea43d_1
  libcxxabi          pkgs/main/osx-64::libcxxabi-4.0.1-hcfea43d_1
  libedit            pkgs/main/osx-64::libedit-3.1.20181209-hb402a30_0
  libffi             pkgs/main/osx-64::libffi-3.2.1-h475c297_4
  libgfortran        pkgs/main/osx-64::libgfortran-3.0.1-h93005f0_2
  libiconv           pkgs/main/osx-64::libiconv-1.15-hdd342a3_7
  libmklml           pkgs/main/osx-64::libmklml-2018.0.3-0
  libmxnet           pkgs/main/osx-64::libmxnet-1.2.1-mkl_hbefbd7c_1
  libopencv          pkgs/main/osx-64::libopencv-3.4.1-h14a57ad_3
  libopus            pkgs/main/osx-64::libopus-1.3-h1de35cc_0
  libpng             pkgs/main/osx-64::libpng-1.6.37-ha441bb4_0
  libprotobuf        pkgs/main/osx-64::libprotobuf-3.5.2-h2cd40f5_0
  libtiff            pkgs/main/osx-64::libtiff-4.0.10-hcb84e12_2
  libvpx             pkgs/main/osx-64::libvpx-1.7.0-h378b8a2_0
  libxml2            pkgs/main/osx-64::libxml2-2.9.9-hab757c2_0
  mkl                pkgs/main/osx-64::mkl-2019.4-233
  mkl-dnn            pkgs/main/osx-64::mkl-dnn-0.14-h04f5b5a_0
  mxnet              pkgs/main/osx-64::mxnet-1.2.1-h8cc8929_0
  ncurses            pkgs/main/osx-64::ncurses-6.1-h0a44026_1
  numpy              pkgs/main/osx-64::numpy-1.14.2-py36ha9ae307_0
  openssl            pkgs/main/osx-64::openssl-1.1.1c-h1de35cc_1
  pcre               pkgs/main/osx-64::pcre-8.43-h0a44026_0
  pip                pkgs/main/osx-64::pip-19.1.1-py36_0
  pixman             pkgs/main/osx-64::pixman-0.38.0-h1de35cc_0
  py-mxnet           pkgs/main/osx-64::py-mxnet-1.2.1-py36h4bd7469_0
  pycparser          pkgs/main/osx-64::pycparser-2.19-py36_0
  pyopenssl          pkgs/main/osx-64::pyopenssl-19.0.0-py36_0
  pysocks            pkgs/main/osx-64::pysocks-1.7.0-py36_0
  python             pkgs/main/osx-64::python-3.6.8-haf84260_0
  readline           pkgs/main/osx-64::readline-7.0-h1de35cc_5
  requests           pkgs/main/osx-64::requests-2.18.4-py36h4516966_1
  setuptools         pkgs/main/osx-64::setuptools-41.0.1-py36_0
  six                pkgs/main/osx-64::six-1.12.0-py36_0
  sqlite             pkgs/main/osx-64::sqlite-3.28.0-ha441bb4_0
  tk                 pkgs/main/osx-64::tk-8.6.8-ha441bb4_0
  urllib3            pkgs/main/osx-64::urllib3-1.22-py36h68b9469_0
  wheel              pkgs/main/osx-64::wheel-0.33.4-py36_0
  xz                 pkgs/main/osx-64::xz-5.2.4-h1de35cc_4
  zlib               pkgs/main/osx-64::zlib-1.2.11-h1de35cc_3
  zstd               pkgs/main/osx-64::zstd-1.3.7-h5bba6e5_0

Proceed ([y]/n)? 

Downloading and Extracting Packages
numpy-1.14.2         | 3.9 MB    | ##################################### | 100% 
certifi-2019.6.16    | 154 KB    | ##################################### | 100% 
mkl-2019.4           | 155.2 MB  | ##################################### | 100% 
Preparing transaction: done
Verifying transaction: done
Executing transaction: done

```
至此，MXNet安装结束
