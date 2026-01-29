uv init rpcats<br/>
<pre>
<i>
[project]
name = "rpcats"
version = "0.1.0"
description = "Display information about specified breed of cats."
readme = "README.md"
requires-python = ">=3.11"
</i>
</pre>
cd rpcats<br/>
uv run main.py # this will give error, no package "requests"<br/>
uv add requests<br/>
<pre>
<i>
dependencies = [
    "requests>=2.32.5",
]
</i>
</pre>
uv run main.py<br/>
uv run main.py -h<br/>
uv run main.py none<br/>
uv run main.py "Australian Mist"<br/>
uv add --dev pytest<br/>
<pre>
<i>
[dependency-groups]
dev = [
    "pytest>=9.0.2",
]
</i>
</pre>
uv pip list<br/>
uv lock<br/>
uv sync<br/>
<pre>
<i>
[project.scripts]
rpcats = "main:main"

[build-system]
requires = ["setuptools>=78.1.0", "wheel>=0.45.1"]
build-backend = "setuptools.build_meta"
</i>
</pre>
uv build<br/>
<pre>
<i>
Successfully built dist\rpcats-0.1.0.tar.gz
Successfully built dist\rpcats-0.1.0-py3-none-any.whl
</i>
</pre>
uv cache dir<br/>
uv cache --help<br/>
uv cache clean<br/>