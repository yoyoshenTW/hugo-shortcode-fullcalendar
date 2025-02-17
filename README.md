# 透過 Hugo Markdown 中使用 Shortcode 製作 Fullcalendar(同步 Google Calendar)

此 Shortcode 為提供給 Hugo 使用，目的是在你的 Hugo Website 中，能夠將 Google Calendar 透過 Fullcalendar 這個套件顯示在網頁上，而使用這個要注意兩件事情：

1. 目前的 Google Calendar API 以及 Google Calendar ID 都是放在前端，建議另外架設後端來提供機密資料
2. 為了要求統一管理，這份的 CSS 與 JS 都寫在一起，如果 CSS 有與你的原生 class 衝突要調製整

# 如何使用
請下載這份檔案 [fullcalendar.html](https://github.com/yoyoshenTW/hugo-shortcode-fullcalendar/blob/main/layouts/shortcodes/fullcalendar.html)
並將他放在你 Hugo 網站的根目錄的 *layouts/shortcodes* 底下
即可完成

接著在你的 markdown 文件中(例如 index.md)
在需要使用 Fullcalendar 的地方，引用此 shortcode，並在參數放上 API Key 以及 Google Calendar ID
在經過渲染後即可實現

## Example
```
{{< fullcalendar "YOUR_API_KEY" "YOUR_CALENDAR_ID" >}}
```
<hr/>

# Creating a Fullcalendar (Synchronized with Google Calendar) via Shortcode in Hugo Markdown

This Shortcode is provided for Hugo. The purpose is to display Google Calendar on your webpage through the Fullcalendar plugin in your Hugo Website. There are two things to note when using this:

1.  The current Google Calendar API and Google Calendar ID are placed on the front end. It is recommended to set up a back end to provide confidential data.
2.  In order to require unified management, this CSS and JS are written together. If the CSS conflicts with your native class, it needs to be adjusted.

# How to use

Please download this file [fullcalendar.html](https://github.com/yoyoshenTW/hugo-shortcode-fullcalendar/blob/main/layouts/shortcodes/fullcalendar.html)
and place it in the *layouts/shortcodes* directory of the root directory of your Hugo website
to complete.

Then in your markdown document (for example, index.md)
In the place where Fullcalendar needs to be used, refer to this shortcode and put the API Key and Google Calendar ID in the parameters
It can be realized after rendering

## Example

