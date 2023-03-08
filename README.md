# [Horizontal Parallax](https://8panteon8.github.io/horizontalParallax/)

With [Swiper.js](https://swiperjs.com) implemented a beautiful website template with horizontal scrolling 

## It is important to pay attention

- **Setting Swiperjs**

```javascript
  speed: 2400,
  mousewheel: {
    enabled: true,
    sensitivity: 2.4,
  },
  spaceBetween: 18,
  parallax: true,
```

- **Adding a percentage of parallax**
```html
data-swiper-parallax="20%"
```

- **Slide styling**
```css
.slider {
  height: 100%;
}

.slider__layer {
  position: absolute;
  inset: 0;
  background-size: cover;
  background-position: center;
}
```

- **For horizontal scrolling and dynamics like on a tipical site**

>paramete horizontal scrolling

```javascript
direction: 'vertical',
```

>paramete for a soft rabbit

```javascript
freeMode: true,
```

>Don't forget to add a transition, it must have an `!important` to override the transition  Swiper.js

```css
transition: 1.75s cubic-bezier(0.2, 0.6, 0, 1);
```

---

## If you want adding some item for slides

- **Add one more swiper for absolute position and connect them**

```javascript
swiperOne.controller.control = swiperTwo;
swiperTwo.controller.control = swiperOne;
```

You can read more about how do it in this [repository](https://github.com/8Panteon8/slider)

## Screenshot


![ezgif com-video-to-gif-2-2](https://user-images.githubusercontent.com/113831614/223845153-76132d90-2d5f-48f2-b8a3-926d69801cfc.gif)

