<div class="Box-sc-g0xbh4-0 bJMeLZ js-snippet-clipboard-copy-unpositioned" data-hpc="true"><article class="markdown-body entry-content container-lg" itemprop="text"><h1 tabindex="-1" dir="auto"><a id="user-content-okhttp" class="anchor" aria-hidden="true" tabindex="-1" href="#okhttp"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">好的http</font></font></h1>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">请参阅</font></font><a href="https://square.github.io/okhttp/" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">项目网站</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">以获取文档和 API。</font></font></p>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">HTTP 是现代应用程序网络的方式。</font><font style="vertical-align: inherit;">这就是我们交换数据和媒体的方式。</font><font style="vertical-align: inherit;">有效地执行 HTTP 可以使您的内容加载速度更快并节省带宽。</font></font></p>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">OkHttp 是一个默认高效的 HTTP 客户端：</font></font></p>
<ul dir="auto">
<li><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">HTTP/2 支持允许对同一主机的所有请求共享套接字。</font></font></li>
<li><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">连接池可减少请求延迟（如果 HTTP/2 不可用）。</font></font></li>
<li><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">透明 GZIP 缩小了下载大小。</font></font></li>
<li><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">响应缓存完全避免了网络重复请求。</font></font></li>
</ul>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">当网络出现问题时，OkHttp 会坚持不懈：它会默默地从常见的连接问题中恢复。</font><font style="vertical-align: inherit;">如果您的服务有多个 IP 地址，OkHttp 将在第一次连接失败时尝试备用地址。</font><font style="vertical-align: inherit;">这对于 IPv4+IPv6 和托管在冗余数据中心的服务是必要的。</font><font style="vertical-align: inherit;">OkHttp 支持现代 TLS 功能（TLS 1.3、ALPN、证书固定）。</font><font style="vertical-align: inherit;">它可以配置为回退以实现广泛的连接。</font></font></p>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">使用 OkHttp 很简单。</font><font style="vertical-align: inherit;">其请求/响应 API 的设计具有流畅的构建器和不变性。</font><font style="vertical-align: inherit;">它支持同步阻塞调用和带有回调的异步调用。</font></font></p>
<h2 tabindex="-1" dir="auto"><a id="user-content-get-a-url" class="anchor" aria-hidden="true" tabindex="-1" href="#get-a-url"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">获取网址</font></font></h2>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">该程序下载 URL 并将其内容打印为字符串。</font></font><a href="https://raw.github.com/square/okhttp/master/samples/guide/src/main/java/okhttp3/guide/GetExample.java"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">完整源码</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">。</font></font></p>
<div class="highlight highlight-source-java notranslate position-relative overflow-auto" dir="auto"><pre><span class="pl-smi">OkHttpClient</span> <span class="pl-s1">client</span> = <span class="pl-k">new</span> <span class="pl-smi">OkHttpClient</span>();

<span class="pl-smi">String</span> <span class="pl-s1">run</span>(<span class="pl-smi">String</span> <span class="pl-s1">url</span>) <span class="pl-k">throws</span> <span class="pl-s1">IOException</span> {
  <span class="pl-smi">Request</span> <span class="pl-s1">request</span> = <span class="pl-k">new</span> <span class="pl-smi">Request</span>.<span class="pl-smi">Builder</span>()
      .<span class="pl-en">url</span>(<span class="pl-s1">url</span>)
      .<span class="pl-en">build</span>();

  <span class="pl-k">try</span> (<span class="pl-smi">Response</span> <span class="pl-s1">response</span> = <span class="pl-s1">client</span>.<span class="pl-en">newCall</span>(<span class="pl-s1">request</span>).<span class="pl-en">execute</span>()) {
    <span class="pl-k">return</span> <span class="pl-s1">response</span>.<span class="pl-en">body</span>().<span class="pl-en">string</span>();
  }
}</pre><div class="zeroclipboard-container">
  
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-copy js-clipboard-copy-icon">
    <path d="M0 6.75C0 5.784.784 5 1.75 5h1.5a.75.75 0 0 1 0 1.5h-1.5a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-1.5a.75.75 0 0 1 1.5 0v1.5A1.75 1.75 0 0 1 9.25 16h-7.5A1.75 1.75 0 0 1 0 14.25Z"></path><path d="M5 1.75C5 .784 5.784 0 6.75 0h7.5C15.216 0 16 .784 16 1.75v7.5A1.75 1.75 0 0 1 14.25 11h-7.5A1.75 1.75 0 0 1 5 9.25Zm1.75-.25a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-7.5a.25.25 0 0 0-.25-.25Z"></path>
</svg>
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-check js-clipboard-check-icon color-fg-success d-none">
    <path d="M13.78 4.22a.75.75 0 0 1 0 1.06l-7.25 7.25a.75.75 0 0 1-1.06 0L2.22 9.28a.751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018L6 10.94l6.72-6.72a.75.75 0 0 1 1.06 0Z"></path>
</svg>
    </clipboard-copy>
  </div></div>
<h2 tabindex="-1" dir="auto"><a id="user-content-post-to-a-server" class="anchor" aria-hidden="true" tabindex="-1" href="#post-to-a-server"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">发布到服务器</font></font></h2>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">该程序将数据发布到服务。</font></font><a href="https://raw.github.com/square/okhttp/master/samples/guide/src/main/java/okhttp3/guide/PostExample.java"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">完整源码</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">。</font></font></p>
<div class="highlight highlight-source-java notranslate position-relative overflow-auto" dir="auto"><pre><span class="pl-k">public</span> <span class="pl-k">static</span> <span class="pl-k">final</span> <span class="pl-smi">MediaType</span> <span class="pl-c1">JSON</span> = <span class="pl-smi">MediaType</span>.<span class="pl-en">get</span>(<span class="pl-s">"application/json"</span>);

<span class="pl-smi">OkHttpClient</span> <span class="pl-s1">client</span> = <span class="pl-k">new</span> <span class="pl-smi">OkHttpClient</span>();

<span class="pl-smi">String</span> <span class="pl-s1">post</span>(<span class="pl-smi">String</span> <span class="pl-s1">url</span>, <span class="pl-smi">String</span> <span class="pl-s1">json</span>) <span class="pl-k">throws</span> <span class="pl-s1">IOException</span> {
  <span class="pl-smi">RequestBody</span> <span class="pl-s1">body</span> = <span class="pl-smi">RequestBody</span>.<span class="pl-en">create</span>(<span class="pl-s1">json</span>, <span class="pl-c1">JSON</span>);
  <span class="pl-smi">Request</span> <span class="pl-s1">request</span> = <span class="pl-k">new</span> <span class="pl-smi">Request</span>.<span class="pl-smi">Builder</span>()
      .<span class="pl-en">url</span>(<span class="pl-s1">url</span>)
      .<span class="pl-en">post</span>(<span class="pl-s1">body</span>)
      .<span class="pl-en">build</span>();
  <span class="pl-k">try</span> (<span class="pl-smi">Response</span> <span class="pl-s1">response</span> = <span class="pl-s1">client</span>.<span class="pl-en">newCall</span>(<span class="pl-s1">request</span>).<span class="pl-en">execute</span>()) {
    <span class="pl-k">return</span> <span class="pl-s1">response</span>.<span class="pl-en">body</span>().<span class="pl-en">string</span>();
  }
}</pre><div class="zeroclipboard-container">
   
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-copy js-clipboard-copy-icon">
    <path d="M0 6.75C0 5.784.784 5 1.75 5h1.5a.75.75 0 0 1 0 1.5h-1.5a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-1.5a.75.75 0 0 1 1.5 0v1.5A1.75 1.75 0 0 1 9.25 16h-7.5A1.75 1.75 0 0 1 0 14.25Z"></path><path d="M5 1.75C5 .784 5.784 0 6.75 0h7.5C15.216 0 16 .784 16 1.75v7.5A1.75 1.75 0 0 1 14.25 11h-7.5A1.75 1.75 0 0 1 5 9.25Zm1.75-.25a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-7.5a.25.25 0 0 0-.25-.25Z"></path>
</svg>
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-check js-clipboard-check-icon color-fg-success d-none">
    <path d="M13.78 4.22a.75.75 0 0 1 0 1.06l-7.25 7.25a.75.75 0 0 1-1.06 0L2.22 9.28a.751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018L6 10.94l6.72-6.72a.75.75 0 0 1 1.06 0Z"></path>
</svg>
    </clipboard-copy>
  </div></div>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">更多示例位于</font></font><a href="https://square.github.io/okhttp/recipes/" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">OkHttp Recipes 页面</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">上。</font></font></p>
<h2 tabindex="-1" dir="auto"><a id="user-content-requirements" class="anchor" aria-hidden="true" tabindex="-1" href="#requirements"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">要求</font></font></h2>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">OkHttp 适用于 Android 5.0+（API 级别 21+）和 Java 8+。</font></font></p>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">OkHttp 依赖于</font></font><a href="https://github.com/square/okio"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">Okio</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">来实现高性能 I/O 和</font></font><a href="https://kotlinlang.org/" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">Kotlin 标准库</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">。</font><font style="vertical-align: inherit;">两者都是小型库，具有很强的向后兼容性。</font></font></p>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">我们强烈建议您保持 OkHttp 是最新的。</font><font style="vertical-align: inherit;">与自动更新 Web 浏览器一样，保持 HTTPS 客户端最新状态是防范潜在安全问题的重要手段。</font></font><a href="https://square.github.io/okhttp/tls_configuration_history/" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">我们跟踪</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">动态 TLS 生态系统并调整 OkHttp 以提高连接性和安全性。</font></font></p>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">OkHttp 使用您平台的内置 TLS 实现。</font><font style="vertical-align: inherit;">在 Java 平台上，OkHttp 还支持
</font></font><a href="https://github.com/google/conscrypt/"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">Conscrypt ，它将</font></font></a><font style="vertical-align: inherit;"></font><a href="https://github.com/google/boringssl"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">BoringSSL</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">与 Java集成</font><font style="vertical-align: inherit;">。</font><font style="vertical-align: inherit;">如果 OkHttp 是第一个安全提供者，它将使用 Conscrypt：</font></font></p>
<div class="highlight highlight-source-java notranslate position-relative overflow-auto" dir="auto"><pre><span class="pl-smi">Security</span>.<span class="pl-en">insertProviderAt</span>(<span class="pl-smi">Conscrypt</span>.<span class="pl-en">newProvider</span>(), <span class="pl-c1">1</span>);</pre><div class="zeroclipboard-container">
    <clipboard-copy aria-label="Copy" class="ClipboardButton btn btn-invisible js-clipboard-copy m-2 p-0 tooltipped-no-delay d-flex flex-justify-center flex-items-center" data-copy-feedback="Copied!" data-tooltip-direction="w" value="Security.insertProviderAt(Conscrypt.newProvider(), 1);" tabindex="0" role="button">
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-copy js-clipboard-copy-icon">
    <path d="M0 6.75C0 5.784.784 5 1.75 5h1.5a.75.75 0 0 1 0 1.5h-1.5a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-1.5a.75.75 0 0 1 1.5 0v1.5A1.75 1.75 0 0 1 9.25 16h-7.5A1.75 1.75 0 0 1 0 14.25Z"></path><path d="M5 1.75C5 .784 5.784 0 6.75 0h7.5C15.216 0 16 .784 16 1.75v7.5A1.75 1.75 0 0 1 14.25 11h-7.5A1.75 1.75 0 0 1 5 9.25Zm1.75-.25a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-7.5a.25.25 0 0 0-.25-.25Z"></path>
</svg>
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-check js-clipboard-check-icon color-fg-success d-none">
    <path d="M13.78 4.22a.75.75 0 0 1 0 1.06l-7.25 7.25a.75.75 0 0 1-1.06 0L2.22 9.28a.751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018L6 10.94l6.72-6.72a.75.75 0 0 1 1.06 0Z"></path>
</svg>
    </clipboard-copy>
  </div></div>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">OkHttp</font></font><code>3.12.x</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">分支支持 Android 2.3+（API 级别 9+）和 Java 7+。</font><font style="vertical-align: inherit;">这些平台缺乏对 TLS 1.2 的支持，不应使用。</font></font></p>
<h2 tabindex="-1" dir="auto"><a id="user-content-releases" class="anchor" aria-hidden="true" tabindex="-1" href="#releases"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">发布</font></font></h2>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">我们的</font></font><a href="https://square.github.io/okhttp/changelog/" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">变更日志</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">有发布历史记录。</font></font></p>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">最新版本可在</font></font><a href="https://search.maven.org/artifact/com.squareup.okhttp3/okhttp/4.12.0/jar" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">Maven Central</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">上获取。</font></font></p>
<div class="highlight highlight-source-kotlin notranslate position-relative overflow-auto" dir="auto"><pre>implementation(<span class="pl-s"><span class="pl-pds">"</span>com.squareup.okhttp3:okhttp:4.12.0<span class="pl-pds">"</span></span>)</pre><div class="zeroclipboard-container">
    <clipboard-copy aria-label="Copy" class="ClipboardButton btn btn-invisible js-clipboard-copy m-2 p-0 tooltipped-no-delay d-flex flex-justify-center flex-items-center" data-copy-feedback="Copied!" data-tooltip-direction="w" value="implementation(&quot;com.squareup.okhttp3:okhttp:4.12.0&quot;)" tabindex="0" role="button">
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-copy js-clipboard-copy-icon">
    <path d="M0 6.75C0 5.784.784 5 1.75 5h1.5a.75.75 0 0 1 0 1.5h-1.5a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-1.5a.75.75 0 0 1 1.5 0v1.5A1.75 1.75 0 0 1 9.25 16h-7.5A1.75 1.75 0 0 1 0 14.25Z"></path><path d="M5 1.75C5 .784 5.784 0 6.75 0h7.5C15.216 0 16 .784 16 1.75v7.5A1.75 1.75 0 0 1 14.25 11h-7.5A1.75 1.75 0 0 1 5 9.25Zm1.75-.25a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-7.5a.25.25 0 0 0-.25-.25Z"></path>
</svg>
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-check js-clipboard-check-icon color-fg-success d-none">
    <path d="M13.78 4.22a.75.75 0 0 1 0 1.06l-7.25 7.25a.75.75 0 0 1-1.06 0L2.22 9.28a.751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018L6 10.94l6.72-6.72a.75.75 0 0 1 1.06 0Z"></path>
</svg>
    </clipboard-copy>
  </div></div>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">快照构建</font></font><a href="https://s01.oss.sonatype.org/content/repositories/snapshots/" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">可用</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">。</font></font><a href="https://square.github.io/okhttp/features/r8_proguard/" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">R8 和 ProGuard</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">规则可用。</font></font></p>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">此外，我们还提供</font></font><a href="https://docs.gradle.org/6.2/userguide/platforms.html#sub:bom_import" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">物料清单 (BOM)，</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">帮助您使 OkHttp 工件保持最新并确保版本兼容性。</font></font></p>
<div class="highlight highlight-source-kotlin notranslate position-relative overflow-auto" dir="auto"><pre>    dependencies {
       <span class="pl-c"><span class="pl-c">//</span> define a BOM and its version</span>
       implementation(platform(<span class="pl-s"><span class="pl-pds">"</span>com.squareup.okhttp3:okhttp-bom:4.12.0<span class="pl-pds">"</span></span>))

       <span class="pl-c"><span class="pl-c">//</span> define any required OkHttp artifacts without version</span>
       implementation(<span class="pl-s"><span class="pl-pds">"</span>com.squareup.okhttp3:okhttp<span class="pl-pds">"</span></span>)
       implementation(<span class="pl-s"><span class="pl-pds">"</span>com.squareup.okhttp3:logging-interceptor<span class="pl-pds">"</span></span>)
    }</pre><div class="zeroclipboard-container">
    <clipboard-copy aria-label="Copy" class="ClipboardButton btn btn-invisible js-clipboard-copy m-2 p-0 tooltipped-no-delay d-flex flex-justify-center flex-items-center" data-copy-feedback="Copied!" data-tooltip-direction="w" value="    dependencies {
       // define a BOM and its version
       implementation(platform(&quot;com.squareup.okhttp3:okhttp-bom:4.12.0&quot;))

       // define any required OkHttp artifacts without version
       implementation(&quot;com.squareup.okhttp3:okhttp&quot;)
       implementation(&quot;com.squareup.okhttp3:logging-interceptor&quot;)
    }" tabindex="0" role="button">
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-copy js-clipboard-copy-icon">
    <path d="M0 6.75C0 5.784.784 5 1.75 5h1.5a.75.75 0 0 1 0 1.5h-1.5a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-1.5a.75.75 0 0 1 1.5 0v1.5A1.75 1.75 0 0 1 9.25 16h-7.5A1.75 1.75 0 0 1 0 14.25Z"></path><path d="M5 1.75C5 .784 5.784 0 6.75 0h7.5C15.216 0 16 .784 16 1.75v7.5A1.75 1.75 0 0 1 14.25 11h-7.5A1.75 1.75 0 0 1 5 9.25Zm1.75-.25a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-7.5a.25.25 0 0 0-.25-.25Z"></path>
</svg>
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-check js-clipboard-check-icon color-fg-success d-none">
    <path d="M13.78 4.22a.75.75 0 0 1 0 1.06l-7.25 7.25a.75.75 0 0 1-1.06 0L2.22 9.28a.751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018L6 10.94l6.72-6.72a.75.75 0 0 1 1.06 0Z"></path>
</svg>
    </clipboard-copy>
  </div></div>
<h2 tabindex="-1" dir="auto"><a id="user-content-mockwebserver" class="anchor" aria-hidden="true" tabindex="-1" href="#mockwebserver"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">模拟Web服务器</font></font></h2>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">OkHttp 包含一个用于测试 HTTP、HTTPS 和 HTTP/2 客户端的库。</font></font></p>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">最新版本可在</font></font><a href="https://search.maven.org/artifact/com.squareup.okhttp3/mockwebserver/4.12.0/jar" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">Maven Central</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">上获取。</font></font></p>
<div class="highlight highlight-source-kotlin notranslate position-relative overflow-auto" dir="auto"><pre>testImplementation(<span class="pl-s"><span class="pl-pds">"</span>com.squareup.okhttp3:mockwebserver:4.12.0<span class="pl-pds">"</span></span>)</pre><div class="zeroclipboard-container">
   
<h2 tabindex="-1" dir="auto"><a id="user-content-graalvm-native-image" class="anchor" aria-hidden="true" tabindex="-1" href="#graalvm-native-image"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">GraalVM 原生镜像</font></font></h2>
<p dir="auto"><font style="vertical-align: inherit;"></font><a href="https://www.graalvm.org/" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">使用 Graal https://www.graalvm.org/</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">构建原生镜像</font><font style="vertical-align: inherit;">应该会自动工作。</font><font style="vertical-align: inherit;">目前这还不是最终发布的版本，因此</font></font><code>5.0.0-alpha.2</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">应该使用。</font><font style="vertical-align: inherit;">请报告您发现的任何错误或解决方法。</font></font></p>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">有关示例构建，请参阅 okcurl 模块。</font></font></p>
<div class="highlight highlight-source-shell notranslate position-relative overflow-auto" dir="auto"><pre>$ ./gradlew okcurl:nativeImage
$ ./okcurl/build/graal/okcurl https://httpbin.org/get</pre><div class="zeroclipboard-container">
    <clipboard-copy aria-label="Copy" class="ClipboardButton btn btn-invisible js-clipboard-copy m-2 p-0 tooltipped-no-delay d-flex flex-justify-center flex-items-center" data-copy-feedback="Copied!" data-tooltip-direction="w" value="$ ./gradlew okcurl:nativeImage
$ ./okcurl/build/graal/okcurl https://httpbin.org/get" tabindex="0" role="button">
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-copy js-clipboard-copy-icon">
    <path d="M0 6.75C0 5.784.784 5 1.75 5h1.5a.75.75 0 0 1 0 1.5h-1.5a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-1.5a.75.75 0 0 1 1.5 0v1.5A1.75 1.75 0 0 1 9.25 16h-7.5A1.75 1.75 0 0 1 0 14.25Z"></path><path d="M5 1.75C5 .784 5.784 0 6.75 0h7.5C15.216 0 16 .784 16 1.75v7.5A1.75 1.75 0 0 1 14.25 11h-7.5A1.75 1.75 0 0 1 5 9.25Zm1.75-.25a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-7.5a.25.25 0 0 0-.25-.25Z"></path>
</svg>
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-check js-clipboard-check-icon color-fg-success d-none">
    <path d="M13.78 4.22a.75.75 0 0 1 0 1.06l-7.25 7.25a.75.75 0 0 1-1.06 0L2.22 9.28a.751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018L6 10.94l6.72-6.72a.75.75 0 0 1 1.06 0Z"></path>
</svg>
    </clipboard-copy>
  </div></div>
<h2 tabindex="-1" dir="auto"><a id="user-content-license" class="anchor" aria-hidden="true" tabindex="-1" href="#license"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">执照</font></font></h2>
<div class="snippet-clipboard-content notranslate position-relative overflow-auto"><pre class="notranslate"><code>Copyright 2019 Square, Inc.

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

   http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
</code></pre><div class="zeroclipboard-container">
    <clipboard-copy aria-label="Copy" class="ClipboardButton btn btn-invisible js-clipboard-copy m-2 p-0 tooltipped-no-delay d-flex flex-justify-center flex-items-center" data-copy-feedback="Copied!" data-tooltip-direction="w" value="Copyright 2019 Square, Inc.

Licensed under the Apache License, Version 2.0 (the &quot;License&quot;);
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

   http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an &quot;AS IS&quot; BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License." tabindex="0" role="button">
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-copy js-clipboard-copy-icon">
    <path d="M0 6.75C0 5.784.784 5 1.75 5h1.5a.75.75 0 0 1 0 1.5h-1.5a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-1.5a.75.75 0 0 1 1.5 0v1.5A1.75 1.75 0 0 1 9.25 16h-7.5A1.75 1.75 0 0 1 0 14.25Z"></path><path d="M5 1.75C5 .784 5.784 0 6.75 0h7.5C15.216 0 16 .784 16 1.75v7.5A1.75 1.75 0 0 1 14.25 11h-7.5A1.75 1.75 0 0 1 5 9.25Zm1.75-.25a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-7.5a.25.25 0 0 0-.25-.25Z"></path>
</svg>
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-check js-clipboard-check-icon color-fg-success d-none">
    <path d="M13.78 4.22a.75.75 0 0 1 0 1.06l-7.25 7.25a.75.75 0 0 1-1.06 0L2.22 9.28a.751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018L6 10.94l6.72-6.72a.75.75 0 0 1 1.06 0Z"></path>
</svg>
    </clipboard-copy>
  </div></div>
</article></div>
