---
title: Night Mode Toggle Across the Website!
description: Changing background color to a darker one helps reading under low light. This can be achieved easily with JS. But making it to remember the change across the site is a little tricky. Here is a way to do it.
article: /dark-theme-switch/
layout: demo
---

<style>
.dark-div {
    padding:30px 60px; 
    border: 1px dashed #000; 
    width: 300px;
    text-align:center;
    margin: 10px;
    cursor: pointer;

}
</style>

## Dark Mode Switch
This box changes color on click but does not retain the state after refresh.

<div class="dark-div" id="dark-div" style="background-color: rgb(255, 255, 255)" onclick="dark()">
    <p>Click me</p>
</div>


## Dark Mode Across the Domin
This box not only changes color on click but also retains the state even after refresh.

<div class="dark-div" id="dark-div-2" style="background-color: rgb(255, 255, 255)" onclick="darker()">
    <p>Switch</p>
</div>


<script>function dark(){"rgb(255, 255, 255)"==document.getElementById("dark-div").style.backgroundColor?(document.getElementById("dark-div").style.backgroundColor="rgb(6, 23, 37)",document.getElementById("dark-div").style.color="rgb(255, 255, 255)"):(document.getElementById("dark-div").style.backgroundColor="rgb(255, 255, 255)",document.getElementById("dark-div").style.color="rgb(6, 23, 37)")};</script>
<script>
document.getElementById("dark-div-2").style.backgroundColor=sessionStorage.getItem("bg");document.getElementById("dark-div-2").style.color=sessionStorage.getItem("cc");function darker(){"rgb(255, 255, 255)"===sessionStorage.getItem("bg")?(sessionStorage.setItem("bg","rgb(6, 23, 37)"),sessionStorage.setItem("cc","#eee")):null==sessionStorage.getItem("bg")?(sessionStorage.setItem("bg","rgb(6, 23, 37)"),sessionStorage.setItem("cc","#eee")):"rgb(6, 23, 37)"===sessionStorage.getItem("bg")&&(sessionStorage.setItem("bg","rgb(255, 255, 255)"),sessionStorage.setItem("cc","#333"));document.getElementById("dark-div-2").style.backgroundColor=sessionStorage.getItem("bg");document.getElementById("dark-div-2").style.color=sessionStorage.getItem("cc")}
;
</script>