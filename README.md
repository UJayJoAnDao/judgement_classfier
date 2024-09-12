# judgement_classifier

## 資料夾結構
- Custom dictionary/
    - dict.txt
    - skip.txt
- Datasets/(原始資料集 => 在模型訓練中也是使用該順序)
    - Abuse/
    - Drug/
    - Sex_assault/
    - Economic_assault/
    - Others/
- ProcessDatasets/(經過處理過的判決書)
    - Abuse/
    - Drug/
    - Sex_assault/
    - Economic_assault/
    - Others/
- models/(存放模型訓練相關的程式)
    - FineTuning_epoch_5/epoch_5/ =>此放置 Bert 模型(檔名:pytorch_model.bin)與配置(config.json)的位置
    - main_code.ipynb =>此程式為主要在訓練 CNN、DNN 與使用 GA 最佳化的集成式模型
    - wiki.zh.vec => 此為原先 fasttext 用的預訓練模型
    - processed_texts.txt => 此檔案目的是蒐集所有文本中出現的文字，將此檔案出現的文字對 fatsttext 進行微調
    - fine_tuned_fasttext.vec => 此檔案為文字轉向量使用到的微調過的模型，需要在底下連結下載並使用
- Web Crawler/(存放資料蒐集階段時所需的爬蟲程式)
- modeltrain.py:微調bert模型使用的程式

## 資料集與模型下載
- 資料集與模型:[點我](https://drive.google.com/drive/folders/1-1IKG4gM4O_JvNAnw-y0W9_kwmLgGKGM?usp=sharing)
