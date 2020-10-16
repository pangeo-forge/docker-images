FROM pangeo/pangeo-notebook:2020.10.10
ENV PATH="/srv/conda/envs/notebook/bin:${PATH}" JUPYTERHUB_USER=pangeoforge TZ=UTC
USER ${NB_USER}
RUN python -m pip install --no-cache-dir \
    prefect[kubernetes]==0.13.0 \
    pygithub=1.53 \
    git+https://github.com/pangeo-forge/pangeo-forge
