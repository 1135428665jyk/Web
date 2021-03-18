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