FROM python:slim

RUN pip install --no-cache-dir notebook \
&& apt-get update && apt-get install -y \
	wget \
	julia \
&&  rm -rf /var/lib/apt/lists/*

RUN julia -e 'using Pkg; Pkg.add.(["IJulia", "Plots"])'

ENTRYPOINT ["/usr/local/bin/jupyter", "notebook", "--allow-root", "--no-browser"]
CMD ["--ip='*'", "--port=8888", "--notebook-dir=/root"]
