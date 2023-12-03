## M-Connectivity [^1]

Basically 8-c but stricter. Let three pixels, `a`, `b` and `c`:

```
0 0 0
0 a 0
b 0 0
```

`a` and `b` is 8-connected and m-connected.

```
0 0 0
0 a 0
b c 0
```

`a` and `b` is 8-connected, but not m-connected because `c` exist as both 4-connected of `a` and `b`.

## Distance

- Euclidean: Pythagoras
- D4: $|x1-x2|+|y1-y2|$
- D8: $max(|x1-x2|,|y1-y2|)$

## References

[^1]: https://stackoverflow.com/questions/45342967