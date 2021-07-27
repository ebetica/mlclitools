#
## qpp
Bash based tool for plotting things quickly

Examples:

Line plot
```
python -c 'import numpy as np; print("\n".join(str(x) for x in np.random.randn(100)))' | qpp line | display
```

Most data is one point per line, like
```
1 0
2 .2
3 .5
4 .3
```

and multiple series are separated by END, and non-number first lines are parsed as headers
```
header
1
2
END
header2
3
4
END
```

## pyscrun

I'm tired of pressing `python -m` to run my importable code, so `pyscrun` automagically detects your git root / python root and sets it to PYTHON_HOME so you don't have to.

## slmt

Easy to use slurm cli wrapper.
Supports checkpointing via `--retry`, tarring your code via `slmt mkimg`, and letting you pipe commands in so you can test your runs easily.
Run `slmt --help` for more information.
