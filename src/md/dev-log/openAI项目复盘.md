# openAI项目复盘（）

## chatgpt-sdk

1. 第一章：
   - 创建了chatgpt-sdk的组件工程；并且使用了okhttp3封装了对openAI的请求处理，实现对话模型（专门用于封装对 OpenAI 接口的使用。）
   -  以 OpenAI 抽象为**会话模型**
   - 我们通过工厂模型，开启一个使用 **okhttp3** 封装的 OpenAI 会话服务，进行流程的调用。（封装接口）
   - 包括请求拦截的处理，因为我们需要对http请求设置一些必要的参数信息，如；**ApiKey、Token** 等。
   - 还需要用到 Retrofit2 组件，Retrofit2 可以将 HTTP API 转化为 Java 接口，并通过注解的方式描述请求参数和响应结果等信息，从而方便地发送网络请求。