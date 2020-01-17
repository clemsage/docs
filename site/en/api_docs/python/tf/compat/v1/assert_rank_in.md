page_type: reference
<style>{% include "site-assets/css/style.css" %}</style>

<!-- DO NOT EDIT! Automatically generated file. -->

# tf.compat.v1.assert_rank_in


<table class="tfo-notebook-buttons tfo-api" align="left">

<td>
  <a target="_blank" href="https://github.com/tensorflow/tensorflow/tree/r2.0/tensorflow/python/ops/check_ops.py#L1467-L1527">
    <img src="https://www.tensorflow.org/images/GitHub-Mark-32px.png" />
    View source on GitHub
  </a>
</td></table>



Assert `x` has rank in `ranks`.

### Aliases:

* `tf.compat.v1.debugging.assert_rank_in`


``` python
tf.compat.v1.assert_rank_in(
    x,
    ranks,
    data=None,
    summarize=None,
    message=None,
    name=None
)
```



<!-- Placeholder for "Used in" -->

Example of adding a dependency to an operation:

```python
with tf.control_dependencies([tf.compat.v1.assert_rank_in(x, (2, 4))]):
  output = tf.reduce_sum(x)
```

#### Args:


* <b>`x`</b>:  Numeric `Tensor`.
* <b>`ranks`</b>:  Iterable of scalar `Tensor` objects.
* <b>`data`</b>:  The tensors to print out if the condition is False.  Defaults to
  error message and first few entries of `x`.
* <b>`summarize`</b>: Print this many entries of each tensor.
* <b>`message`</b>: A string to prefix to the default message.
* <b>`name`</b>: A name for this operation (optional).
  Defaults to "assert_rank_in".


#### Returns:

Op raising `InvalidArgumentError` unless rank of `x` is in `ranks`.
If static checks determine `x` has matching rank, a `no_op` is returned.



#### Raises:


* <b>`ValueError`</b>:  If static checks determine `x` has mismatched rank.