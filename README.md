---
documentclass: physycomen
title:  "data_tools"
author: "Fabbri, Sinigardi"
---

<a href="http://www.physycom.unibo.it"> 
<div class="image">
<img src="https://cdn.rawgit.com/physycom/templates/697b327d/logo_unibo.png" width="90" height="90" alt="© Physics of Complex Systems Laboratory - Physics and Astronomy Department - University of Bologna"> 
</div>
</a>
<a href="https://travis-ci.org/physycom/data_tools"> 
<div class="image">
<img src="https://travis-ci.org/physycom/data_tools.svg?branch=master" width="90" height="20" alt="Build Status"> 
</div>
</a>
<a href="https://ci.appveyor.com/project/cenit/list-to-json"> 
<div class="image">
<img src="https://ci.appveyor.com/api/projects/status/cf9icu8pp70hqwip?svg=true" width="90" height="20" alt="Build Status"> 
</div>
</a>


### Purpose
This tool has been written in order to easily plot some statistics on inertial and GNSS data coming from tests developed and executed at the Physics of the City Laboratory.

### Installation
**make** and a **C++11** compatible compiler are required. Clone the repo and type ``make``, it should be enough in most cases to build the two executables!   
There's also a **VS2015** solution avalaible.   
Contains [jsoncons](https://github.com/danielaparker/jsoncons) as a git submodule.   
Uses the boost C++ libraries (http://www.boost.org/).   

json configuration example:
```
{
  "input_file_name"               : "a_acc.txt",
  "output_file_histox"            : "a_acc_histox_bin.txt",
  "output_gnuplot_file_histox"    : "a_acc_histox_bin.plt",
  "output_image_file_histox"      : "a_acc_histox_bin.png",
  "output_file_histoy"            : "a_acc_histoy_bin.txt",
  "output_gnuplot_file_histoy"    : "a_acc_histoy_bin.plt",
  "output_image_file_histoy"      : "a_acc_histoy_bin.png",
  "output_gnuplot_file_histoxy"   : "a_acc_histoxy_bin.plt",
  "output_image_file_histoxy"     : "a_acc_histoxy_bin.png",
  "output_file_cart"              : "a_acc_cart_bin.txt",
  "output_gnuplot_file_cart"      : "a_acc_cart_bin.plt",
  "output_image_file_cart"        : "a_acc_cart_bin.png",
  "output_file_polar"             : "a_acc_polar_bin.txt",
  "output_gnuplot_file_polar"     : "a_acc_polar_bin.plt",
  "output_image_file_polar"       : "a_acc_polar_bin.png",
  "output_gnuplot_file_polar_exp" : "a_acc_polar_bin_exp.plt",
  "output_image_file_polar_exp"   : "a_acc_polar_bin_exp.png",
  "col_acc_x"                     :  2,
  "col_acc_y"                     :  3,
  "nbin_x"                        :  500,
  "nbin_y"                        :  500,
  "nbin_magn"                     :  500,
  "nbin_angle"                    :  62
//  "min_acc_x"                   :  0.0,
//  "max_acc_x"                   :  0.0,
//  "min_acc_y"                   :  0.0,
//  "max_acc_y"                   :  0.0,
//  "min_acc"                     :  0.0,
//  "max_acc"                     :  0.0
 }
```

