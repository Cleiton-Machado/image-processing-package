--------------
charset: utf-8
--------------

# Desafio: Pacote de Processamento de Imagens

## Description. 

- Esse projeto consiste na criação de um pacote para python, com base no curso ministrado por Karina Kato.
- É apenas um pacote de exemplo, baseado no [scikit-image](https://scikit-image.org)


## Passos para a hospedagem no Pypi

- Primeiro se realiza uma instalação ou upgrade do `pip`, `twine`, `setuptools` e `wheel`
- remova a opção `--user` se não deseja instalar no `user.home` ou esteja usando um `venv`.
```bash
python -m pip install --upgrade pip
python -m pip install --user twine
python -m pip install --user setuptools
python -m pip install --user wheel
```
- Cria-se as distribuições
```bash
python setup.py sdist bdist_wheel
```
- Serão criadas 3 pastas no projeto: 
  - build
  - dist
  - image_processing_package.egg-info
- O próximo passo é o upload no Test Pypi.
```bash
python -m twine upload --repository-url https://test.pypi.org/legacy/ dist/*

```
- O comando para upload no Pypi é:
```bash
python -m twine upload --repository-url https://upload.pypi.org/legacy/ dist/*

```
## Instalação
- Para a instalação local, é necessário instalar os requerimentos primeiro.
```bash
pip install -r requirements.txt
 ```

Para a instalação do pacote, basta usar o [pip](https://pip.pypa.io/en/stable/) direcionando para o image-processing-test-package

```bash
pip install processing-image-mctech
```
---
## Uso
- Basta importar os módulos de acordo com o que deseja

---
## Autor
Cleiton Machado

#### [LinkdIn](https://www.linkedin.com/in/cleiton-machado/)


## Licença
[MIT](https://choosealicense.com/licenses/mit/)


