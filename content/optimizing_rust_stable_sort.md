+++
title = "Optimizing stable sort in Rust (and mostly failing)"
date = 2022-08-06

[taxonomies]
tags = ["rust", "sort"]
+++

This journey started when I discovered [fluxsort](https://github.com/scandum/fluxsort) a seemingly novel stable sort implementation promising impressive performance. It claims to be faster than pdqsort which is the pattern defeating quick sort used by Rust's [sort_unstable](https://doc.rust-lang.org/std/primitive.slice.html#method.sort_unstable). My hope was to port this C library to Rust and improve the standard library stable sort with it.
<!-- more -->

 