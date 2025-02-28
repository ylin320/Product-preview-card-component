# Frontend Mentor - Product preview card component solution

This is a solution to the [Product preview card component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/product-preview-card-component-GO7UmttRfa). Frontend Mentor challenges help you improve your coding skills by building realistic projects.

這是 Frontend Mentor 上產品預覽卡片元件挑戰的解決方案。Frontend Mentor 的挑戰通過構建真實的項目來幫助提升編碼技能。

## Table of contents 目錄

- [Overview 總覽](#overview)
  - [The challenge 挑戰內容](#the-challenge)
  - [Screenshot 截圖](#screenshot)
  - [Links 連結](#links)
- [My process 我的過程](#my-process)
  - [Built with 使用技術](#built-with)
  - [What I learned 學習心得](#what-i-learned)
  - [Continued development 持續發展](#continued-development)
  - [Useful resources 有用資源](#useful-resources)
- [Author 作者](#author)

## Overview 總覽

### The challenge 挑戰內容

Users should be able to:
使用者應該能夠：

- View the optimal layout depending on their device's screen size
  根據設備螢幕大小查看最佳佈局
- See hover and focus states for interactive elements
  看到互動元素的懸停和焦點狀態

### Screenshot 截圖

[Add your screenshots here]
[在此添加截圖]

Desktop view 桌面版視圖:
![](./screenshot-desktop.jpg)

Mobile view 移動版視圖:
![](./screenshot-mobile.jpg)

### Links 連結

- Solution URL 解決方案網址: [Add solution URL here]
- Live Site URL 實際網站網址: [Add live site URL here]

## My process 我的過程

### Built with 使用技術

- Semantic HTML5 markup 語義化 HTML5 標記
- CSS custom properties CSS 自定義屬性
- Flexbox 彈性盒子佈局
- Mobile-first workflow 移動優先工作流程
- BEM naming methodology BEM 命名方法論

### What I learned 學習心得

This project was my first attempt at implementing a mobile-first approach. Here are some key learnings:
這個項目是我第一次嘗試實施移動優先方法。以下是一些主要的學習心得：

Using CSS custom properties for consistent theming:
使用 CSS 自定義屬性實現一致的主題設置：

```css
:root {
  /* Colors 顏色 */
  --color-green-500: hsl(158, 36%, 37%);
  --color-green-700: hsl(158, 42%, 18%);
  /* Typography 排版 */
  --font-family-montserrat: "Montserrat", sans-serif;
  --font-family-fraunces: "Fraunces", serif;
}
```

Implementing responsive images using the picture element:
使用 picture 元素實現響應式圖片：

```html
<picture class="card-image">
  <source
    srcset="./images/image-product-desktop.jpg"
    media="(min-width: 650px)"
  />
  <img
    src="./images/image-product-mobile.jpg"
    alt="Gabrielle Essence Eau De Parfum"
  />
</picture>
```

Creating a responsive layout with flexbox:
使用 flexbox 創建響應式佈局：

```css
.card {
  display: flex;
  flex-direction: column;
}

@media only screen and (min-width: 650px) {
  .card {
    flex-direction: row;
  }
}
```

### Continued development 持續發展

In future projects, I want to focus on:
在未來的項目中，我想專注於：

- Implementing better accessibility features
  實現更好的無障礙功能
- Exploring CSS Grid for more complex layouts
  探索 CSS Grid 實現更複雜的佈局
- Optimizing performance with responsive images
  優化響應式圖片的性能
- Improving CSS organization and architecture
  改進 CSS 組織和架構
- Learning more about CSS animations and transitions
  學習更多關於 CSS 動畫和過渡效果

### Useful resources 有用資源

- [A Complete Guide to Flexbox](https://css-tricks.com/snippets/css/a-guide-to-flexbox/) - This helped me understand flexbox layout concepts. The visual examples were particularly helpful.
  這幫助我理解了 flexbox 佈局概念。視覺示例特別有幫助。
- [CSS Custom Properties Guide](https://developer.mozilla.org/en-US/docs/Web/CSS/Using_CSS_custom_properties) - Excellent resource for understanding CSS variables and their usage.
  理解 CSS 變量及其用法的優秀資源。
- [Mobile-First CSS](https://www.mobileresponsive.io/blog/mobile-first-css) - Great article explaining the benefits and implementation of mobile-first approach.
  很好的文章，解釋了移動優先方法的好處和實施方式。

## Author 作者

- Frontend Mentor - [@yourusername](https://www.frontendmentor.io/profile/yourusername)
- GitHub - [@yourusername](https://github.com/yourusername)
