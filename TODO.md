
    <header class="page-header"  
        role="banner">
      <h1 id="project-name"></h1>
    </header>
    <main id="content" class="main-content" role="main">
      {% include navigation.html %}
      <h2>{{ page.title }}</h2>
      <section>
        {{ content }}
      </section>
      <footer class="site-footer">
        &copy; 2022 ~ WEzSet
      </footer>
    </main>
    <!-- Global site tag (gtag.js) - Google Analytics --><!--
    <script async src="https://www.googletagmanager.com/gtag/js?id=UA-218058024-1"></script>
    <script>
      window.dataLayer = window.dataLayer || [];
      function gtag(){dataLayer.push(arguments);}
      gtag('js', new Date());
      
      gtag('config', 'UA-218058024-1');
    </script>-->

@import "modularscale@3.*";
@import "neat@4.*";
@import "bourbon@5.*";
@import "color-schemer";
@import "breakpoint";
@import "susy";
/* setiings */
/* free to use */
$element-background-color: #444243;
$element-text-color: white;
$border-raiud: 16px;
$breakp1: 40px;

@mixin res-border-radius($value, $breakpoint) {
  & {
    border-radius: #{"max(0px, min(#{$value}, 100% - #{$breakpoint} + 1px) * 9999) / #{$value}"};
  }
}

* {
  color: $element-text-color;
  border-radius: 5px;
}
.page-header {
  background: $element-background-color;
}
p {
  margin: 5px;
  color: LightGreen;
  background-color: #4f1818;
  border-radius: 10px 3px 3px 12px;
  border: 5px;
  font-family: monospace;
}
#error {
  margin: 0;
  color: red;
  background-color: black;
  position: relative;
  left: 10px;
  border-radius: 0;
  text-align: center;
}
#code-text {
  text-align: left;
  margin: 0;
  color: green;
  background-color: black;
  border-radius: 0;
}
#warning {
  text-align: center;
  color: red;
}
body {
  margin: 0;
  background: linear-gradient(312deg, #0600ff, #111032);
  background-size: 400% 400%;

  /*-webkit-animation: movegradient 2s ease infinite;
    -moz-animation: movegradient 2s ease infinite;
    animation: movegradient 2s ease infinite;*/
}

.css-selector {
  background: linear-gradient(312deg, #0600ff, #111032);
  background-size: 400% 400%;

  -webkit-animation: movegradient 0.5s ease infinite;
  -moz-animation: movegradient 0.5s ease infinite;
  animation: movegradient 0.5s ease infinite;
}

@-webkit-keyframes movegradient {
  0% {
    background-position: 0% 14%;
  }
  50% {
    background-position: 100% 87%;
  }
  100% {
    background-position: 0% 14%;
  }
}
@-moz-keyframes movegradient {
  0% {
    background-position: 0% 14%;
  }
  50% {
    background-position: 100% 87%;
  }
  100% {
    background-position: 0% 14%;
  }
}
@keyframes movegradient {
  0% {
    background-position: 0% 14%;
  }
  50% {
    background-position: 100% 87%;
  }
  100% {
    background-position: 0% 14%;
  }
}

h2 {
  color: green;
  font-size: 30px;
  background-color: yellow;
  opacity: 50%;
}
