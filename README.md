# FtemplatewordLayout
html {
  color: #222;
  font-size: 1em;
  line-height: 1.4;
}

/*
 * Remove text-shadow in selection highlight:
 * https://twitter.com/miketaylr/status/12228805301
 *
 * Vendor-prefixed and regular ::selection selectors cannot be combined:
 * https://stackoverflow.com/a/16982510/7133471
 *
 * Customize the background color to match your design.
 */

::-moz-selection {
  background: #b3d4fc;
  text-shadow: none;
}

::selection {
  background: #b3d4fc;
  text-shadow: none;
}

/*
 * A better looking default horizontal rule
 */

hr {
  display: block;
  height: 1px;
  border: 0;
  border-top: 1px solid #ccc;
  margin: 1em 0;
  padding: 0;
}

/*
 * Remove the gap between audio, canvas, iframes,
 * images, videos and the bottom of their containers:
 * https://github.com/h5bp/html5-boilerplate/issues/440
 */

audio,
canvas,
iframe,
img,
svg,
video {
  vertical-align: middle;
}

/*
 * Remove default fieldset styles.
 */

fieldset {
  border: 0;
  margin: 0;
  padding: 0;
}

/*
 * Allow only vertical resizing of textareas.
 */

textarea {
  resize: vertical;
}

/* ==========================================================================
   Browser Upgrade Prompt
   ========================================================================== */

.browserupgrade {
  margin: 0.2em 0;
  background: #ccc;
  color: #000;
  padding: 0.2em 0;
}

/* ==========================================================================
   Author's custom styles
   ========================================================================== */
    #wrapper {
      width: 960px;
      border: black thin;
      margin-left: auto;
      margin-right: auto;
      font-size: 18px;
      line-height: 30px;
      font-family: SansSerif, "Helvetica Neue", Helvetica;
    }
    #logo img {
      height: 116px;

    }
    #article_text {
      padding-left: 20px;
      padding-right: 20px;
    }
    #top {
      height: 120px;
      line-height: 120px
    }
    #masthead {
      height: 78px;
      background-size: cover;
      background: url(../img/background.jpg) no-repeat;
      background-position-y: center;
    }
    #main_menu menu {
      padding: 0px;
      margin: 0px;
      text-align: right;
    }
    #sidebar img {
      padding: 20px;
    }
    #sidebar_image {
      margin-right: auto;
      margin-left: auto;
      width: 320px;
    }
    #footer {
      height: 120px;
    }
    .centerText {
      text-align: center;
    }
    .floatLeft {
      float: left;
    }
    .grBig {
      width: 593px;
    }
    .grSmall {
      width: 367px;
    }
    .clear {
      clear: both;
    }
    #main_menu li  {
      display: inline;
      margin: 0px 0px 0px 30px;

    }
/* ==========================================================================
   Helper classes
   ========================================================================== */

/*
 * Hide visually and from screen readers
 */

.hidden {
  display: none !important;
}

/*
* Hide only visually, but have it available for screen readers:
* https://snook.ca/archives/html_and_css/hiding-content-for-accessibility
*
* 1. For long content, line feeds are not interpreted as spaces and small width
*    causes content to wrap 1 word per line:
*    https://medium.com/@jessebeach/beware-smushed-off-screen-accessible-text-5952a4c2cbfe
*/

.sr-only {
  border: 0;
  clip: rect(0, 0, 0, 0);
  height: 1px;
  margin: -1px;
  overflow: hidden;
  padding: 0;
  position: absolute;
  white-space: nowrap;
  width: 1px;
  /* 1 */
}

/*
* Extends the .sr-only class to allow the element
* to be focusable when navigated to via the keyboard:
* https://www.drupal.org/node/897638
*/

.sr-only.focusable:active,
.sr-only.focusable:focus {
  clip: auto;
  height: auto;
  margin: 0;
  overflow: visible;
  position: static;
  white-space: inherit;
  width: auto;
}

/*
* Hide visually and from screen readers, but maintain layout
*/

.invisible {
  visibility: hidden;
}

/*
* Clearfix: contain floats
*
* For modern browsers
* 1. The space content is one way to avoid an Opera bug when the
*    `contenteditable` attribute is included anywhere else in the document.
*    Otherwise it causes space to appear at the top and bottom of elements
*    that receive the `clearfix` class.
* 2. The use of `table` rather than `block` is only necessary if using
*    `:before` to contain the top-margins of child elements.
*/

.clearfix:before,
.clearfix:after {
  content: " ";
  /* 1 */
  display: table;
  /* 2 */
}

.clearfix:after {
  clear: both;
}

/* ==========================================================================
   EXAMPLE Media Queries for Responsive Design.
   These examples override the primary ('mobile first') styles.
   Modify as content requires.
   ========================================================================== */

@media only screen and (min-width: 35em) {
  /* Style adjustments for viewports that meet the condition */
}

@media print,
  (-webkit-min-device-pixel-ratio: 1.25),
  (min-resolution: 1.25dppx),
  (min-resolution: 120dpi) {
  /* Style adjustments for high resolution devices */
}

/* ==========================================================================
   Print styles.
   Inlined to avoid the additional HTTP request:
   https://www.phpied.com/delay-loading-your-print-css/
   ========================================================================== */

@media print {
  *,
  *:before,
  *:after {
    background: transparent !important;
    color: #000 !important;
    /* Black prints faster */
    -webkit-box-shadow: none !important;
    box-shadow: none !important;
    text-shadow: none !important;
  }
  a,
  a:visited {
    text-decoration: underline;
  }
  a[href]:after {
    content: " (" attr(href) ")";
  }
  abbr[title]:after {
    content: " (" attr(title) ")";
  }
  /*
     * Don't show links that are fragment identifiers,
     * or use the `javascript:` pseudo protocol
     */
  a[href^="#"]:after,
  a[href^="javascript:"]:after {
    content: "";
  }
  pre {
    white-space: pre-wrap !important;
  }
  pre,
  blockquote {
    border: 1px solid #999;
    page-break-inside: avoid;
  }
  /*
     * Printing Tables:
     * https://web.archive.org/web/20180815150934/http://css-discuss.incutio.com/wiki/Printing_Tables
     */
  thead {
    display: table-header-group;
  }
  tr,
  img {
    page-break-inside: avoid;
  }
  p,
  h2,
  h3 {
    orphans: 3;
    widows: 3;
  }
  h2,
  h3 {
    page-break-after: avoid;
  }
}
