
<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Transitional//EN" "http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd">
<html xmlns="http://www.w3.org/1999/xhtml">
  <head>
    <meta http-equiv="Content-Type" content="text/html; charset=UTF-8"/>
    <title>Loading... :: Reader View</title>
    <link rel="stylesheet" href="fontello.css">
    <link rel="stylesheet" href="index.css">
    <link rel="stylesheet" href="libs/text-to-speech/tts.css">
  </head>
  <body data-speech=false>
    <div id="toolbar">
      <span class="icon-close" data-cmd="close" title="Close Reader View"></span>
      <span class="icon-font" data-cmd="open-font-utils" title="Type controls"></span>
      <div id="font-utils" tabindex="-1" class="hidden">
        <table border="0" cellpadding="0" cellspacing="0">
          <colgroup>
            <col style="border-right: solid 1px #B5B5B5;" width=50%>
            <col>
          </colgroup>
          <tr>
            <td data-cmd="font-type-sans-serif"><span>Aa</span><span>Sans-serif</span></td>
            <td data-cmd="font-type-serif"><span>Aa</span><span>Serif</span></td>
          </tr>
          <tr>
            <td data-cmd="font-decrease"><span class="icon-minus"></span></td>
            <td data-cmd="font-increase"><span class="icon-plus"></span></td>
          </tr>
          <tr>
            <td data-id="full-width" data-cmd="full-width">
              <input id="full-width" type="checkbox"/>
              <label>Full Width</label>
            </td>
            <td>
              <div class="strech">
                <span data-cmd="width-increase" class="icon-"></span>&nbsp;
                <span data-cmd="width-decrease" class="icon-"></span>
              </div>
            </td>
          </tr>
          <tr>
            <td data-id="no-height" data-cmd="no-height">
              <input id="no-height" type="checkbox"/>
              <label>No Height</label>
            </td>
            <td>
              <div class="strech">
                <span class="icon-article-collapsed" data-cmd="line-height-type-1"></span>
                <span class="icon-article-expanded" data-cmd="line-height-type-2"></span>
              </div>
            </td>
          </tr>
          <tr>
            <td colspan="2" data-id="color">
              <div>
                <span data-cmd="color-mode-light">Light</span>
                <span data-cmd="color-mode-sepia">Sepia</span>
                <span data-cmd="color-mode-solarized-light">Solarized</span>
              </div>
              <div>
                <span data-cmd="color-mode-dark">Dark</span>
                <span data-cmd="color-mode-groove-dark">Groove</span>
                <span data-cmd="color-mode-solarized-dark">Solarized</span>
              </div>
            </td>
          </tr>
        </table>
      </div>
      <div id="image-utils" tabindex="-1" class="hidden">
        <table border="0" cellpadding="0" cellspacing="0">
          <colgroup>
            <col style="border-right: solid 1px #B5B5B5;" width=50%>
            <col>
          </colgroup>
          <tr title="The +/- buttons only scale images with width greater than 32px. Scaling is not persistent operation. To reset, refresh the page.">
            <td data-cmd="image-decrease"><span class="icon-minus"></span></td>
            <td data-cmd="image-increase"><span class="icon-plus"></span></td>
          </tr>
          <tr>
            <td data-cmd="image-hide">Hide</td>
            <td data-cmd="image-show">Show</td>
          </tr>
        </table>
      </div>
    </div>
    <div id="content">
      <div id="tips">
        <div>
          <input type="button" value="×">
          <span></span>
        </div>
      </div>
      <iframe></iframe>
    </div>
    <div id="speech">
      <span data-cmd="close-speech">×</span>
    </div>
    <div id="navigate" class="hidden">
      <input type="button" id="navigate-previous" value="&#xE80D;" disabled=true title="move to the previous page (Meta + Shift + Left Arrow Key)">
      <input type="button" id="navigate-next" value="&#xE80A;" disabled=true title="move to the next page (Meta + Shift + Right Arrow Key)">
    </div>
    <script src="/config.js"></script>
    <script src="index.js"></script>
    <script async src="tip.js"></script>
  </body>
</html>
