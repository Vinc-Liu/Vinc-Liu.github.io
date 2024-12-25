---
permalink: /
title: "🐣 About Me"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

<!-- 想要在markdown里引入markdown文件就用以下语法 -->

<span class='anchor' id='about-me'></span>
{% include_relative includes/intro.md %}

{% include_relative includes/news.md %}

{% include_relative includes/edu.md %}

{% include_relative includes/pub.md %}

{% include_relative includes/honors.md %}

<div class='paper-box'><div class='paper-box-image'><div><div class="badge">NeurIPS 2019</div><img src='images/profile.png' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

[FastSpeech: Fast, Robust and Controllable Text to Speech](https://papers.nips.cc/paper/8580-fastspeech-fast-robust-and-controllable-text-to-speech.pdf) \\
**Yi Ren**, Yangjun Ruan, Xu Tan, Tao Qin, Sheng Zhao, Zhou Zhao, Tie-Yan Liu

[**Project**](https://speechresearch.github.io/fastspeech/) <strong><span class='show_paper_citations' data='4FA6C0AAAAAJ:qjMakFHDy7sC'></span></strong>

- FastSpeech is the first fully parallel end-to-end speech synthesis model.
- **Academic Impact**: This work is included by many famous speech synthesis open-source projects, such as [ESPNet ![](https://img.shields.io/github/stars/espnet/espnet?style=social)](https://github.com/espnet/espnet). Our work are promoted by more than 20 media and forums, such as [机器之心](https://mp.weixin.qq.com/s/UkFadiUBy-Ymn-zhJ95JcQ)、[InfoQ](https://www.infoq.cn/article/tvy7hnin8bjvlm6g0myu).
- **Industry Impact**: FastSpeech has been deployed in [Microsoft Azure TTS service](https://techcommunity.microsoft.com/t5/azure-ai/neural-text-to-speech-extends-support-to-15-more-languages-with/ba-p/1505911) and supports 49 more languages with state-of-the-art AI quality. It was also shown as a text-to-speech system acceleration example in [NVIDIA GTC2020](https://resources.nvidia.com/events/GTC2020s21420).
</div>
</div>

<style>

.paper-box {
    display: flex;
    justify-content: left;
    align-items: center;
    flex-direction: row;
    flex-wrap: wrap;
    border-bottom: 1px #efefef solid;
    padding: 2em 0 2em 0;
    
    

    .paper-box-image{
        justify-content: center;
        display: flex;
        width: 100%;
        order: 2;
        img {
            max-width: 400px;
            box-shadow: 3px 3px 6px #888;
            object-fit: cover;
        }
    }
    
    .paper-box-text{
        max-width: 100%;
        order: 1;
    }
    
    @include breakpoint($medium) {
        .paper-box-image{
            justify-content: left;
            min-width: 200px;
            max-width: 40%;
            order: 1;
        }
        
        .paper-box-text{
            justify-content: left;
            padding-left: 2em;
            max-width: 60%;
            order: 2;
        }

    }


}

$scroll_offset : 2em;
h1:before, .anchor:before { 
    content: ''; 
    display: block; 
    position: relative; 
    width: 0; 
    height: $scroll_offset; 
    margin-top: -$scroll_offset;
}

.badge {
    padding-left: 1rem;
    padding-right: 1rem;
    position: absolute;
    margin-top: .5em;
    margin-left: -.5em;
    color: white;
    background-color: #00369f;
    font-size: .8em;
}
</style>
