# hse_hw2_chip

Ссылка на Google Colab: https://colab.research.google.com/drive/1r6UkS9vF3_KdZ2Sa3OuXEHlZbww16XYo?usp=sharing

Для задания была выбрана клеточная линия - **MCF-7**, гистоновая метка - **H2AFZ**:

## Анализ Fastq

Для начала был сделан fastqc для одного из ChIP-seq(**ENCFF081DDG.fastq**):

После подрезания, стало, конечно, лучше...

Было:

<p float="left">
  <img src="/pictures/1cs-p4.png" width="350" />
  <img src="/pictures/1cs-p1.png" width="350" />
  <img src="/pictures/1cs-p2.png" width="350" />
  <img src="/pictures/1cs-p3.png" width="350" />
</p>

Стало:

<p float="left">
  <img src="/pictures/1cst-p4.png" width="350" />
  <img src="/pictures/1cst-p1.png" width="350" />
  <img src="/pictures/1cst-p2.png" width="350" />
  <img src="/pictures/1cst-p3.png" width="350" />
</p>

После был сделан fastqc для одного из ChIP-seq(**ENCFF565MIO.fastq**):

Вообще не особо нужно было делать подрезание, но после очевидно стало лучше...

Было:

<p float="left">
  <img src="/pictures/2ch-p1.png" width="350" />
  <img src="/pictures/2ch-p2.png" width="350" />
  <img src="/pictures/2ch-p3.png" width="350" />
  <img src="/pictures/2ch-p4.png" width="350" />
</p>

Стало:

<p float="left">
  <img src="/pictures/2cst-p1.png" width="350" />
  <img src="/pictures/2cht-p2.png" width="350" />
  <img src="/pictures/2cht-p3.png" width="350" />
  <img src="/pictures/2cht-p4.png" width="350" />
</p>

Насчет файла контроля (**ENCFF640MKX.fastq**):

Тут все хорошо, думаю тут не имеет смысла делать подрезание...

<p float="left">
  <img src="/pictures/3cst-p1.png" width="350" />
  <img src="/pictures/3cst-p2.png" width="350" />
  <img src="/pictures/3cst-p3.png" width="350" />
  <img src="/pictures/3cst-p4.png" width="350" />
</p>

## Выравнивание на хромосому

Таблица со статистикой по каждому из 3 образцов:

<img src="/pictures/table.png" width="800" />


```
Q: Почему процент выравниваний получился именно таким?
A:
```

## Cравнение результатов

Диаграммы Венна:


<p float="left">
  <img src="/pictures/d_venna1.png" width="400" />
  <img src="/pictures/d_venna2.png" width="400" />
</p>

```
Q: Как можно объяснить различия в количестве пересечений?
A: Различия появляются, потому что сначала мы накладываем одни участки на другие, 
а потом вторые на первые... 
```

