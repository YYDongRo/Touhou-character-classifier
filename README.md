***TOUHOU VISION AI***


**Introduction**

This is a AI classfier that recognizes Hakurei Reimu(博丽灵梦), Kirisame Marisa(雾雨魔理沙), Cirno(琪露诺) (More characters will be coming up!) in Touhou Project. I built the model with Pytorch, and trained by finding dataset oniline. I also include a Grad-CAM heatmaps as the output for visual explanations of 'WHY' this character is identified.


**Installation (Using terminal)**

*1. Clone the repo*
```python
git clone https://github.com/YYDongRo/Touhou_character_classifier.git
cd Touhou_character_classifier
```

*2. Create a virtual environment*
```python
source .venv/bin/activate
```

*3. Install dependencies*
```python
pip install -r requirements.txt
```

*4. Web interface*
```python
streamlit run app.py
```

*5. Feel free to train the model yourself, but remember to place the dataset like shown below*
```python
(data/
  reimu/
  marisa/
  cirno/)
  ```

*6.  Train the model*
```pythonn
python -m src.train
```



*Here are some examples of heatmap using Grad-CAM*:

## 博丽灵梦 (Hakurei Reimu)  
**Reimu Grad-CAM Example**

![Reimu Grad-CAM](grad-cam_examples/Figure_Reimu_001.png)

---

## 雾雨魔理沙 (Kirisame Marisa)  
**Marisa Grad-CAM Example**

![Marisa Grad-CAM](grad-cam_examples/Figure_Marisa_003.png)

---

## 琪露诺 (Cirno)  
**Cirno Grad-CAM Example**

![Cirno Grad-CAM](grad-cam_examples/Figure_Cirno_011.png)






