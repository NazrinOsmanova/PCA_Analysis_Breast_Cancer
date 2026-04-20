# PCA_Analysis_Breast_Cancer

Bu layihədə **Breast Cancer Wisconsin (Diagnostic) Dataset** istifadə edilərək, **PCA (Principal Component Analysis)** metodu ilə xərçəng xəstəliyi nəticələrinin vizual ayrılması həyata keçirilmişdir.

Dataset: [Kaggle – Breast Cancer Wisconsin Dataset](https://www.kaggle.com/datasets/uciml/breast-cancer-wisconsin-data)

---

## Layihənin Məqsədi

Layihənin əsas məqsədi, xəstələrin analiz nəticələrini və tibbi qeydlərini istifadə edərək **bədxassəli (Malignant) və xoşxassəli (Benign) xərçəng xəstələrini PCA nəticəsi ilə vizual olaraq ayırmaqdır**.

---

## Addımlar

1. **Tələb olunan kitabxanaların idxalı**  
   Python kitabxanaları: `pandas`, `numpy`, `scikit-learn`, `matplotlib`.

2. **Datasetin Google Colab-a əlavə edilməsi**  
   Kaggle-dan yüklənən `data.csv` faylı Colab mühitinə əlavə edilir.

3. **Lazımsız sütunların çıxarılması**  
   `id` və `diagnosis` kimi analitik üçün vacib olmayan sütunlar datasetdən çıxarılır.

4. **Missing value-lərin median ilə əvəzlənməsi**  
   Datasetdə mövcud olan boş dəyərlər median dəyərlərlə tamamlanır.

5. **Datanın standartlaşdırılması**  
   `StandardScaler` istifadə edilərək bütün feature-lar eyni ölçü miqyasına gətirilir.

6. **Datasetin ölçüsünün 2 komponentə qədər azaldılması**  
   PCA metodu ilə dataset 2 əsas komponentə qədər azaldılır.

7. **Nəticənin vizuallaşdırılması**  
   - `PC1` və `PC2` əsasında scatter plot yaradılır.  
   - Mavi nöqtələr → Benign (B) → xoşxassəli  
   - Qırmızı nöqtələr → Malignant (M) → bədxassəli

8. **PCA komponentlərinin özündə nə qədər informasiya saxladığı müəyyənləşdirilir**  
   - `PC1` → 44.27% informasiya  
   - `PC2` → 18.97% informasiya  
   - Cəmi → ~63.2% informasiya iki komponentdə saxlanılıb

---

## Nəticə

PCA nəticəsində **iki qrup bir-birindən vizual olaraq ayrılıb**, yəni PCA bu ədədi feature-larla xəstələri qismən ayırmağa imkan verir. Bu analiz xəstələrin bədxassəli və xoşxassəli olmasını vizual təhlil üçün effektiv üsuldur.

---

## İstifadə

1. Colab-da notebook-u açın.  
2. Dataset-i yükləyin.  
3. Addımları ardıcıl olaraq işə salın.  
4. Scatter plot və PCA komponentlərinin məlumat paylanmasını müşahidə edin.

---

## Lisensiya

Bu layihə təhsil məqsədli istifadə üçündür.
