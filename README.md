uv init rpcats<br/>
cd rpcats<br/>
uv run main.py<br/>
uv add requests<br/>
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