

- #    推送 codeReview



## 数据结构：

### {

​    **"title"**:**"title"**,
​    **"content"**:**"****视频****12"**,
​    **"param"**:{
​        **"module"**:**"9"**,
​        **"category"**:**"category"**,
​        **"noticeId"**:**"0e5aa58879914959b69ed7b1c01cb5c6"**,
​        **"msgIosCount"**:**"1"**,
​        **"bizCode"**:**"1501"**,
​        **"h5Url"**:**""**,
​        **"courseId"**:**"2009909"**,
​        **"mutable-content"**:**"1"**,
​        **"bizId"**:**"211573"**,
​        **"msgIsRead"**:**"0"**,
​        **"group"**:**"12431223"**
​    },
​    **"functionName"**:**"message"**,
​    **"projectName"**:**"zhsmanager"**
}



## 处理逻辑：

**switch(module){**

​           **1://普通消息**		

​           **2://事务**

​           **3://批阅**

​           **4://动态模块**

​           **5://新增推送类型**

​                 **switch(type){**

​                      	**switch(bizCode){**

​                                  **1://视频详情**

​                                  **2://倾听**

​                                  **3://直播**

​                                  **4://活动**

​                    	  **}**

​                 **}** 

**}**

# 接收跳转逻辑:

### 1、应用在前台时不接受消息；

### 2、点击通知栏，若界面处于非主界面，点击通知栏不跳转

### 3、点击通知栏，只有在界面处于主界面的时候才跳转



## 统计：

#### /appteacher/teacher/discover/recordPushClick?uuid=123%groupId=456