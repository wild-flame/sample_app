# README

RAILS TUTORIAL 3rd edtion demo 3.

## Ruby on Rails Tutorial: sample application

This is the sample application for the
[*Ruby on Rails Tutorial:
Learn Web Development with Rails*](http://www.railstutorial.org/)
by [Michael Hartl](http://www.michaelhartl.com/).

## 演示地址：

Railtutorail第三版Demo（当前项目）：

http://salty-tor-8375.herokuapp.com/

Railtutorial第二版Demo：

http://mighty-meadow-4109.herokuapp.com/

TIPS:

1. 只有重定向使用 _url 形式，其余都使用 _path 形式。（因为 HTTP 标准严格要求重定向的 URL 必须完整。不过在大多数浏览器中，两种形式都可以正常使用。）

2. Rails 会以这些 name 属性的值为键，用户输入的内容为值，构成一个名为 params 的哈希，用来创建用户。

3. **RAILS里放置跨站的机制**简单来说，这段代码首先使用 Unicode 字符 &#x2713;（对号 ✓）强制浏览器使用正确的字符编码提交数据，然后是一个“真伪令牌”（authenticity token），Rails 用它抵御“跨站请求伪造”（Cross-Site Request Forgery，简称 CSRF）攻击。

...
<div style="display:none">
  <input name="utf8" type="hidden" value="&#x2713;" />
  <input name="authenticity_token" type="hidden"
         value="NNb6+J/j46LcrgYUC60wQ2titMuJQ5lLqyAbnbAUkdo=" />
</div>
...

4. `.form-control`在Bootstrap里面的意义
