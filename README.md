# Steps

1. Create the project with [Vite](https://vitejs.dev/guide/)

```bash
npm create vite@latest vite-swip-react -- --template react
```

2. Add [swipper](https://swiperjs.com/react)

```bash
npm install swiper
```

3. Import demo from docs:
```js
import { Swiper, SwiperSlide } from 'swiper/react';
import 'swiper/swiper.css';

function App () {

  return (
    <>
      <Swiper
        spaceBetween={50}
        slidesPerView={1}
        onSlideChange={() => console.log('slide change')}
        onSwiper={(swiper) => console.log(swiper)}
        style={{ backgroundColor: 'red', height: '100vh' }}
      >
        <SwiperSlide>Slide 1</SwiperSlide>
        <SwiperSlide>Slide 2</SwiperSlide>
        <SwiperSlide>Slide 3</SwiperSlide>
        <SwiperSlide>Slide 4</SwiperSlide>
      </Swiper >
    </>
  )
}

export default App
```

## React + Vite

This template provides a minimal setup to get React working in Vite with HMR and some ESLint rules.

Currently, two official plugins are available:

- [@vitejs/plugin-react](https://github.com/vitejs/vite-plugin-react/blob/main/packages/plugin-react/README.md) uses [Babel](https://babeljs.io/) for Fast Refresh
- [@vitejs/plugin-react-swc](https://github.com/vitejs/vite-plugin-react-swc) uses [SWC](https://swc.rs/) for Fast Refresh
