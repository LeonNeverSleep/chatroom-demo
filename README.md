本html文件是本人学习html+css时练习的一个小demo

html结构可拆分为组件进行使用

css采用内联样式

使用了简单的js来实现发送消息的功能：

        function send(){
            var text = document.querySelector(".text").value
            var right = document.querySelector(".ChatDiv")
                right.innerHTML=right.innerHTML+`<div class="right1">
                <div class="head2">肖战</div>
                <div class="msg2">
                    <div class="time2">13:40</div>
                    <div class="content2">${text}</div>
                </div>
            </div>`
            right.scrollTop=right.scrollHeight
            document.querySelector(".text").value=' '
        }
