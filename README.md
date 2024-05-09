<<<<<<< Updated upstream
# Sentiment Analysis for Korean Sentences

### <sup>Emotion Inference Model of </sup> [<img src="https://github.com/mj0410/Korean-SentimentAnalysis/assets/66175878/13608ed3-b5ef-4113-9d92-0ae64fe98bce" width="120">](https://github.com/pal-ette/iNotePal)
</br>

### <sup>:books: Training Data from </sup> [<img src="https://github.com/mj0410/Korean-SentimentAnalysis/assets/66175878/819e5a07-535c-4e29-9728-b93ad6a75fd2" width="100">](https://aihub.or.kr/)

> [한국어 감정 정보가 포함된 단발성 대화 데이터셋](https://aihub.or.kr/aihubdata/data/view.do?dataSetSn=270)</br>
> [한국어 감정 정보가 포함된 연속적 대화 데이터셋](https://aihub.or.kr/aihubdata/data/view.do?dataSetSn=271)</br>
> [감정 분류를 위한 대화 음성 데이터셋](https://www.aihub.or.kr/aihubdata/data/view.do?currMenu=115&topMenu=100&dataSetSn=263)
</br>

### :computer: Models

> LSTM </br>
> KoBERT `conv-7_KoBERT.ipynb` `merged_dataset_10k_KoBERT.ipynb` </br>
> RoBERTa `roberta_large_5k_samples_7_emotions.ipynb` </br> 

BEST MODEL - RoBERTa + LSTM `roberta-small.ipynb` built upon [klue/roberta-small🤗](https://huggingface.co/klue/roberta-small) </br>
</br>

### :bricks: Model Architecture
=======
# Roberta-small-lstm

[klue/roberta-small](https://huggingface.co/klue/roberta-small)

### Model Architecture
>>>>>>> Stashed changes

```mermaid
graph BT;
    emb[Roberta Embeddings];
    enc[Roberta Encoder];
    lstm[LSTM Layer];
    cla[Roberta Classifier];
    emb --> enc;
    enc --> lstm;
    lstm --> cla;
```
<<<<<<< Updated upstream
</br>

### :thinking: Sentiment Analysis Example
=======

### Sentiment Analysis Example
>>>>>>> Stashed changes

```diff
Input      :  한강에 가면 유독 그런 생각해요. 빠져 죽을까. 빠지면 구출 될까, 한번에 죽을까.
Prediction :  공포

Input      :  공부도 재미있고 학교 활동도 재미있었어요.
Prediction :  기쁨

Input      :  나는 순간 내가 잘못 들은 줄 알았어.
Prediction :  놀람

Input      :  사람 취급 못 받고 사는 거 같아.
Prediction :  분노

Input      :  사실 이런 생각들이 비참한 자위 같아서… 요즘은 마음이 좀 심란해요.
Prediction :  슬픔

Input      :  약도 먹어봐야 알겠지만 크게 기대는 안 하게 되는 것 같아요.
Prediction :  중립

Input      :  저게 인간이야? 잘 안 씻어서 냄새까지 나. 짐승도 저것보단 낫겠다.
Prediction :  혐오
```
<<<<<<< Updated upstream
</br>

### :chart_with_upwards_trend: Model Evaluation

##### Loss-Epoch / Accuracy-Epoch Curve
<img src="https://github.com/mj0410/Korean-SentimentAnalysis/assets/66175878/894ad2c7-7b63-4313-9155-029a90e41f49" width="700"></br>

##### Confusion Matrix / f1-score / recall / precision per Emotion
<img src="https://github.com/mj0410/Korean-SentimentAnalysis/assets/66175878/a7329122-3d2c-4e4a-968c-bf39aefdf8b3" width="350">
<img src="https://github.com/mj0410/Korean-SentimentAnalysis/assets/66175878/7f7491e2-74a1-4b10-ae88-71f0e2dd6d09" width="350">
=======


### Model Evaluation

<img src="https://github.com/pal-ette/iNotePal/assets/66175878/6d235826-5f81-4acd-9fcb-562f2113c288" width="400">

<img src="https://github.com/pal-ette/iNotePal/assets/66175878/3c77537d-fb19-4050-bd62-9c2a1c7e509b" width="400">
>>>>>>> Stashed changes
