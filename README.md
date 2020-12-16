# -Nintendo-Switch-eShop-API-
 Nintendo Switch eShop API 
 
 
 
### 港区所有游戏列表 Game Full List HK
https://www.nintendo.com.hk/data/json/switch_software.json

### 日区所有游戏列表 Game Full List JP
https://www.nintendo.co.jp/data/software/xml/switch.xml

### 打折游戏列表 Discounting Game List
#### 日区 Japanese：  
https://ec.nintendo.com/api/JP/ja/search/sales?count=30&offset=0  

#### 英语区 English：  
https://ec.nintendo.com/api/US/en/search/sales?count=30&offset=0  
https://ec.nintendo.com/api/GB/en/search/sales?count=10&offset=0  
https://ec.nintendo.com/api/CA/en/search/sales?count=30&offset=0#Canada  
https://ec.nintendo.com/api/AU/en/search/sales?count=10&offset=0#Australia  
https://ec.nintendo.com/api/NZ/en/search/sales?count=10&offset=0#NewZealand  
https://ec.nintendo.com/api/CZ/en/search/sales?count=10&offset=0#Czech  
https://ec.nintendo.com/api/DK/en/search/sales?count=10&offset=0#Denmark  
https://ec.nintendo.com/api/FI/en/search/sales?count=10&offset=0#Finland  
https://ec.nintendo.com/api/GR/en/search/sales?count=10&offset=0#Greece  
https://ec.nintendo.com/api/HU/en/search/sales?count=10&offset=0#Hungary  
https://ec.nintendo.com/api/NO/en/search/sales?count=10&offset=0#Norway  
https://ec.nintendo.com/api/PL/en/search/sales?count=10&offset=0#Poland  
https://ec.nintendo.com/api/ZA/en/search/sales?count=10&offset=0#SouthAfrica  
https://ec.nintendo.com/api/SE/en/search/sales?count=10&offset=0#Sweden  

#### 德语区 German：  
https://ec.nintendo.com/api/DE/de/search/sales?count=10&offset=0  
https://ec.nintendo.com/api/CH/de/search/sales?count=10&offset=0#Switzerland  

#### 法语区 French：  
https://ec.nintendo.com/api/FR/fr/search/sales?count=10&offset=0  
https://ec.nintendo.com/api/BE/fr/search/sales?count=10&offset=0#Belgium  

#### 意大利 Italian：  
https://ec.nintendo.com/api/IT/it/search/sales?count=10&offset=0  

#### 荷兰 Dutch：  
https://ec.nintendo.com/api/NL/nl/search/sales?count=10&offset=0  
https://ec.nintendo.com/api/BE/nl/search/sales?count=10&offset=0#Belgium  

#### 俄区 Russian：  
https://ec.nintendo.com/api/RU/ru/search/sales?count=30&offset=0  

#### 西语区 Spanish：  
https://ec.nintendo.com/api/ES/es/search/sales?count=30&offset=0  
https://ec.nintendo.com/api/MX/es/search/sales?count=30&offset=0#Mexico  
https://ec.nintendo.com/api/CO/es/search/sales?count=10&offset=0#Columbia  
https://ec.nintendo.com/api/AR/es/search/sales?count=10&offset=0#Argentina  
https://ec.nintendo.com/api/CL/es/search/sales?count=10&offset=0#Chile  
https://ec.nintendo.com/api/PE/es/search/sales?count=10&offset=0#Peru  

#### 葡语区 Portuguese：  
https://ec.nintendo.com/api/PT/pt/search/sales?count=30&offset=0  
https://ec.nintendo.com/api/BR/pt/search/sales?count=10&offset=0  

#### 亚洲区 Asian：  
https://ec.nintendo.com/api/HK/zh/search/sales?count=10&offset=0  
https://ec.nintendo.com/api/KR/ko/search/sales?count=10&offset=0  

#### Return
- contents: array
  - content_type: string
  - disclaimer: string
  - dominant_colors: string[]
  - formal_name: string
  - hero_banner_url: string
  - id: number
  - is_new: boolean
  - public_status: string
  - release_date_on_eshop: string
  - strong_disclaimer: string
  - tags: array
  - target_titles: array
- length: number
- offset: number
- total: number

### 游戏价格查询 Game Price Query
https://api.ec.nintendo.com/v1/price?country=JP&ids=70010000009922&lang=jp  

#### Return
- personalized: boolean
- country: string
- prices: array
    - title_id: number,
    - sales_status: string
    - regular_price:
       - amount: string
       - currency: string
       - raw_value: string
    - discount_price:
       - amount: string
       - currency: string
       - raw_value: string
       - start_datetime: date
       - end_datetime: date

### 最新发售游戏列表 Latest Released Game List
https://ec.nintendo.com/api/JP/ja/search/new?count=30&offset=0  

### 下载游戏排行 Downloading Game Ranking
https://ec.nintendo.com/api/JP/ja/search/ranking?count=10&offset=0  

### 游戏详情 Game Details
view-source:https://ec.nintendo.com/JP/ja/titles/70010000012325  

### Game
  - title
    - cn
    - jp
    - en
  - cover_url
  - prices: array
      - sales_status: string
      - regular_price:
        - amount: string
        - currency: string
        - raw_value: string
      - discount_price:
        - amount: string
        - currency: string
        - raw_value: string
        - start_datetime: date
        - end_datetime: date
  - release_date
  - categories
  - publisher
  - developer
  - language_availability
  - total_rom_size
  - players_from
  - players_to
  - screenshots

