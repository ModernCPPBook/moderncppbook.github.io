---
layout: post
title:  "Building HPX applications"
date:   2024-12-06 14:34:25
categories: building
tags: cmake
---
In this blog post, we will provide more details on how to build your own HPX application using [CMake](https://cmake.org/). In the previous [blog post](https://hpxbook.stellar-group.org/building/2024/08/13/build-hpx.html) we showcased how on compile and install HPX.


## Building a HPX application

We assume that we have a `CMakeLists.txt` and the `main.cpp` in the same folder. Below the main `CMakeLists.txt` is listed

{% highlight bash %}
project(MyHPXApp LANGUAGES CXX)
cmake_minimum_required(VERSION 3.18)

# Find the HPX package
find_package(HPX REQUIRED)

# Compile a HPX application
add_hpx_executable(app SOURCES main.cpp)
{% endhighlight %}






