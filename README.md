# Price Range Forecast of House :house_with_garden:

## ＊ Introduction ＊
1. use `customers' house browsing history` to `predict price range of houses` that customers will `click on next`.

## ＊ Process ＊
1. **[ Construct dataset ]**
	1. Used K-means to understand the price distribution of houses browsed by customers, and sorted out the following three kinds of fields.
	2. `Fields of dataset:`
		-  `Basic information of houses:` price, age, size, etc.
		-  `The road section or administrative district where the house is located:`  represents the house price range that customers are interested in.
		-  `Browsing history of customers:` explore customers' preferred room type and learn its behavior pattern in order to predict the house item that the customer will click next accurately.
                
                
2. **[ Build Models & Predict house price range ]**
	1. `Forecast` house price range of `next click based on` the data of customers' `previous two clicks`.
	2. `Models:` deep neural network, convolutional neural network, long short-term memory.
	3. `Metrics of evaluating models' performance :` mean squared error, mean absolute error.
	4. After the model predicts house price of customers' next click, I will `calculate` the `predicted price range with the custom error rate`, and analyze whether the real prices are included in the prediction interval through the accuracy rate.
	5. `Error rate:` the difference between the real price and the predicted price of next click expressed in percentage. `Accuracy rate:` the ratio of the real price of next click falling within the predicted price range.

## ＊ Results ＊
1. `LSTM` performed the `best`, and the obtained `accuracy rate` was `64.1%`.

------

# 瀏覽房價預測 :camping:

## ＊ 簡介 ＊
1. 利用`顧客`的`房屋物件瀏覽歷史`，`預測`顧客`下一次點擊的房屋所處的價格區間`。

## ＊ 流程 ＊
1. **[ 建置資料集 ]**
	1. 先透過K-means瞭解顧客所瀏覽的房價分佈範圍，並加以整理出以下三種欄位。
	2. `資料欄位：`
		- `房屋物件之基本資訊：`房價、屋齡、坪數等。
		- `房屋物件所在之路段或行政區：`代表顧客偏好的房屋價格區間。
		- `顧客瀏覽歷史：`探索顧客感興趣之房型和學習其行為模式，以助模型預測顧客下一次欲點擊之房屋物件。
                
2. **[ 訓練模型 & 預測房價區間 ]**
	1. 以`前兩筆`瀏覽資料`預測下一筆`瀏覽資料之房屋價格範圍。
	2. `模型：` 深度神經網路、卷積神經網路以及長短期記憶模型。
	3. `評估模型表現指標：`均方誤差、平均絕對誤差。
	4. 模型預測出顧客下一次點擊之房價後，會再`以自定義之error rate計算出預測房價區間`，並透過accuracy rate分析真實房價是否落在預測區間內。
	5. `error rate：`下一次點擊之真實房價和預測房價之差異百分比。`accuracy rate：`下一次點擊之真實房價落在預測房價區間內之比率。

## ＊ 結果 ＊
1. `LSTM模型表現最好`，且獲得`64.1%`的`準確率`。
