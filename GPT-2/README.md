## GPT-2

### 사용방법
*   git repository 다운 받기

```
git clone https://github.com/ye1111k/NUZAK
```

*   GPT-2를 사용할 때 필요한 모듈 설치하기

```
pip install --upgrade -r requirements.txt
```
* 사용할 모델 다운받기
- 뒤의 숫자는 모델의 parameter 수를 의미, parameter 수가 클수록 다운받는 시간이 오래 걸리지만 더 정교한 모델
- 124M, 355M, 774M, 1.5B의 총 네 가지 모델이 있다.
```
python download_model.py 774M
```
* GPT2 repository 내 src 폴더의 interactive_conditional_samples.py 파일의 model_name 부분을 내가 사용할 모델의 parameter로 바꿔준다.
```
python src/interactive_conditional_samples.py --model_name='774M' --nsamples=2 --temparature=.80
```
