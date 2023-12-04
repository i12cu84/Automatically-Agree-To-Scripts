### Automatically-Agree-To-Scripts



QQ空间自动点赞脚本(免安装,免配置复杂环境,可直接快速使用)

 这段代码是一个JavaScript脚本，其功能是自动执行某些操作。下面是代码的逐行解析：

1. `function auto() { ... }`：定义了一个名为`auto`的函数，该函数会在文档加载完成后执行。

2. `var isLike = document.getElementsByClassName("item qz_like_btn_v3 ")[0];`：通过`getElementsByClassName`方法查找具有特定类名的第一个元素，这里查找的是类名为"item qz_like_btn_v3"的元素，并将它存储在变量`isLike`中。

3. `if (isLike.attributes[6].value == 'like') { ... }`：检查`isLike`元素的第7个属性（索引为6）的值是否为'like'。如果是，则执行下面的代码。

4. `isLike.firstChild.click();`：如果上述条件为真，则点击`isLike`元素的第一个子元素。

5. `document.getElementsByClassName("ui-icon icon-refresh-v9")[0].click();`：查找具有类名"ui-icon icon-refresh-v9"的第一个元素，并对其执行点击操作。

6. `var time = prompt("60") * 1000`：通过`prompt`函数获取用户输入的数字（这里假设用户输入的是"60"），然后将其转换为毫秒并存储在变量`time`中。

7. `setInterval(auto, time);`：设置一个定时器，每`time`毫秒执行一次`auto`函数。

这段代码的主要功能是每隔一段时间自动点击具有特定类名的两个元素。

### 使用方法

(以Chrome为例)打开q空间(网页) -> 左边一栏点开"好友动态"

随后在页面中右键"检查" -> Console -> 最下方指令以本节的js代码存入 -> 回车执行脚本 -> 放着挂机即可(会持续执行脚本)