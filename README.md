
## CSSReactions

UI web development based on an extrapolation of the W3C Visual Formatting Model and component-based design. CSSR is a content independent naming pattern that allows one to efficiently develop browser compatible components and complex layouts. 

### Simple Modular Naming Convention For Complex UI

```
:root {
  --primary-1: #ffffff;
  --primary-2: #eeeeee;
  --primary-3: #d8d8d8;
  --color-magenta: #f50057;
  --color-blue: #2196F3;
  --color-green: #00c853;
  --color-yellow: #ffd600;
  --color-default: #56596f;
  --color-bg: #37474f;
  --color-line: #37474f;
  --line-height: 40px;
  --line-height-large: 50px;
  --height-large: 50px;
  --color-border: #eeeeee;
  --border-radius: 21px;
  --border-width: 2px;
  --input-background-color: transparent;
  --input-border-color: #d8d8d8;
  --input-shadow: none;
}

*,
*:before,
*:after {
  box-sizing: border-box;
}

* {
  padding: 0;
  margin: 0;
}

html,
body {
  /* height: 100%; */
}

html {
  font-size: 16px;
}

body {
  font-family: 'Roboto', sans-serif;
  color: var(--color-default);
  font-size: 1rem;
  line-height: 1.5;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  background-color: #1c2542;
  width: 100%;
  overflow-x: hidden;
  -webkit-tap-highlight-color: transparent;
}

a {
  text-decoration: none;
  outline: none;
  color: var(--color-blue);
  -webkit-tap-highlight-color: transparent;
}

a:hover {
  text-decoration: none;
  color: var(--color-magenta);
}

img {
  max-width: 100%;
  height: auto;
}

.if__base-wrapper {
  display: inline-flex;
}

.ib__base-wrapper {
  display: inline-block;
}

[class*="base-wrapper"] {
  position: relative;
  padding: 20px 0;
  margin: 0;
  width: 100%;
}

.flex__mid-container {
  display: flex;
}

.block__mid-container {
  display: block;
}

[class*="mid-container"] {
  position: relative;
  margin-left: auto;
  margin-right: auto;
  padding-left: 20px;
  padding-right: 20px;
  width: 100%;
}

.if__content-panel {
  display: inline-flex;
}

.flex__content-panel {
  display: -webkit-flex;
  display: -ms-flexbox;
  display: flex;
}

.ib__content-panel {
  display: inline-block;
}

.block__content-panel {
  display: block;
}

[class*="content-panel"] {
  position: relative;
  margin: 0;
  padding: 0;
  height: auto;
}

.display-flex {
  display: flex !important;
}

.display-inline-flex {
  display: inline-flex !important;
}

.display-block {
  display: block !important;
}

.display-inline-block {
  display: inline-block !important;
}

.vertical-inline-flex {
  position: relative;
  display: inline-flex;
  flex-direction: column;
  width: 100%;
}

.horizontal-inline-flex {
  position: relative;
  display: inline-flex;
  width: 100%;
}

.layer-inline-block {
  position: relative;
  display: inline-block;
  width: 100%;
  float: left;
}

.layer-block {
position: relative;
width: 100%;
float: left;
}

.direction--row { flex-direction: row }
.direction--column { flex-direction: column }
.flex--no-wrap { flex-wrap: nowrap; }
.flex--wrap { flex-wrap: wrap; }
.justify--center { justify-content: center; }
.justify--space-between { justify-content: space-between; }
.justify--space-around { justify-content: space-around; }
.justify--flex-start { justify-content: flex-start; }
.justify--flex-end { justify-content: flex-end; }
.align--flex-start { align-items: flex-start; }
.align--flex-end { align-items: flex-end; }
.align--center { align-items: center; }
.align--baseline { align-items: baseline; }
.align--stretch { align-items: stretch; }
.align-self--auto { align-self: auto; }
.align-self--start { align-self: flex-start; }
.align-self--end { align-self: flex-end; }
.align-self--center { align-self: center; }
.align-self--baseline { align-self: baseline; }
.align-self--stretch { align-self: stretch; }

.float-l { float: left; }
.float-r { float: right; }



.transform--center {
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
}

.transform--top-center {
  position: absolute;
  top: 50%;
  transform: translateY(-50%);
}

.transform--right-center {
  position: absolute;
  top: 50%;
  right: 0;
  transform: translate(0%, -50%);
}

.transform--left-center {
  position: absolute;
  top: 50%;
  left: 0;
  transform: translate(0%, -50%);
}


@media screen and (max-width: 960px) {
  .column-under--960 {
  flex-direction: column !important;
}

.hide--under-960 {
  isplay: none !important;
}

.w-100-perc--under-960 {
  width: 100% !important;
  }
}
```

