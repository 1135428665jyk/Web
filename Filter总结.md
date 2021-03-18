## Filter
#### (1)生命周期
```bash
    （1）初始化
        default void init(FilterConfig filterConfig)
        init方法只执行一次
    （2）过滤功能
        void doFilter(ServletRequest var1, ServletResponse var2, FilterChain var3)
    （3）销毁
        default void destroy()
        destroy方法只执行一次
```
（2）filter执行顺序
```bash
    （1）在web.xml中，先定义的先执行
    
    （2）需求分析
        登录时将登录的账号密码保存到cookie中，下次访问时携带账号和密码，过滤器中进行校验
        用户没有登录直接访问主页时，要跳转到登录页面
        登录过滤器不对登录页面进行过滤
```