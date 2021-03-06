# Style guide

- 目標：可以重複使用的stylesheet，讓之後改版盡可能無痛的轉換。

- 原則
    
    1. 減少巢狀、針對性的class、html tag

    2. 盡量把對style的調整都抽象出來變成一個class（以下稱unit class）

    3. 確定component使用上述的class組合不出來時，才使用特定的class去定義它的style

    4. 用unit class來定義

    5. 上述的component如果畫面上只會出現一次，使用id來定義它

-----

#### NOTE ：筆記區

- 如果最外層已經有id的話，除非__有必要__，否則盡量不要再增加class來指定element，使用原生的html tag去調整

    - 優點：較乾淨的html view

    - 缺點：要想一下再寫

    - 結論：其實要想一下再去寫雖然會多花一些開發時間，但是長期看下來會寫出較好維護html。例外的情況就是這個element內部有一個非常複雜的component要指定，就可以考慮多給一個class、或是id。

- 上述情況，如果考慮到button等可能會需要加入event的地方，可以有以下選項：

    - 讓front-end自己加上id
    
    - 一開始就做好一個id當接口給他

-----

## Todo

- 調整box padding或margin的地方，垂直用px(命名地方用數字)，水平用percentage

- 在html裡面擺放的順序

- 決定`text-align`放在哪裡

- range在doc說明的表現方式()

- 決定`z-index`放哪

- text style的命名

- utility（常用的class）




-----

## Issue

- color如果也抽成unit class會不會過度抽象化


-----

## HTML

- 放置class的順序 `position` > `width` > `height` >

## CSS style

- 註解的地方全部用大寫英文

-----

## 各類型stylesheet

### Box

- 參考名稱：`box.css.scss`

- 包含`width`, `height`, `margin`, `padding`的處理都依照這裡的guide走


- Width
    
    - `.w-100` ~ `.w-10` : 寬度，單位是%，從100%~10%。

    - `.vw-100` ~ `.vw-10` : 單位是vw，從100vw~10vw。

- Height

    - `.h-100` ~ `.h-10` : 高度，單位是%，從100%~10%。

    - `.vh-100` ~ `.vh-10` : 單位是vh，從100vh~10vh。

- Margin 

    - `.margin-t-100`(top), `.margin-r-100`(right), `.margin-b-100`(bottom), 
    `.margin-l-100`(left) ~ `.margin-t-5`(top), `.margin-r-5`(right), `.margin-b-5`(bottom), `.margin-l-5`(left)

- Padding

    - `.padding-t-100`(top), `.padding-r-100`(right), `.padding-b-100`(bottom), 
    `.padding-l-100`(left) ~ `.padding-t-5`(top), `.padding-r-5`(right), `.padding-b-5`(bottom), `.padding-l-5`(left)


### Color

- color.css.scss

- 所有顏色的處理都放在這


### Image

- image.css.scss

- 跟照片有關的處理會放在這，包括filter

- Brightness

    - 

### Word

- 包含font-size letter-spacing

