# Directroy Structure


## Rails

- 使用框架：Rails

- `assets/stylesheets/`: 所有的CSS在Rails中會放在這個下面，所以以下提到的資料夾也會這樣

- `pages/` : 各個desktop頁面的CSS

- `mobile/` : 各個手機版頁面的CSS

> pages, mobile底下頁面命名的原則依照頁面對應的controller action。
> 比如說company的show頁面就是`company_show.scss.css`，
> CSS中最外層就是名字當成id，如上例就是 `#company_show`

- `components/` : 各個會重複利用的元件的CSS(對應每一頁的客製化會在各頁面的CSS去做)