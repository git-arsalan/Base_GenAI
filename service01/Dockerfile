FROM jupyter/base-notebook:latest
WORKDIR /service01
RUN pip install poetry
COPY . /service01/
RUN poetry config virtualenvs.create false
EXPOSE 8888
CMD ["jupyter", "notebook" , "--port" , "8888" , "--no-browser" ,  "--allow-root"]