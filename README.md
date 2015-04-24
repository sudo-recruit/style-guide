# Style guide

- 目標：可以重複使用的stylesheet，讓之後改版盡可能無痛的轉換。

- 原則
    
    1. 減少巢狀、針對性的class、html tag

    2. 盡量把對style的調整都抽象出來變成一個class（以下稱unit class）

    3. 確定component使用上述的class組合不出來時，才使用特定的class去定義它的style

    4. 用unit class來定義

    5. 上述的component如果畫面上只會出現一次，使用id來定義它


-----

## Todo

- 決定z-index放哪

- text style的命名

- utility（常用的class）


-----

## Issue

- color如果也抽成unit class會不會過度抽象化


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

- 所有顏色的處理都放在這

-

### Word

- 包含font-size,
