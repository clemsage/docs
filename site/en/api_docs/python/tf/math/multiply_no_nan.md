page_type: reference
<style>{% include "site-assets/css/style.css" %}</style>

<!-- DO NOT EDIT! Automatically generated file. -->

# tf.math.multiply_no_nan


<table class="tfo-notebook-buttons tfo-api" align="left">

<td>
  <a target="_blank" href="https://github.com/tensorflow/tensorflow/tree/r2.0/tensorflow/python/ops/math_ops.py#L1121-L1143">
    <img src="https://www.tensorflow.org/images/GitHub-Mark-32px.png" />
    View source on GitHub
  </a>
</td></table>



Computes the product of x and y and returns 0 if the y is zero, even if x is NaN or infinite.

### Aliases:

* `tf.compat.v1.math.multiply_no_nan`
* `tf.compat.v2.math.multiply_no_nan`


``` python
tf.math.multiply_no_nan(
    x,
    y,
    name=None
)
```



<!-- Placeholder for "Used in" -->


#### Args:


* <b>`x`</b>: A `Tensor`. Must be one of the following types: `float32`, `float64`.
* <b>`y`</b>: A `Tensor` whose dtype is compatible with `x`.
* <b>`name`</b>: A name for the operation (optional).


#### Returns:

The element-wise value of the x times y.