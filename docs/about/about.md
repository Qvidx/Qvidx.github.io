---
title: About Me
hide:
  #- navigation  #隐藏边框目录
  - toc
  - path
  - feedback
glightbox: false
comments: true  #默认不开启评论
---

<div class="flip-container">
<div class="image-container">
    <img src="https://avatars.githubusercontent.com/u/155136161?s=400&u=c443d94617f3997d385efdf2231740294d9eafbf&v=4" alt="Back Image">
    <img src="./docs\images\照骗.JPG" alt="Front Image">
</div>
</div>
<style>
    .flip-container {
    position: relative;
    width: 290px;
    height: 290px;
    margin: 10px auto;
    display: flex;
    align-items: flex-start;
    /* 对齐顶部 */
    justify-content: flex-end;
    /* 将文字放置右上角 */
    }
    .image-container {
        position: relative;
        position: relative;
        width: 290px;
        height: 290px;
    }
    .image-container img {
        position: absolute;
        top: 0;
        left: 0;
        width: 100%;
        height: 100%;
        object-fit: cover;    /* 图片填满容器 */
        border-radius: 50%;
        border: 4px solid #ffffff; /* 白色边框 */
        box-shadow: 0 8px 24px rgba(14, 30, 37, 0.15); /* 阴影 */
        backface-visibility: hidden; /* 隐藏背面 */
        transition: transform 0.6s ease-in-out; /* 仅对transform过渡 */
    }
    .image-container img:first-child {
        z-index: 1;
        backface-visibility: hidden;
    }
    .image-container img:last-child {
        z-index: 0;
        transform: rotateY(180deg);
        backface-visibility: hidden;
    }
    .image-container:hover img:first-child {
        transform: rotateY(180deg);
        z-index: 2;
    }
    .image-container:hover img:last-child {
        transform: rotateY(0deg);
        z-index: 3;
    }
</style>


<!-- script src="https://sdk.jinrishici.com/v2/browser/jinrishici.js" charset="utf-8" ></script>-->

<div class="grid cards" markdown>

- :simple-qq: __QQ:__ 1586517373
- :simple-wechat: __WeChat:__ Qvi15523375720
- :telephone_receiver: __Tel1:__ 15523375720
- :telephone_receiver: __Tel2:__ 18010405720
- :simple-neteasecloudmusic: __网易云音乐:__ wkkkkyo
- :simple-github: [__GitHub:__ Qvidx](https://github.com/Qvidx){ target="_blank" }
- :simple-tiktok: [__抖音:__ sleeep](https://www.douyin.com/user/MS4wLjABAAAAHUzLA-zgJikwHAtsf7V083S7zfaa5CSlR2EOR6XNSVI?from_tab_name=main){ target="_blank" }
</div>



## 我的履历

<section class="qualification section">
    <div class="qualification__container container">
        <div class="qualification__tabs">
            <div class="qualification__button button--flex qualification__active" data-target='#education'>
                <iconify-icon icon="fluent:hat-graduation-12-regular" class="qualification__icon"></iconify-icon>
                来时路
            </div>
        </div>       
        <div class="qualification__sections">
            <!-- 教育经历时间线 -->
            <div class="qualification__content qualification__active" data-content id="education">
                <!-- 时间线项目 -->
                <div class="qualification__data">
                    <div>
                        <h3 class="qualification__title">垫江实验中学</h3>
                        <span class="qualification__subtitle">平凡的三年</span>
                        <div class="qualification__calendar">
                            <iconify-icon icon="tabler:calendar" aria-hidden="true"></iconify-icon>
                            <span class="qualification__date">2018 - 2021</span>
                        </div>
                    </div>
                    <div>
                        <span class="qualification__rounder"></span>
                        <span class="qualification__line"></span>
                    </div>
                </div>
                <div class="qualification__data">
                    <div></div>
                    <div>
                        <span class="qualification__rounder"></span>
                        <span class="qualification__line"></span>
                    </div>
                    <div>
                        <h3 class="qualification__title">CQUE</h3>
                        <span class="qualification__subtitle">计算机科学与技术专业学士</span>
                        <div class="qualification__calendar">
                            <iconify-icon icon="tabler:calendar" aria-hidden="true"></iconify-icon>
                            <span class="qualification__date">2021 - 2024</span>
                        </div>
                    </div>
                </div>
                <div class="qualification__data">
                    <div>
                        <h3 class="qualification__title">交流学习</h3>
                        <span class="qualification__subtitle">重庆大学智能网联汽车专业</span>
                        <div class="qualification__calendar">
                            <iconify-icon icon="tabler:calendar" aria-hidden="true"></iconify-icon>
                            <span class="qualification__date">2024 - 2025</span>
                        </div>
                    </div>
                    <div>
                        <span class="qualification__rounder"></span>
                        <span class="qualification__line"></span>
                    </div>
                </div>
                <div class="qualification__data">
                    <div></div>
                    <div>
                        <span class="qualification__rounder"></span>
                        <span class="qualification__line"></span>
                    </div>
                    <div>
                        <h3 class="qualification__title">未完待续</h3>
                        <span class="qualification__subtitle">于道各努力，千里自同风</span>
                        <div class="qualification__calendar">
                            <iconify-icon icon="tabler:calendar" aria-hidden="true"></iconify-icon>
                            <span class="qualification__date">Before - After</span>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</section>
<HR style="FILTER: progid:DXImageTransform.Microsoft.Shadow(color:#608DBD,direction:145,strength:15)" width="100%" color=#009485 SIZE=1>