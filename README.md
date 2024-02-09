# House-Property-Sales---Time-Series-Analysis-and-Forecasting

<h3>Source Dataset: https://www.kaggle.com/htagholdings/property-sales </h3>

## Overview

Project ini menggunakan <b>ARIMA dan SARIMA model</b> untuk meramalkan rata-rata harga rumah satu tahun ke depan. Model terbaik dipilih berdasarkan <b>akurasi terbaik atau Mean Absolute Percentage Error (MAPE) terendah.</b> Project ini juga melakukkan Adfuller test dan menunjukkan autocorellation plot dan partial autocorrelation plot untuk original time-series, deseasonal time-series, dan time-series yang telah di-differencing. 

## Summary

### Bussiness Insight

Dari project ini, dapat disimpulkan bahwa rata-rata harga rumah terus meninggi dengan berjalannya waktu. Pada bagian model. SARIMA lebih baik daripada ARIMA dalam memprediksi time series ini, yang dapat diartikan bahwa komponen seasonal cukup penting dalam memprediksi rata-rata harga rumah. Untuk ringkasan hasilnya dapat dilihat di bawah ini, sedangkan untuk lengkapnya dapat dilihat di [notebook ini](https://github.com/Stev-create/House-Property-Sales---Time-Series-Analysis-and-Forecasting/blob/master/House%20Property%20Sales.ipynb).

### Dataset

![GitHub Logo](/images/1.png)

![GitHub Logo](/images/10.png)

![GitHub Logo](/images/11.png)


#### Time series decomposition

![GitHub Logo](/images/7.png)

Terlihat dari komponen trendnya, bahwa rata-rata harga rumah terus meninggi seiringnya berjalan dengan waktu. Dan terdapat pola di komponen seasonal setiap tahunnya. 


### Splitting Dataset 

#### Original Time Series

![GitHub Logo](/images/2.png)

#### Deseasonal Time Series

![GitHub Logo](/images/3.png)

Untuk melihat autocorrelation plot dan partial autocorrelation plotnya dapat dilihat di [notebook ini](https://github.com/Stev-create/House-Property-Sales---Time-Series-Analysis-and-Forecasting/blob/master/House%20Property%20Sales.ipynb)

### ARIMA dan SARIMA 

Pada ARIMA tidak terlalu terlihat peramalan yang signifikan, mengingat hasilnya hanya memberi kita garis lurus:

![GitHub Logo](/images/4.png)

Itu kenapa pada ARIMA punya <b>Mean Absolute Percentage Error (MAPE)</b> yang sangat besar. Sedangkan SARIMA memiliki MAPE yang kecil hanya sekitar 4% dan ini hasilnya:

![GitHub Logo](/images/6.png)

Dan untuk diagnostic modelnya sudah diperlihatkan di notebook. 

### Predictions

Saya mencoba memprediksi dalam jangka waktu 1 tahun menggunakan SARIMA (Yang dimana SARIMA adalah model yang lebih baik daripada ARIMA dalam kasus ini).

![GitHub Logo](/images/pred.png)


### Thank You

