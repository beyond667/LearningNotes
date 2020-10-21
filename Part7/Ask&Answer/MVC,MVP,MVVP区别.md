#### MVC
model-view-controller，view发送指令到controller，controller通知model层去更新数据，更新完数据后直接显示在view中。  
对于android来说，xml和activity/fragment就是view，java bean就是model，activity和fragment就是controller  
比如界面有个按钮，点了后去后台拿数据，xml和activity是view，点击后调用到setonclicklistener中，相当于通知controller，从后台拿数据相当于model，拿回的数据在activity中显示。
##### MVC缺点
activity既是controller，又是view，导致activity还会成百上千行代码
#### MVP
model-view-presenter，mvc的演化版，把activity作为纯粹的view层，相关的业务逻辑都抽到presenter层，由persenter作为桥梁来连接view和model。  
##### MVP优缺点
优点就是把view和model完全分离，模块职责划分清晰，缺点就是persenter维护困难，而且可能接口爆炸，比如一个接口有5个操作，A类只需要其中3个，B类需要另外的3个，C类需要4个，这几个类需要的既有交叉又有相同，persenter复用困难。
#### MVVM
model-view-viewmodel，



