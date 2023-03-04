# -==用户脚本==
@name 百度翻译 - 页面净化
@version 0.2.3
 🔥 @description 持续更新 🔥 去除百度翻译页面中的多余广告和元素。
@author翁·
@namespace https://gist.github.com/wengx-unx/be2d30e6a9cb3cfa9dda53a8910e3b4c
@supportURL https://github.com/wengx-unx
@match *：//fanyi.baidu.com/*
@icon https://img1.imgtp.com/2023/02/25/YCeeiEQ1.png
@grant GM_addStyle
@license麻省理工学院
==/用户脚本==


(功能() {
    “使用严格”;

    /** 清除样式 */
    常量purge_css = `
#app读，
#transOtherRight，
。页脚
.额外包装，
.op-trans-fb，
.nav-dxy-logo，
.nav-sort-btn，
.new-icon-btn，
.字典标签，
.note-expand-btn，
.manual-trans-btn，
.字典底部，
.navigation-wrapper
       {
显示：无 ！重要;
       }
    `
    /** 设置清除样式 */
    GM_addStyle（purge_css);

    /** 自定义样式 */
    康斯特custom_css = `
.trans-other-wrap-left-part { width： 100% ！important; }
#side-nav .nav-ol .nav-search-again，
#side-nav .nav-item { font-weight： unset; }
#side-nav .nav-item span { color： rgb（0 0 0 / 45%）; }
    `
    /** 设置自定义样式 */
    GM_addStyle（custom_css);

    您的代码在这里...
})();
