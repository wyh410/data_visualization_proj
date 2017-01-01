# data_visualization_proj
我的作品主題為「世界各國城市土地面積及人口數」，我所要呈現的資料就是各個國家的城市所占總土地面積，以及居住在這些城市裡的人口數。  
資料來源為The World Bank網站，其中各國城市面積取自 http://data.worldbank.org/indicator/AG.LND.TOTL.UR.K2?end=2010&start=1990 ，由於最新資料時間為2010年，且觀察與1990年之資料內容並無太大的差異，因此推測各國城市面積在近年來並無太大的變化，選擇呈現2010年之資料並不會太過時；城市人口數則取自 http://data.worldbank.org/indicator/SP.URB.TOTL?end=2015&start=2010 ，配合土地面積資料而選擇2010年之資料內容。    

# 使用技術
我所使用的工具為D3.js，它是一套JavaScript的函式庫，D3的全名為Data-Driven Documents，亦即透過資料來驅動文件，且使用者能根據自己的需求作相當彈性的操作，對於資料視覺化是一項很好的輔助工具。  

# 設計流程
而考量到我所要呈現的主題之一是土地的面積，我決定要使用泡泡圖來呈現資料的內容，因為比起長條圖等，泡泡圖更能直接看出不同資料間相對的大小，讓讀者更方便聯想。且不同於一般常見的泡泡圖是圓形，我將泡泡圖的形狀改成正方形，除了展現創意，我也認為方塊泡泡圖更有陸塊的感覺，較貼近我所要呈現的資料視覺效果。方塊的大小呈現了不同土地面積的狀態，透過滑鼠懸浮在該方塊上方，即可看到確切的土地面積數值(單位為平方公里)。點擊國家的名稱則會另外呈現出居住在該面積的總人口數(單位為千)，讓讀者能夠在一張圖表中看到兩種資料的內容，並加入了動態的視覺效果，使得整個頁面更活潑。
