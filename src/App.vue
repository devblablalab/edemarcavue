<template>
  <div class="p-content">
    <HeaderBrand></HeaderBrand>
    <div class="col">
       <ProjectBrand></ProjectBrand>
       <ShirtGif></ShirtGif>
    </div>
  </div>
  <BrandList></BrandList>
</template>

<script>
import HeaderBrand from './components/HeaderBrand.vue';
import ProjectBrand from './components/ProjectBrand.vue';
import ShirtGif from './components/ShirtGif.vue';
import BrandList from './components/Brand/BrandList.vue';

export default {
    name: "App",
    components: { HeaderBrand, ProjectBrand, ShirtGif, BrandList }
}
</script>

<style>
:root {
  --muted:#7C7C7C;
  --light : #FFF;
  --dark: #222;
}

html, body, div, span, applet, object, iframe,
h1, h2, h3, h4, h5, h6, p, blockquote, pre,
a, abbr, acronym, address, big, cite, code,
del, dfn, em, img, ins, kbd, q, s, samp,
small, strike, strong, sub, sup, tt, var,
b, u, i, center,
dl, dt, dd, ol, ul, li,
fieldset, form, label, legend,
table, caption, tbody, tfoot, thead, tr, th, td,
article, aside, canvas, details, embed, 
figure, figcaption, footer, header, hgroup, 
menu, nav, output, ruby, section, summary,
time, mark, audio, video {
	margin: 0;
	padding: 0;
	border: 0;
	font-size: 100%;
	font: inherit;
	vertical-align: baseline;
}

article, aside, details, figcaption, figure, 
footer, header, hgroup, menu, nav, section {
	display: block;
}

body {
	line-height: 1;
}

ol, ul {
	list-style: none;
}

blockquote, q {
	quotes: none;
}

blockquote:before, blockquote:after,
q:before, q:after {
	content: '';
	content: none;
}

table {
	border-collapse: collapse;
	border-spacing: 0;
}

a {
  text-decoration: none;
  color: unset;
}

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
}

.col {
  display: flex;
  flex-direction: column;
  align-items: center;
}

.p-content {
  padding: 1.4em;
}

.fw-bold {
  font-weight: bold;
}

.flex-1 {
  flex: 1;
}

.flex-2 {
  flex: 2;
}
</style>
