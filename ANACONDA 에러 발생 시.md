## ANACONDA

## 20210607

PANDAS , PANDAS PROFILING , IPYWIDGETS 설치



anaconda 내 pypi 에서 다운받은 패키지 버전 확인 방법 : pip freeze



## kernel 오류

conda deactivate multi

conda remove --name multi--all

conda create --name multi python=3.7.6

conda activate multi

pip install ipykernel

python -m ipykernel install --user --name multi --display-name "Python Multi"

conda install -c conda-forge jupyterlab

pip install pandas

pip install pandas-profiling==2.12.0

pip install ipywidgets

conda activate multi

jupyter lab