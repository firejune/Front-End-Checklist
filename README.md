<h1 align="center">
<br>
  <img src="https://raw.githubusercontent.com/thedaviddias/Front-End-Checklist/master/src/img/banners/logo-front-end-checklist.jpg" alt="프론트엔드 체크리스트" width="170">
  <br>
    <br>
  프론트엔드 체크리스트
  <br>
</h1>

<h4 align="center">프론트엔드 체크리스트는 당신의 HTML 사이트 또는 페이지를 프로덕션으로 런칭하기 이전에 가지고 있어야 할, 또한 테스트 되어야 할 전반적인 요소들의 집합입니다.</h4>

<p align="center">
  <a href="http://makeapullrequest.com">
    <img src="https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square" alt="PRs Welcome">
  </a>
  <a href="https://gitpod.io/#https://github.com/thedaviddias/Front-End-Checklist">
  <img src="https://img.shields.io/badge/Gitpod-Ready--to--Code-blue?logo=gitpod" alt="Gitpod Ready-to-Code">
  </a>
    <a href="https://github.com/thedaviddias/Front-End-Checklist/graphs/contributors">
    <img src="https://img.shields.io/github/contributors/thedaviddias/Front-End-Checklist.svg?style=flat-square" alt="Contributors">
  </a>
  <a href="https://spectrum.chat/front-end-checklist">
    <img src="https://img.shields.io/badge/chat-on_spectrum-4837E2.svg?style=flat-square" alt="Spectrum">
  </a>
      <a href="https://github.com/thedaviddias/Front-End-Checklist/">
    <img src="https://img.shields.io/badge/Front‑End_Checklist-followed-brightgreen.svg?style=flat-square" alt="Front‑End_Checklist followed">
</a>
    <a href="https://creativecommons.org/publicdomain/zero/1.0/">
    <img src="https://img.shields.io/badge/license-CC0-green.svg?style=flat-square" alt="CC0">
  </a>
</p>

<p align="center">
  <a href="#how-to-use">How To Use</a> • <a href="#contributing">Contributing</a> • <a href="https://frontendchecklist.io">Website</a> • <a href="https://www.producthunt.com/posts/front-end-checklist">Product Hunt</a>
</p>
<p align="center">
    <span>Other Checklists:</span>
    <br>
  <a href="https://github.com/thedaviddias/Front-End-Performance-Checklist#---------front-end-performance-checklist-">🎮 Front-End Performance Checklist</a> • <a href="https://github.com/thedaviddias/Front-End-Design-Checklist#front-end-design-checklist">💎 Front-End Design Checklist</a>
</p>

이 리스트는 다년간의 프론트엔드 개발자들의 경험으로 작성되었으며, 몇몇 항목들은 타 오픈소스 체크리스트들의 참고를 통해 추가되었습니다.

## 목차

1. **[Head](#head)**
2. **[HTML](#html)**
3. **[웹폰트](#웹폰트)**
4. **[CSS](#css)**
5. **[이미지](#이미지)**
6. **[자바스크립트](#자바스크립트)**
7. **[보안](#보안)**
8. **[성능](#성능-1)**
9. **[접근성](#접근성)**
10. **[SEO](#seo)**

---

## 이 리스트는 어떻게 사용하나요?

**프론트엔드 체크리스트**에 속해있는 모든 항목들은 대다수의 프로젝트에서 필요로 하는 사항들이지만, 몇몇 요소들은 생략되거나 필수적이 아닐 수도 있습니다(예를 들면 관리형 웹 어플리케이션의 경우 RSS 피드는 필요 없을 것입니다). 우리는 따라서 각각의 항목들을 3가지의 기준으로 구분하였습니다:

* ![Low][low_img] 의 경우 해당 항목이 **권유** 되지만, 몇몇 특정한 상황에서는 생략될 수도 있습니다.
* ![Medium][medium_img] 의 경우 해당 항목이 **권고** 되지만, 굉장히 특정한 상황에서는 결국 생략이 될 수도 있습니다. 몇몇 요소의 경우, 생략 시 성능이나 SEO 측면에서 안 좋은 영향을 끼칠 수도 있습니다.
* ![High][high_img] 의 경우 해당 항목은 어떠한 상황에서라도 **생략될 수 없습니다**. 이를 생략하게 되면 당신의 페이지는 오동작하거나 접근, 또는 SEO에 문제가 발생할 것입니다. 이러한 요소들에 대해서 우선적으로 테스트 하시기 바랍니다.


몇몇 추가 내용들은 그것들이 어떠한 종류의 내용인지 이해하는데에 도움을 주기 위하여 이모티콘을 추가하였습니다. 이로 인해 체크리스트에서 해당 항목들을 이해하는 데에 도움이 될 것입니다:

* 📖: 문서 또는 기사
* 🛠: 온라인 도구 / 테스트 도구
* 📹: 미디어 또는 비디오 컨텐츠

> 당신은 [README_APP 파일](https://github.com/thedaviddias/Front-End-Checklist/blob/master/README_APP.md)에서 프로젝트에 대한 모든 것을 설명하는 ***프론트엔드 체크리스트 앱***에 기여햘 수 있습니다.

---

## Head

> **노트:** [a list of everything](https://github.com/joshbuchea/HEAD) 에서 HTML 문서 내의 `<head>` 에서 사용할 수 있는 모든 것을 찾아보실 수 있습니다.

### 메타 태그

* [ ] **Doctype:** ![High][high_img] HTML5 을 사용하며, Doctype이 모든 HTML 페이지의 최상단에 위치함

```html
<!doctype html> <!-- HTML5 -->
```

> * 📖 [문자 인코딩 결정하기 - HTML5 W3C](https://www.w3.org/TR/html5/syntax.html#determining-the-character-encoding)

*다음 2개의 메타 태그(Charset과 Viewport)들은 다른 요소들에 비해 head 안에서도 상단에 위치해야만 합니다.*

* [ ] **Charset:** ![High][high_img] 문자집합(UTF-8)이 올바르게 선언됨

```html
<!-- 이 문서에 대한 문자 인코딩을 설정 -->
<meta charset="utf-8">
```

* [ ] **Viewport:** ![High][high_img] Viewport가 제대로 선언됨

```html
<!-- 반응형 웹 디자인을 위한 Viewport 설정 -->
<meta name="viewport" content="width=device-width, initial-scale=1, viewport-fit=cover">
```

* [ ] **Title:** ![High][high_img] 모든 페이지에 title이 사용됨 (SEO 가이드: Google은 제목에 사용된 글자들의 너비의 픽셀 값을 계산한 뒤, 472~482px 사이의 값으로 잘라냅니다. 평균적인 글자 길이의 제한은 약 55개의 글자입니다.)

```html
<!-- 문서의 Title -->
<title>55개 이하의 문자로 구성된 페이지 제목</title>
```

> * 📖 [Title - HTML - MDN](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/title)
> * 🛠 [SERP Snippet Generator](https://www.sistrix.com/serp-snippet-generator/)

* [ ] **Description:** ![High][high_img] description이 제대로 기재됨 (설명값은 고유해야 하며, 150개 이하의 문자로 구성되어야 함)

```html
<!-- Meta Description -->
<meta name="description" content="페이지에 대한 설명 (150개 이하의 문자)">
```

> * 📖 [Meta Description - HTML - MDN](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/The_head_metadata_in_HTML#Adding_an_author_and_description)

* [ ] **Favicons:** ![Medium][medium_img] 각각의 favicon이 제대로 생성되었고 올바르게 보여지는가? 만약 `favicon.ico` 파일만 가지고 있다면, 해당 내용을 페이지의 상단부에 추가하라. 일반적으로는 해당 태그를 사용할 필요는 없지만, 아래의 예시를 포함하는 것이 좋은 습관임. 오늘날에는 `.ico` 포맷보다 **PNG 포맷의 아이콘 사용을 추천**함(크기: 32x32px).

```html
<!-- 표준 favicon -->
<link rel="icon" type="image/x-icon" href="https://example.com/favicon.ico">
<!-- 추천 favicon 포맷 -->
<link rel="icon" type="image/png" href="https://example.com/favicon.png">
```

> * 🛠 [Favicon Generator](https://www.favicon-generator.org/)
> * 🛠 [RealFaviconGenerator](https://realfavicongenerator.net/)
> * 📖 [Favicon Cheat Sheet](https://github.com/audreyr/favicon-cheat-sheet)
> * 📖 [Favicons, Touch Icons, Tile Icons, etc. Which Do You Need? - CSS Tricks](https://css-tricks.com/favicon-quiz/)
> * 📖 [PNG favicons - caniuse](https://caniuse.com/#feat=link-icon-png)

* [ ] **Apple 웹앱 메타:** ![Low][low_img] Apple에만 유효한 메타-태그

```html
<!-- Apple 터치 아이콘 (최소한 200x200 px) -->
<link rel="apple-touch-icon" href="/custom-icon.png">

<!-- To run web application in full-screen -->
<meta name="apple-mobile-web-app-capable" content="yes">

<!-- Status Bar Style (see Supported Meta Tags below for available values) -->
<!-- Has no effect unless you have the previous meta tag -->
<meta name="apple-mobile-web-app-status-bar-style" content="black">
```

> * 📖 [웹 어플리케이션 설정하기](https://developer.apple.com/library/content/documentation/AppleApplications/Reference/SafariWebContent/ConfiguringWebApplications/ConfiguringWebApplications.html)
> * 📖 [Meta Tags 지원하기](https://developer.apple.com/library/content/documentation/AppleApplications/Reference/SafariHTMLRef/Articles/MetaTags.html)

- [ ] **윈도우 타일:** ![Low][low_img] 윈도우 타일에만 유효하게 연결됨

```html
<!-- Microsoft 타일 -->
<meta name="msapplication-config" content="browserconfig.xml" />
```

`browserconfig.xml` 파일에서 사용되는 최소한의 XML 내용은 다음과 같습니다:

```xml
<?xml version="1.0" encoding="utf-8"?>
<browserconfig>
   <msapplication>
     <tile>
        <square70x70logo src="small.png"/>
        <square150x150logo src="medium.png"/>
        <wide310x150logo src="wide.png"/>
        <square310x310logo src="large.png"/>
     </tile>
   </msapplication>
</browserconfig>
```

> * 📖 [브라우저 설정 스키마 레퍼런스](https://msdn.microsoft.com/en-us/library/dn320426(v=vs.85).aspx)

* [ ] **Canonical:** ![Medium][medium_img] 컨텐츠의 중복을 피하기 위하여 `rel="canonical"` 을 사용함

```html
<!-- 컨텐츠 중복 문제 방지 -->
<link rel="canonical" href="http://example.com/2017/09/a-new-article-to-read.html">
```

> * 📖 [표준 URL을 사용하기 - Search Console Help - Google Support](https://support.google.com/webmasters/answer/139066?hl=en)
> * 📖 [rel=canonical을 사용할 때 흔히 겪는 5가지 실수 - Google Webmaster Blog](https://webmasters.googleblog.com/2013/04/5-common-mistakes-with-relcanonical.html)

### HTML 태그
* [ ] **언어 속성:** ![High][high_img] 현재 페이지 내의 언어에 알맞게 속성 값이 부여됨
```html
<html lang="ko">
```

* [ ] **글자 방향 속성:** ![Medium][medium_img] 글자들의 방향이 제대로 설정됨 (우리나라에서는 좌에서 우로 글씨를 읽고 쓰지만 몇몇 나라에서는 우에서 좌로 읽고 쓰는 경우도 있음)

```html
<html dir="rtl">
```

> * 📖 [dir - HTML - MDN](https://developer.mozilla.org/en-US/docs/Web/HTML/Global_attributes/dir)

* [ ] **대체 언어:** ![Low][low_img] 현재 페이지를 언어에 맞게 대체할 수 있는 태그 속성 값을 사용함

```html
<link rel="alternate" href="https://en.example.com/" hreflang="en">
```

* [ ] **조건부 주석:** ![Low][low_img] Internet Explorer 를 위한 조건부 주석을 사용함

> * 📖 [조건부 주석에 관하여 (Internet Explorer) - MSDN - Microsoft](https://msdn.microsoft.com/en-us/library/ms537512(v=vs.85).aspx)

* [ ] **RSS 피드:** ![Low][low_img] 만일 페이지가 블로그이거나 기사가 있다면, RSS 링크에 대해 확인하시오

* [ ] **CSS Critical:** ![Medium][medium_img] 페이지가 로딩되는 즉시(펼쳐지는 그 순간) 컨텐츠에 영향을 끼치는 CSS를 "critical CSS" 라고 함. 이는 당신의 실질적인 어플리케이션의 CSS 가 로딩되기 이전에 `<style></style>` 태그 사이에 최소화 된 상태로 한 줄로 추가되어 임베딩 됨

> * 🛠 [Critical by Addy Osmani on Github](https://github.com/addyosmani/critical) 이 레포는 CSS Critical을 자동화 하는데에 도움을 줍니다.

* [ ] **CSS의 순서:** ![High][high_img] 모든 CSS 파일이 `<head>` 내에서 자바스크립트 파일보다 이전에 로딩이 완료됨 (자바스크립트 파일이 비동기적으로 로딩되는 특정한 경우는 제외함).

### 소셜 메타
Visualize and generate automatically our social meta tags with [Meta Tags](https://metatags.io/)

***Facebook OG*** and ***Twitter Cards*** are, for any website, highly recommended. The other social media tags can be considered if you target a particular presence on those and want to ensure the display.

* [ ] **Facebook Open Graph:** ![Low][low_img] 모든 Facebook의 Open Graph (OG) 가 테스트 되었으며, 그것들 중에 누락된 정보나 잘못된 정보를 가지고 있지는 않나? (이미지의 경우 최소한 600 x 315 픽셀은 되어야 하며, 1200 x 630 픽셀 크기를 권장함)

> **노트:** `og:image:width`와 `og:image:height` 를 사용하는 것은 이미지의 크기를 웹 크롤러에게 알려주어서, 이미지를 비동기적으로 다운로드하고 처리할 필요 없이 즉시 보여줄 수 있도록 합니다.

```html
<meta property="og:type" content="website">
<meta property="og:url" content="https://example.com/page.html">
<meta property="og:title" content="Content Title">
<meta property="og:image" content="https://example.com/image.jpg">
<meta property="og:description" content="Description Here">
<meta property="og:site_name" content="Site Name">
<meta property="og:locale" content="en_US">
<!-- 다음의 태그는 필수는 아니지만, 포함하는 것을 추천함 -->
<meta property="og:image:width" content="1200">
<meta property="og:image:height" content="630">
```

> * 📖 [웹마스터를 위한 쉐어링 가이드](https://developers.facebook.com/docs/sharing/webmasters/)
> * 📖 [쉐어링 - 모범 사례](https://developers.facebook.com/docs/sharing/best-practices/)
> * 🛠 [Facebook OG testing](https://developers.facebook.com/tools/debug/) 도구를 이용하여 당신의 페이지 테스트하기

* [ ] **Twitter Card:** ![Low][low_img]

```html
<meta name="twitter:card" content="summary">
<meta name="twitter:site" content="@site_account">
<meta name="twitter:creator" content="@individual_account">
<meta name="twitter:url" content="https://example.com/page.html">
<meta name="twitter:title" content="Content Title">
<meta name="twitter:description" content="Content description less than 200 characters">
<meta name="twitter:image" content="https://example.com/image.jpg">
```

> * 📖 [Twitter cards 시작하기 — Twitter Developers](https://developer.twitter.com/en/docs/tweets/optimize-with-cards/guides/getting-started)
> * 🛠 [Twitter card 검사기](https://cards-dev.twitter.com/validator) 도구를 이용하여 당신의 페이지 테스트하기

**[⬆ 목차로](#목차)**

---

## HTML

### 모범 사례

* [ ] **HTML5 시맨틱 엘리먼트:** ![High][high_img] HTML5의 시맨틱 엘리먼트들이 적절히 사용됨 (header, section, footer, main... 등).

> * 📖 [HTML 레퍼런스](http://htmlreference.io/)

* [ ] **에러 페이지:** ![High][high_img] 에러를 위한 404 페이지와 5xx 페이지가 존재하는가? 5xx 페이지는 서버로부터의 데이터를 전송받지 않고 독립적인 자체 CSS를 포함하고 있어야 함을 기억하라 (5xx 에러는 서버 에러이므로!).

* [ ] **Noopener:** ![Medium][medium_img] 외부 링크를 `target="_blank"`를 이용하여 연 경우, [tab nabbing 피싱 공격](https://blog.coderifleman.com/2017/05/30/tabnabbing_attack_and_noopener/)을 방지하기 위하여 `rel="noopener"` 속성을 사용해야만 한다. 만약 Firefox 옛 버전을 지원해야만 한다면, `rel="noopener noreferrer"` 을 사용하라.

> * 📖 [rel=noopener에 대하여](https://mathiasbynens.github.io/rel-noopener/)

* [ ] **주석 지우기:** ![Low][low_img] 웹사이트를 프로덕션 하기 이전에 불필요한 코드는 제거하였는지, 주석은 제거하였는지 점검하라

### HTML testing

* [ ] **W3C 규격:** ![High][high_img] 모든 페이지는 HTML 코드 내에서 일어날 수 있는 경우를 확인하기 위하여 W3C 의 validator를 이용하여 테스트 되어야 함

> * 🛠 [W3C 검사기](https://validator.w3.org/)

* [ ] **HTML Lint:** ![High][high_img] 도구를 이용하여 HTML 코드 내에 발생할 수 있는 문제들을 분석하도록 하자

> * 🛠 [Dirty markup](https://dirtymarkup.com/): HTML 코드를 정돈해주는 온라인 도구

> * 🛠 [Sonar a linting tool for the web](https://sonarwhal.com/)
* [ ] **Link checker:** ![High][high_img] 페이지 내에 깨진 링크는 없는지, 404 에러가 존재하지 않는지 다시 한번 확인하도록 함

> * 🛠 [W3C Link Checker](https://validator.w3.org/checklink)

* [ ] **광고차단기 테스트:** ![Medium][medium_img] 광고차단기가 활성화 된 상태에서도 컨텐츠가 제대로 보여짐 (사람들에게 광고차단기를 비활성화 해달라고 메세지를 알릴수도 있습니다)

> * 📖 [Use AdBlocking in your Dev Environment](https://andreicioara.com/use-adblocking-in-your-dev-environment-48db500d9b86)

**[⬆ 목차로](#목차)**

---

## 웹폰트

> **노트:** 웹폰트를 사용하면 스타일링 되지 않은 글자나 보이지 않는 글자들이 깜빡일 수 있습니다. 실패했을 경우를 대비한 대체용 폰트를 포함하거나, 웹폰트 로더를 활용하여 이러한 동작들을 제어하세요.
> * 📖 [구글의 웹폰트에 대한 기술적 고려사항](https://developers.google.com/fonts/docs/technical_considerations)

* [ ] **웹폰트 포맷:** ![High][high_img] WOFF, WOFF2 와 TTF는 모든 최신 브라우저에서 지원됨

> * 📖 [WOFF - Web Open Font Format - Caniuse](https://caniuse.com/#feat=woff).
> * 📖 [WOFF 2.0 - Web Open Font Format - Caniuse](https://caniuse.com/#feat=woff2).
> * 📖 [TTF/OTF - TrueType and OpenType font support](https://caniuse.com/#feat=ttf)
> * 📖 [Using @font-face - CSS-Tricks](https://css-tricks.com/snippets/css/using-font-face/)

* [ ] **웹폰트 크기:** ![High][high_img] 모든 종류(이탤릭, 볼드체 등등)를 포함한 웹폰트 크기의 총 합계는 2 MB를 넘지 않도록 함

* [ ] **웹폰트 로더:** ![Low][low_img] 웹폰트 로더를 이용하여 폰트가 로딩되는 동작을 제어하시오

> * 🛠 [Typekit 웹폰트 로더](https://github.com/typekit/webfontloader)

**[⬆ 목차로](#목차)**

---

## CSS

> **노트:** 대다수의 프론트엔드 개발자들이 따르는 [CSS 가이드라인](https://cssguidelin.es/)과 [Sass 가이드라인](https://sass-guidelin.es/) 을 살펴보세요. 만약 모르는 CSS 속성 값이 있다면, [CSS 레퍼런스](http://cssreference.io/)를 참조하길 바랍니다. 또한 CSS의 일관성을 위한 [코드 가이드](http://codeguide.co/)도 읽어보기 바랍니다.

* [ ] **반응형 웹 디자인:** ![High][high_img] 웹사이트가 반응형으로 디자인 됨
* [ ] **CSS Print:** ![Medium][medium_img] 프린터가 사용할 print 스타일시트 값이 설정되었고, 각각의 페이지마다 올바르게 설정됨
* [ ] **CSS 전처리기:** ![Medium][medium_img] 디자인에 CSS 전처리기를 이용함 (추천: [Sass](http://sass-lang.com/)).
* [ ] **고유 ID값:** ![High][high_img] 여러 개의 ID 값이 사용된 경우, 각각의 ID 값은 페이지 내에 고유해야함
* [ ] **Reset CSS:** ![High][high_img] 최신의 Reset CSS (reset, normalize나 reboot) 이 사용됨 *(Bootstrap이나 Foundation 같은 CSS 프레임워크를 사용할 경우, Normalize가 이미 포함되어 있음)*

> * 📖 [Reset.css](https://meyerweb.com/eric/tools/css/reset/)
> * 📖 [Normalize.css](https://necolas.github.io/normalize.css/)
> * 📖 [Reboot](https://getbootstrap.com/docs/4.0/content/reboot/)

* [ ] **JS 접두사:** ![Low][low_img] **js**-로 시작하는 자바스크립트 파일 내에서 사용되는 모든 클래스나 ID는 CSS 파일에서 스타일링 되지 않도록 함

```html
<div id="js-slider" class="my-slider">
<!-- 또는 -->
<div id="id-used-by-cms" class="js-slider my-slider">
```

* [ ] **CSS 임베딩 또는 인라인:** ![High][high_img] 어떠한 경우에도 CSS를 직접 임베딩하거나 인라인으로 사용하지 마시오! 타당한 이유가 있는 경우에만 사용하시오 (예: 슬라이더 내의 background-image, 또는 CSS critical)
* [ ] **벤더 프리픽스:** ![High][high_img] CSS 벤더 프리픽스들이 사용되었고 브라우저 지원 호환성에 따라 알맞게 생성되었는지 확인

> * 🛠 [Autoprefixer CSS online](https://autoprefixer.github.io/)

### 성능

- [ ] **파일 단일화:** ![High][high_img] CSS 파일들이 하나의 CSS 파일로 단일화 되었음 *(HTTP/2의 경우는 여러 개의 파일을 사용하는 것이 더 성능에 좋음)*
- [ ] **최소화:** ![High][high_img] 모든 CSS 파일들이 최소화 됨
- [ ] **Non-blocking:** ![Medium][medium_img] CSS 파일들은 DOM이 로딩하는데에 방해가 되지 않도록 비동기적으로 로드 되어야 함

> * 📖 [loadCSS by filament group](https://github.com/filamentgroup/loadCSS)
> * 📖 [Example of preload CSS using loadCSS](https://gist.github.com/thedaviddias/c24763b82b9991e53928e66a0bafc9bf)

- [ ] **사용하지 않은 CSS:** ![Low][low_img] 사용되지 않은 CSS는 제거함

> * 🛠 [UnCSS Online](https://uncss-online.com/)
> * 🛠 [PurifyCSS](https://github.com/purifycss/purifycss)
> * 🛠 [PurgeCSS](https://github.com/FullHuman/purgecss)
> * 🛠 [Chrome DevTools Coverage](https://developers.google.com/web/updates/2017/04/devtools-release-notes#coverage)


### CSS 테스트

* [ ] **Stylelint:** ![High][high_img] 모든 CSS와 SCSS 파일들에 아무런 에러가 없는지 확인

> * 🛠 [stylelint, a CSS 린터](https://stylelint.io/)
> * 📖 [Sass 가이드라인](https://sass-guidelin.es/)

* [ ] **반응형 웹 디자인:** ![High][high_img] 모든 페이지가 다음 지점에서 테스트 완료되었음: 320px, 768px, 1024px (그 외 당신이 필요한 크기에 따라 다를 수 있음)

* [ ] **CSS 검사기:** ![Medium][medium_img] CSS가 제대로 테스트 되었고, 오류들이 알맞게 수정되었음

> * 🛠 [CSS 검사기](https://jigsaw.w3.org/css-validator/)

* [ ] **데스크탑 브라우저:** ![High][high_img] 모든 페이지가 모든 현존하는 데스크탑 브라우저에서 테스트 됨 (Safari, Firefox, Chrome, Internet Explorer, EDGE... 등).
* [ ] **모바일 브라우저:**  ![High][high_img] 모든 페이지가 모든 현존하는 모바일 브라우저에서 테스트 됨 (Native browser, Chrome, Safari... 등).
* [ ] **운영체제:**  ![High][high_img] 모든 페이지가 모든 현존하는 운영체제에서 테스트 됨 (Windows, Android, iOS, Mac... 등).

- [ ] **디자인 충실도:** ![Low][low_img] 창작물에서 의도했던 디자인 품질에 가까워야 함, 일부 도구를 사용하여 코드 구현과 비교하고 일관성을 보장할 수 있음.

> [Pixel Perfect - Chrome 확장도구](https://chrome.google.com/webstore/detail/perfectpixel-by-welldonec/dkaagdgjmgdmbnecmcefdhjekcoceebi?hl=en)

* [ ] **글자 방향:** ![High][high_img] 다국어를 지원해야 할 경우, 글자 방향에 맞게 모든 페이지가 정상 동작함 (LTR / RTL)

> * 📖 [Building RTL-Aware Web Apps & Websites: Part 1 - Mozilla Hacks](https://hacks.mozilla.org/2015/09/building-rtl-aware-web-apps-and-websites-part-1/)
> * 📖 [Building RTL-Aware Web Apps & Websites: Part 2 - Mozilla Hacks](https://hacks.mozilla.org/2015/10/building-rtl-aware-web-apps-websites-part-2/)

**[⬆ 목차로](#목차)**

---

## 이미지

> **노트:** 이미지 최적화의 완전한 이해를 위해서는, Addy Osmani가 쓴 무료 ebook **[Essential Image Optimization](https://images.guide/)** 을 확인하세요.

### 모범 사례

* [ ] **최적화:** ![High][high_img] 모든 이미지가 브라우저에 렌더링 될 수 있도록 최적화 되었나? 홈페이지 같이 성능이 중요한 페이지에는 WebP 포맷을 사용할 수도 있음

> * 🛠 [Imagemin](https://github.com/imagemin/imagemin)
> * 🛠 [ImageOptim](https://imageoptim.com/)를 사용하여 당신의 이미지를 무료로 최적화하세요.
> * 🛠 [KeyCDN Image Processing](https://www.keycdn.com/support/image-processing)를 사용하여 실시간으로 이미지를 최적화하세요.
> * 🛠 [Kraken.io](https://kraken.io/web-interface)를 사용하여 png와 jpg을 꽤나 대단하게 최적화 할 수 있습니다. 파일 당 1MB에 대해서는 무료입니다.
> * 🛠 [TinyPNG](https://tinypng.com/) png, apng(애니메이션 png)와 jpg 이미지를 손실없이 최적화합니다. 무료 및 유료 버전 있음
> * 🛠 [ZorroSVG](http://quasimondo.com/ZorroSVG/) svg 마스킹을 사용하여 투명 이미지, jpg와 같은 압축
> * 🛠 [SVGO](https://github.com/svg/svgo) SVG 벡터 그래픽 파일을 최적화 하기 위한 Nodejs기반 도구.
> * 🛠 [SVGOMG](https://jakearchibald.github.io/svgomg/) SVGO의 온라인 웹기반 GUI 버전, svg 파일 최적화

* [ ] **Picture/Srcset:** ![Medium][medium_img] picture와 srcset을 이용하여 사용자의 현재 뷰포트에 가장 적합한 이미지를 제공하였음

> * 📖 [srcset을 사용하여 반응형 이미지 만드는 방법](https://www.sitepoint.com/how-to-build-responsive-images-with-srcset/)

* [ ] **레티나 디스플레이 지원:** ![Low][low_img] 레티나 디스플레이를 지원하기 위하여 당신의 현 레이아웃에 해당하는 2배, 또는 3배 이상 큰 이미지를 지원함
* [ ] **[이미지 스프라이트](https://www.w3schools.com/css/css_image_sprites.asp):** ![Medium][medium_img] 작은 이미지의 경우 스프라이트 파일로 구성되어져 있음 (아이콘의 경우, SVG 스프라이트 이미지 일 수도 있음).
* [ ] **너비와 높이:** ![High][high_img] 모든 `<img>` 태그에 너비와 높이가 설정되었음 (px이나 %로 지정하지 마시오)
* [ ] **대체 텍스트:** ![High][high_img] 모든 `<img>` 태그가 이미지를 잘 서술하는 대체 텍스트를 가지고 있음 (`alt` 속성으로 부여)

> * 📖 [대체 텍스트: 최고의 가이드](https://axesslab.com/alt-texts/)

* [ ] **Lazy 로딩:** ![Medium][medium_img] 이미지들이 lazy 로드 됨 (자바스크립트 미지원에 대한 예외처리가 항상 제공 되어야 함)

**[⬆ 목차로](#목차)**

---

## 자바스크립트

### 모범 사례

* [ ] **인라인 자바스크립트:** ![High][high_img] HTML 코드와 섞어 자바스크립트 코드를 인라인으로 포함하지 않도록 하시오
* [ ] **파일 단일화:** ![High][high_img] 자바스크립트 파일들이 하나의 자바스크립트 파일로 단일화 되었음
* [ ] **최소화:** ![High][high_img] 모든 자바스크립트 파일이 최소화 되었음(뒤에 `.min` 접미사를 붙이는 것을 추천)

> * [리소스(HTML, CSS, and JavaScript) 최소화하기](https://developers.google.com/speed/docs/insights/MinifyResources)

* [ ] **자바스크립트 보안:**

> * [자바스크립트를 활용하여 보안에 안전한 어플리케이션 개발 가이드라인](https://www.owasp.org/index.php/DOM_based_XSS_Prevention_Cheat_Sheet#Guidelines_for_Developing_Secure_Applications_Utilizing_JavaScript)*

* [ ] **`noscript` 태그:** ![Medium][medium_img] 브라우저 내에 자바스크립트를 지원하지 않거나 꺼져 있을 경우를 고려하여 HTML 내에 `<noscript>` 태그를 사용하시오. 이는 React.js 어플리케이션처럼 클라이언트 사이드에 렌더링이 굉장히 무거운 어플리케이션의 경우 굉장히 유용함. 다음의 [예제](https://webdesign.tutsplus.com/tutorials/quick-tip-dont-forget-the-noscript-element--cms-25498) 를 살펴보시오

```html
<noscript>
  이 어플리케이션을 실행시키기 위해선 자바스크립트를 활성화 시켜야 합니다.
</noscript>
```

* [ ] **Non-blocking:** ![Medium][medium_img] JavaScript 파일들은 `async`와 `defer` 속성값을 이용하여 비동기적으로 로드 되어야 함

> * 📖 [렌더링을 막는 자바스크립트 제거하기](https://developers.google.com/speed/docs/insights/BlockingJS)

* [ ] **Optimized and updated JS libraries:** ![Medium][medium_img] All JavaScript libraries used in your project are necessary (prefer Vanilla Javascript for simple functionalities), updated to their latest version and don't overwhelm your JavaScript with unnecessary methods.

> * 📖 [You may not need jQuery](http://youmightnotneedjquery.com/)
> * 📖 [Vanilla JavaScript for building powerful web applications](https://plainjs.com/)

* [ ] **Modernizr:** ![Low][low_img] 특정한 기능을 지칭하고 싶다면, 커스터마이징 된 Modernizr를 이용하여 `<html>` 태그 내에 클래스들을 추가할 수 있음

> * 🛠 [당신의 Modernizr 커스터마이징 하기](https://modernizr.com/download?setclasses)

### 자바스크립트 테스트

* [ ] **ESLint:** ![High][high_img] 표준 규칙이나 당신의 설정에 따라 ESLint를 에러 없이 통과함

> * 📖 [ESLint - 자바스크립트와 JSX를 위한, 언제든지 사용할 수 있는 린팅 유틸리티](https://eslint.org/)

**[⬆ 목차로](#목차)**

---

## 보안

### 당신의 웹사이트를 미리 검토하고 확인하세요

> * [securityheaders.io](https://securityheaders.io/)
> * [Observatory by Mozilla](https://observatory.mozilla.org/)

### 모범 사례

* [ ] **HTTPS:** ![Medium][medium_img] 페이지 내에 존재하는 모든 외부 컨텐츠(플러그인, 이미지...)에 대해서도 HTTPS 가 사용되었음.

> * 🛠 [Let's Encrypt - Free SSL/TLS Certificates](https://letsencrypt.org/)
> * 🛠 [Free SSL Server Test](https://www.ssllabs.com/ssltest/index.html)
> * 📖 [Strict Transport Security](http://caniuse.com/#feat=stricttransportsecurity)

* [ ] **HTTP Strict Transport Security (HSTS):** ![Medium][medium_img] HTTP 헤더 값으로 'Strict-Transport-Security'가 설정됨.

> * 🛠 [Check HSTS preload status and eligibility](https://hstspreload.org/)
> * 📖 [HSTS 참조서 - OWASP](https://www.owasp.org/index.php/HTTP_Strict_Transport_Security_Cheat_Sheet)
> * 📖 [전송 계층 보안 참조서 - OWASP](https://www.owasp.org/index.php/Transport_Layer_Protection_Cheat_Sheet)

* [ ] **사이트 간 요청 위조(CSRF; Cross Site Request Forgery):** ![High][high_img] CSRF 공격을 방지하기 위하여 위하여 당신의 서버 쪽으로 발생하는 모든 HTTP 요청이 합법적이고 당신의 웹사이트나 어플리케이션으로부터 발생한 것임을 확신함

> * 📖 [CSRF 예방 참조서 - OWASP](https://www.owasp.org/index.php/Cross-Site_Request_Forgery_(CSRF)_Prevention_Cheat_Sheet)

* [ ] **사이트 간 스크립팅(XSS; Cross Site Scripting):** ![High][high_img] 당신의 페이지나 웹사이트가 사이트 간 스크립팅이 발생할 여지가 전혀 없음

> * 📖 [XSS 예방 참조서 - OWASP](https://www.owasp.org/index.php/XSS_(Cross_Site_Scripting)_Prevention_Cheat_Sheet)
> * 📖 [DOM 기반 XSS 예방 참조서  - OWASP](https://www.owasp.org/index.php/DOM_based_XSS_Prevention_Cheat_Sheet)

* [ ] **Content Type Options:** ![Medium][medium_img] Prevents Google Chrome and Internet Explorer from trying to mime-sniff the content-type of a response away from the one being declared by the server.

> * 📖 [X-Content-Type-Options - Scott Helme](https://scotthelme.co.uk/hardening-your-http-response-headers/#x-content-type-options)

* [ ] **X-Frame-Options (XFO)** ![Medium][medium_img] 방문자를 클릭재킹 공격으로부터 보호함

> * 📖 [X-Frame-Options - Scott Helme](https://scotthelme.co.uk/hardening-your-http-response-headers/#x-frame-options)
> * 📖 [RFC7034 - HTTP Header Field X-Frame-Options](https://tools.ietf.org/html/rfc7034)

* [ ] **컨텐츠 보안 정책(CSP; Content Security Policy)** ![Medium][medium_img] 사이트 내의 컨텐츠가 어떻게 로딩되고, 어디서 로딩되도록 허가받았는지를 확인. 이를 적용함으로써 클릭재킹 공격을 방지할 수 있음

> * 📖 [컨텐츠 보안 정책 소개 - Scott Helme](https://scotthelme.co.uk/content-security-policy-an-introduction/)
> * 📖 [컨텐츠 보안 정책 가이드라인 - Scott Helme](https://scotthelme.co.uk/csp-cheat-sheet/)
> * 📖 [컨텐츠 보안 정책 가이드라인 - OWASP](https://www.owasp.org/index.php/Content_Security_Policy_Cheat_Sheet)
> * 📖 [컨텐츠 보안 정책 레퍼런스](https://content-security-policy.com/)

**[⬆ 목차로](#목차)**

---

## 성능

### 모범 사례

- [ ] **Goals to achieve:** ![Medium][medium_img] Your pages should reach these goals:
  - First Meaningful Paint under 1 second
  - Time To Interactive under 5 seconds for the "average" configuration (a $200 Android on a slow 3G network with 400ms RTT and 400kbps transfer speed) and under 2 seconds for repeat visits
  - Critical file size under 170Kb gzipped

> * 🛠 [웹사이트 페이지 분석](https://tools.pingdom.com)
> * 🛠 [웹페이지 테스트](https://www.webpagetest.org/)
> * 📖 [페이지 용량을 제한함으로써 웹을 더욱 가볍게 만드세요](https://evilmartians.com/chronicles/size-limit-make-the-web-lighter)

- [ ] **최소화:** ![Medium][medium_img] HTML이 최소화가 되었음

* [ ] **Lazy 로딩:** ![Medium][medium_img] 이미지, 스크립트, CSS 파일들이 lazy 로드 되어서 현 페이지의 응답시간을 향상시킴 (각 섹션의 자세한 부분을 참조하시오).

* [ ] **쿠키 크기:** 쿠키를 사용한다면, 각 쿠키의 크기가 4096 바이트를 넘지 않고, 도메인 내에 20개 이상의 쿠키를 가지지 않도록 주의하시오

> * 📖 [쿠키 사양: RFC 6265](https://tools.ietf.org/html/rfc6265)
> * 📖 [쿠키](https://developer.mozilla.org/en-US/docs/Web/HTTP/Cookies)
> * 🛠 [브라우저 쿠키의 제한점](http://browsercookielimits.squawky.net/)

* [ ] **서드 파티 컴포넌트:** ![Medium][medium_img] 공유하기 버튼처럼 외부 자바스크립트 파일에 의존하는 서드파티 iframe이나 컴포넌트의 경우, 가급적 정적인 컴포넌트로 교체하여서 외부 API 호출을 제한하고 사용자들의 활동들을 외부로 유출되지 않도록 하시오

> * 🛠 [간단한 공유하기 버튼 생성기](https://simplesharingbuttons.com/)

### 다음에 발생할 HTTP 요청을 미리 준비하기

> * 📖 [다음 기술들에 대한 설명](https://css-tricks.com/prefetching-preloading-prebrowsing/)

* [ ] **DNS resolution:** ![Low][low_img] DNS of third-party services that may be needed are resolved in advance during idle time using `dns-prefetch`.

```html
<link rel="dns-prefetch" href="https://example.com">
```

* [ ] **Preconnection:** ![Low][low_img] DNS lookup, TCP handshake and TLS negotiation with services that will be needed soon is done in advance during idle time using `preconnect`.

```html
<link rel="preconnect" href="https://example.com">
```

* [ ] **Prefetching:** ![Low][low_img] Resources that will be needed soon (e.g. lazy loaded images) are requested in advance during idle time using `prefetch`.

```html
<link rel="prefetch" href="image.png">
```

* [ ] **Preloading:** ![Low][low_img] Resources needed in the current page (e.g. scripts placed at the end of `<body>`) in advance using `preload`.

```html
<link rel="preload" href="app.js">
```

> * 📖 [prefetch와 preload의 차이점](https://medium.com/reloading/preload-prefetch-and-priorities-in-chrome-776165961bbf)

### 성능 테스트

* [ ] **Google PageSpeed:** ![High][high_img] 홈페이지 뿐 아니라 모든 페이지가 테스트 완료 되었고 최소한 100점 만점 90점은 획득하였음

> * 🛠 [Google PageSpeed](https://developers.google.com/speed/pagespeed/insights/)
> * 🛠 [Google에서 모바일 속도를 측정해보세요](https://testmysite.withgoogle.com)
> * 🛠 [WebPagetest - 웹사이트 성능 및 최적화 테스트](https://www.webpagetest.org/)
> * 🛠 [GTmetrix - 웹사이트 속도 및 성능 최적화](https://gtmetrix.com/)
> * 🛠 [Speedrank - 웹사이트 성틍 개선](https://speedrank.app/)

**[⬆ 목차로](#목차)**

---

## 접근성

> **노트:** 유튜브의 재생 목록을 확인해보세요 [A11ycasts with Rob Dodson](https://www.youtube.com/playlist?list=PLNYkxOF6rcICWx0C9LVWWVqvHlYJyqw7g) 📹

### 모범 사례

- [ ] **Progressive enhancement:** ![Medium][medium_img] 메인 네비게이션이나 검색과 같은 대다수의 기능들이 자바스크립트가 작동하지 않고도 동작해야 함

> * 📖 [Chrome 개발자 도구를 이용하여 자바스크립트 키고 끄기](https://www.youtube.com/watch?v=kBmvq2cE0D8)

- [ ] **색상 대비:** ![Medium][medium_img] 색상 대비 기준이 최소한 WCAG AA를 통과해야 함 (모바일의 경우 AAA를 통과해야 함)

> * 🛠 [대비율](https://leaverou.github.io/contrast-ratio/)

#### 헤딩

* [ ] **H1:** ![High][high_img] 모든 페이지 내에 웹사이트의 타이틀과 다른 H1 태그가 존재해야 함
* [ ] **헤딩:** ![High][high_img] 헤딩이 올바른 순서(H1부터 H6까지)로 적절히 사용되어야 함

> * 📹 [헤딩과 랜드마크가 그렇게 중요한 이유 -- A11ycasts #18](https://www.youtube.com/watch?v=vAAzdi1xuUY&index=9&list=PLNYkxOF6rcICWx0C9LVWWVqvHlYJyqw7g)

### 시맨틱

- [ ] **특정한 HTML5의 input 타입들의 사용:** ![Medium][medium_img] 이 항목은 각각 다른 input 타입에 대하여 개별적인 키패드나 위젯을 보여주는 모바일 장치들에 대해 특히 더욱 중요함

> * 📖 [모바일 Input 타입](http://mobileinputtypes.com/)

### 폼

* [ ] **레이블:** ![High][high_img] 레이블은 각각의 입력 폼 엘리먼트와 연관됨. 레이블이 보여질 수 없는 경우 `aria-label` 을 대신 사용하시오

> * 📖 [aria-label 속성 사용하기 - MDN](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/ARIA_Techniques/Using_the_aria-label_attribute)

### 접근성 테스트

* [ ] **접근성 표준 테스트:** ![High][high_img] WAVE 도구를 이용하여 당신의 페이지가 접근성 표준을 만족하였는지 테스트 해보세요

> * 🛠 [Wave 테스트](http://wave.webaim.org/)

* [ ] **키보드 네비게이션:** ![High][high_img] 키보드만을 이용하여 웹사이트를 예측 가능하도록 움직일 수 있는지 테스트 하시오. 모든 인터랙티브 엘리먼트들은 접근 가능하고 사용 가능해야 함
* [ ] **스크린 리더:** ![Medium][medium_img] 모든 페이지들이 스크린 리더 (VoiceOver, ChromeVox, NVDA or Lynx) 테스트를 완료함
* [ ] **포커스 스타일링:** ![High][high_img] 포커스 되지 않은 경우, 눈에 보이는 상태의 CSS로 대체되어야 함

> * 📹 [포커스 관리하기 - A11ycasts #22](https://www.youtube.com/watch?v=srLRSQg6Jgg&index=5&list=PLNYkxOF6rcICWx0C9LVWWVqvHlYJyqw7g)

**[⬆ 목차로](#목차)**

---

## SEO

* [ ] **구글 애널리틱스:** ![High][high_img] 구글 애널리틱스가 설치되었고 제대로 설정되었음

> * 🛠 [구글 애널리틱스](https://analytics.google.com/analytics/web/)
> * 🛠 [구글 애널리틱스 체커 (및...)](http://www.gachecker.com/)

* [ ] **적절한 제목 배치:** ![Medium][medium_img] 제목은 현 페이지의 내용을 이해하는 데에 도움을 줌

> * 🛠 [Tota11y, tab Headings](http://khan.github.io/tota11y/#Try-it)

* [ ] **sitemap.xml:** ![High][high_img] sitemap.xml 파일이 존재하고 Google Search Console(예전 이름: Google Webmaster Tools)으로 제출되었음

> * 🛠 [Sitemap 생성기](https://websiteseochecker.com/html-sitemap-generator/)

* [ ] **robots.txt:** ![High][high_img] robots.txt 파일이 웹페이지를 블록킹 하지 않음

> * 📖 [The robots.txt file](https://varvy.com/robottxt.html)
> * 🛠 [Google Robots 테스트 도구](https://www.google.com/webmasters/tools/robots-testing-tool)를 이용하여 당신의 robots.txt 파일을 테스트 해보세요

* [ ] **구조화 된 데이터:** ![High][high_img] 구조화 된 데이터를 사용하여 페이지가 테스트되었고 에러가 존재하지 않는가? 구조화 된 데이터는 웹 크롤러가 현 페이지 내의 컨텐츠를 이해하는 데에 도움이 됨

> * 📖 [구조화 된 데이터 소개 - Search - Google Developers](https://developers.google.com/search/docs/guides/intro-structured-data)
> * 📖 [RDFa - Linked Data in HTML](https://rdfa.info/)
> * 📖 [JSON-LD](https://json-ld.org/)
> * 📖 [Microdata](https://www.w3.org/TR/microdata/)
> * 🛠 [구조화 된 데이터 테스트 도구](https://developers.google.com/structured-data/testing-tool/)를 이용하여 당신의 페이지를 테스트 해보세요
> * 🛠 구조화 된 데이터로 사용될 수 있는 단어들의 목록을 만들어보세요 [Schema.org Full Heirarchy](http://schema.org/docs/full.html)

* [ ] **HTML 사이트맵:** ![Medium][medium_img] HTML 사이트맵이 제공되었으며 웹사이트의 푸터 내에 존재하는 링크를 통하여 접근이 가능함

> * 📖 [사이트맵 가이드라인 - Google Support](https://support.google.com/webmasters/answer/183668?hl=ko)

* [ ] **Pagination link tags:** ![Medium][medium_img] Provide `rel="prev"` and `rel="next"` to indicate paginated content.

> * 🛠 [Pagination (rel="prev/next") Testing Tool](https://technicalseo.com/seo-tools/rel-prev-next/)

> * 📖 [Pagination guidelines - Google Support](https://support.google.com/webmasters/answer/1663744?hl=en)

```html
<!-- Example: Pagination link tags for page 2 of a paginated list -->
<link rel="prev" href="https://example.com/?page=1">
<link rel="next" href="https://example.com/?page=3">
```

**[⬆ 목차로](#목차)**

---

## 번역

프론트엔드 체크리스트는 다른 언어로도 이용 가능합니다. 모든 번역자들과 그들의 멋진 노력에 감사합니다!

* 🇯🇵 Japanese: [miya0001/Front-End-Checklist](https://github.com/miya0001/Front-End-Checklist)
* 🇪🇸 Spanish: [eoasakura/Front-End-Checklist-ES](https://github.com/eoasakura/Front-End-Checklist-ES)
* 🇨🇳 Chinese: [JohnsenZhou/Front-End-Checklist](https://github.com/JohnsenZhou/Front-End-Checklist)
* 🇰🇷 Korean: [kesuskim/Front-End-Checklist](https://github.com/kesuskim/Front-End-Checklist)
* 🇧🇷 Portuguese: [jcezarms/Front-End-Checklist](https://github.com/jcezarms/Front-End-Checklist)
* 🇻🇳 Vietnamese: [euclid1990/Front-End-Checklist](https://github.com/euclid1990/Front-End-Checklist)
* 🇹🇼 Traditional Chinese: [EngineLin/Front-End-Checklist](https://github.com/EngineLin/Front-End-Checklist)
* 🇫🇷 French: [ynizon/Front-End-Checklist](https://github.com/ynizon/Front-End-Checklist)
* 🇷🇺 Russian: [ungear/Front-End-Checklist](https://github.com/ungear/Front-End-Checklist)
* 🇹🇷 Turkish: [eraycetinay/Front-End-Checklist](https://github.com/eraycetinay/Front-End-Checklist)
* 🇩🇪 German: [xfuture603/Front-End-Checklist](https://github.com/xFuture603/Front-End-Checklist)

---

## 프론트엔드 체크리스트 배지

만약 당신이 프론트엔드 체크리스트의 규칙을 따르고 있다고 보여주길 원한다면, 하단의 배지를 README 파일에 추가하세요!

➔ [![Front‑End_Checklist followed](https://img.shields.io/badge/Front‑End_Checklist-followed-brightgreen.svg)](https://github.com/thedaviddias/Front-End-Checklist/)

```md
[![Front‑End_Checklist followed](https://img.shields.io/badge/Front‑End_Checklist-followed-brightgreen.svg)](https://github.com/thedaviddias/Front-End-Checklist/)
```

**[⬆ 목차로](#목차)**

---

## 프로젝트에 기여

**이슈를 새로 생성하거나 PR을 날려서 수정 사항이나 추가할 부분에 대해 알려주세요.**

### 가이드

**프론트엔드 체크리스트** 레포지토리는 2개의 브랜치로 구성되어져 있습니다:

#### 1. `master`

이 브랜치는 [프론트엔드 체크리스트](http://frontendchecklist.com/) 웹사이트에 반영되는 `README.md`파일로 구성되어져 있습니다.

#### 2. `develop`

이 브랜치는 필요하다면 구조나 컨텐츠에 상당한 변화를 줄 수 있습니다. 간단한 에러 수정을 하거나 새로운 항목을 추가할 경우, master 브랜치에 직접 하는 것을 추천드립니다.

### Online Setup with a single Click

You can use gitpod ( A free VS Code like IDE) for contributing online, with a single click it will launch a ready to code workspace with all the dependencies pre-installed, build finished & the web server running so that you can start coding straight away.

[![Open in Gitpod](https://gitpod.io/button/open-in-gitpod.svg)](https://gitpod.io/#https://github.com/thedaviddias/Front-End-Checklist)

## Support

질문이나 제안이 있다면, 주저하지 말고 Gitter나 Twitter를 이용하세요:

* [Chat on Gitter](https://gitter.im/Front-End-Checklist/Lobby?utm_source=share-link&utm_medium=link&utm_campaign=share-link)
* [Facebook](https://www.facebook.com/frontendchecklist/)
* [Twitter](https://twitter.com/thedaviddias)

## 저자

**[David Dias](https://github.com/thedaviddias/Front-End-Checklist)**

## Contributors

This project exists thanks to all the people who contribute. [[Contribute]](CONTRIBUTING.md).
<a href="https://github.com/thedaviddias/Front-End-Checklist/graphs/contributors"><img src="https://opencollective.com/front-end-checklist/contributors.svg?width=890" /></a>


## Backers

Thank you to all our backers! 🙏 [[Become a backer](https://opencollective.com/front-end-checklist#backer)]

<a href="https://opencollective.com/front-end-checklist#backers" target="_blank"><img src="https://opencollective.com/front-end-checklist/backers.svg?width=890"></a>


## Sponsors

Support this project by becoming a sponsor. Your logo will show up here with a link to your website. [[Become a sponsor](https://opencollective.com/front-end-checklist#sponsor)]

<a href="https://opencollective.com/front-end-checklist/sponsor/0/website" target="_blank"><img src="https://opencollective.com/front-end-checklist/sponsor/0/avatar.svg"></a>
<a href="https://opencollective.com/front-end-checklist/sponsor/1/website" target="_blank"><img src="https://opencollective.com/front-end-checklist/sponsor/1/avatar.svg"></a>
<a href="https://opencollective.com/front-end-checklist/sponsor/2/website" target="_blank"><img src="https://opencollective.com/front-end-checklist/sponsor/2/avatar.svg"></a>
<a href="https://opencollective.com/front-end-checklist/sponsor/3/website" target="_blank"><img src="https://opencollective.com/front-end-checklist/sponsor/3/avatar.svg"></a>
<a href="https://opencollective.com/front-end-checklist/sponsor/4/website" target="_blank"><img src="https://opencollective.com/front-end-checklist/sponsor/4/avatar.svg"></a>
<a href="https://opencollective.com/front-end-checklist/sponsor/5/website" target="_blank"><img src="https://opencollective.com/front-end-checklist/sponsor/5/avatar.svg"></a>
<a href="https://opencollective.com/front-end-checklist/sponsor/6/website" target="_blank"><img src="https://opencollective.com/front-end-checklist/sponsor/6/avatar.svg"></a>
<a href="https://opencollective.com/front-end-checklist/sponsor/7/website" target="_blank"><img src="https://opencollective.com/front-end-checklist/sponsor/7/avatar.svg"></a>
<a href="https://opencollective.com/front-end-checklist/sponsor/8/website" target="_blank"><img src="https://opencollective.com/front-end-checklist/sponsor/8/avatar.svg"></a>
<a href="https://opencollective.com/front-end-checklist/sponsor/9/website" target="_blank"><img src="https://opencollective.com/front-end-checklist/sponsor/9/avatar.svg"></a>


## 라이센스

[![CC0](https://i.creativecommons.org/p/zero/1.0/88x31.png)](https://creativecommons.org/publicdomain/zero/1.0/)

**[⬆ 목차로](#목차)**

[low_img]: data/images/priority/low.svg
[medium_img]: data/images/priority/medium.svg
[high_img]: data/images/priority/high.svg
