<div align="center">
<img src="/docs/images/gateway-border.png" width=350>

# AI 网关
### 通过 1 个快速且友好的 API 升读 100 多个 LLMs.

[![License](https://img.shields.io/github/license/Ileriayo/markdown-badges)](./LICENSE)
[![Discord](https://img.shields.io/discord/1143393887742861333)](https://portkey.ai/community)
[![Twitter](https://img.shields.io/twitter/url/https/twitter/follow/portkeyai?style=social&label=Follow%20%40PortkeyAI)](https://twitter.com/portkeyai)
[![npm version](https://badge.fury.io/js/%40portkey-ai%2Fgateway.svg)](https://www.npmjs.com/package/@portkey-ai/gateway)
<!-- ![example workflow](https://github.com/github/docs/actions/workflows/main.yml/badge.svg) -->

</div>
<br><br>

<p dir="auto"><a href="https://portkey.ai/features/ai-gateway" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">Portkey 的 AI 网关</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">是您的应用程序和托管 LLM 之间的接口。</font><font style="vertical-align: inherit;">它通过统一的 API 简化了对 OpenAI、Anthropic、Mistral、LLama2、Anyscale、Google Gemini 等的 API 请求。</font></font></p>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">✅ 速度</font></font><strong><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">极快</font></font></strong><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">（快 9.9 倍），占用</font></font><strong><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">空间极小</font></font></strong><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">（已安装约 45kb）</font></font><br><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">
✅&nbsp; </font><font style="vertical-align: inherit;">跨多个模型、提供程序和密钥的负载</font></font><strong><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">平衡</font></font></strong><font style="vertical-align: inherit;"></font><br><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">
✅&nbsp; </font></font><strong><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">回退</font></font></strong><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">确保您的应用程序保持弹性  </font></font><br><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">
✅&nbsp; </font><font style="vertical-align: inherit;">默认情况下具有指数回退的  </font></font><strong><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">自动重试</font></font></strong><font style="vertical-align: inherit;"></font><br><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">
✅ 插件中间件根据需要✅ 经过超过</font><strong><font style="vertical-align: inherit;">100B 代币的</font></strong></font><br><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">
战斗测试</font></font><strong><font style="vertical-align: inherit;"></font></strong> <br>
<br></p>
<h2 tabindex="-1" dir="auto"><a id="user-content-getting-started" class="anchor" aria-hidden="true" tabindex="-1" href="#getting-started"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">入门</font></font></h2>
<h3 tabindex="-1" dir="auto"><a id="user-content-installation" class="anchor" aria-hidden="true" tabindex="-1" href="#installation"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">安装</font></font></h3>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">如果您熟悉 Node.js 和</font></font><code>npx</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">，您可以在本地运行您的私有 AI 网关。</font><font style="vertical-align: inherit;">（</font></font><a href="#deploying-ai-gateway"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">其他部署选项</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">）</font></font></p>
<div class="highlight highlight-source-shell notranslate position-relative overflow-auto" dir="auto"><pre>npx @portkey-ai/gateway</pre><div class="zeroclipboard-container">
    <clipboard-copy aria-label="Copy" class="ClipboardButton btn btn-invisible js-clipboard-copy m-2 p-0 tooltipped-no-delay d-flex flex-justify-center flex-items-center" data-copy-feedback="Copied!" data-tooltip-direction="w" value="npx @portkey-ai/gateway" tabindex="0" role="button">
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-copy js-clipboard-copy-icon">
    <path d="M0 6.75C0 5.784.784 5 1.75 5h1.5a.75.75 0 0 1 0 1.5h-1.5a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-1.5a.75.75 0 0 1 1.5 0v1.5A1.75 1.75 0 0 1 9.25 16h-7.5A1.75 1.75 0 0 1 0 14.25Z"></path><path d="M5 1.75C5 .784 5.784 0 6.75 0h7.5C15.216 0 16 .784 16 1.75v7.5A1.75 1.75 0 0 1 14.25 11h-7.5A1.75 1.75 0 0 1 5 9.25Zm1.75-.25a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-7.5a.25.25 0 0 0-.25-.25Z"></path>
</svg>
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-check js-clipboard-check-icon color-fg-success d-none">
    <path d="M13.78 4.22a.75.75 0 0 1 0 1.06l-7.25 7.25a.75.75 0 0 1-1.06 0L2.22 9.28a.751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018L6 10.94l6.72-6.72a.75.75 0 0 1 1.06 0Z"></path>
</svg>
    </clipboard-copy>
  </div></div>
<blockquote>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">您的 AI 网关现在正在</font></font><a href="http://localhost:8787" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">http://localhost:8787</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">上运行🚀</font></font></p>
</blockquote>
<br>
<h3 tabindex="-1" dir="auto"><a id="user-content-usage" class="anchor" aria-hidden="true" tabindex="-1" href="#usage"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">用法</font></font></h3>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">让我们尝试</font><font style="vertical-align: inherit;">通过 AI 网关对 OpenAI进行</font></font><strong><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">聊天完成调用：</font></font></strong><font style="vertical-align: inherit;"></font></p>
<div class="highlight highlight-source-shell notranslate position-relative overflow-auto" dir="auto"><pre>curl <span class="pl-s"><span class="pl-pds">'</span>127.0.0.1:8787/v1/chat/completions<span class="pl-pds">'</span></span> \
  -H <span class="pl-s"><span class="pl-pds">'</span>x-portkey-provider: openai<span class="pl-pds">'</span></span> \
  -H <span class="pl-s"><span class="pl-pds">"</span>Authorization: Bearer <span class="pl-smi">$OPENAI_KEY</span><span class="pl-pds">"</span></span> \
  -H <span class="pl-s"><span class="pl-pds">'</span>Content-Type: application/json<span class="pl-pds">'</span></span> \
  -d <span class="pl-s"><span class="pl-pds">'</span>{"messages": [{"role": "user","content": "Say this is test."}], "max_tokens": 20, "model": "gpt-4"}<span class="pl-pds">'</span></span></pre><div class="zeroclipboard-container">
    <clipboard-copy aria-label="Copy" class="ClipboardButton btn btn-invisible js-clipboard-copy m-2 p-0 tooltipped-no-delay d-flex flex-justify-center flex-items-center" data-copy-feedback="Copied!" data-tooltip-direction="w" value="curl '127.0.0.1:8787/v1/chat/completions' \
  -H 'x-portkey-provider: openai' \
  -H &quot;Authorization: Bearer $OPENAI_KEY&quot; \
  -H 'Content-Type: application/json' \
  -d '{&quot;messages&quot;: [{&quot;role&quot;: &quot;user&quot;,&quot;content&quot;: &quot;Say this is test.&quot;}], &quot;max_tokens&quot;: 20, &quot;model&quot;: &quot;gpt-4&quot;}'" tabindex="0" role="button">
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-copy js-clipboard-copy-icon">
    <path d="M0 6.75C0 5.784.784 5 1.75 5h1.5a.75.75 0 0 1 0 1.5h-1.5a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-1.5a.75.75 0 0 1 1.5 0v1.5A1.75 1.75 0 0 1 9.25 16h-7.5A1.75 1.75 0 0 1 0 14.25Z"></path><path d="M5 1.75C5 .784 5.784 0 6.75 0h7.5C15.216 0 16 .784 16 1.75v7.5A1.75 1.75 0 0 1 14.25 11h-7.5A1.75 1.75 0 0 1 5 9.25Zm1.75-.25a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-7.5a.25.25 0 0 0-.25-.25Z"></path>
</svg>
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-check js-clipboard-check-icon color-fg-success d-none">
    <path d="M13.78 4.22a.75.75 0 0 1 0 1.06l-7.25 7.25a.75.75 0 0 1-1.06 0L2.22 9.28a.751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018L6 10.94l6.72-6.72a.75.75 0 0 1 1.06 0Z"></path>
</svg>
    </clipboard-copy>
  </div></div>
<p dir="auto"><a href="#supported-sdks"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">支持的 SDK 的完整列表</font></font></a></p>
<br>
<h2 tabindex="-1" dir="auto"><a id="user-content-supported-providers" class="anchor" aria-hidden="true" tabindex="-1" href="#supported-providers"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">支持的提供商</font></font></h2>
<table>

|| Provider  | Support | Stream | Supported Endpoints |
|---|---|---|---|--|
| <img src="docs/images/openai.png" width=25 />| OpenAI | ✅  |✅  | `/completions`, `/chat/completions`,`/embeddings`, `/assistants`, `/threads`, `/runs` |
| <img src="docs/images/azure.png" width=25>| Azure OpenAI | ✅  |✅  | `/completions`, `/chat/completions`,`/embeddings` |
| <img src="docs/images/anyscale.png" width=25>| Anyscale | ✅   | ✅  | `/chat/completions` |
| <img src="https://upload.wikimedia.org/wikipedia/commons/2/2d/Google-favicon-2015.png" width=25>| Google Gemini & Palm | ✅  |✅  | `/generateMessage`, `/generateText`, `/embedText` |
| <img src="docs/images/anthropic.png" width=25>| Anthropic  | ✅  |✅  | `/messages`, `/complete` |
| <img src="docs/images/cohere.png" width=25>| Cohere  | ✅  |✅  | `/generate`, `/embed`, `/rerank` |
| <img src="https://assets-global.website-files.com/64f6f2c0e3f4c5a91c1e823a/654693d569494912cfc0c0d4_favicon.svg" width=25>| Together AI  | ✅  |✅  | `/chat/completions`, `/completions`, `/inference` |
| <img src="https://www.perplexity.ai/favicon.svg" width=25>| Perplexity  | ✅  |✅  | `/chat/completions` |
| <img src="https://docs.mistral.ai/img/favicon.ico" width=25>| Mistral  | ✅  |✅  | `/chat/completions`, `/embeddings` |

> [View the complete list of 100+ supported models here](https://portkey.ai/docs/welcome/what-is-portkey#ai-providers-supported)
<br />

## 特征 

<table>
  <tr>
    <td>
      <h4><a href="https://portkey.ai/docs/product/ai-gateway-streamline-llm-integrations/universal-api">统一API签名</a></h4>
      使用 OpenAI 的 API 签名与 100 多个LLMs建立联系。</font><font style="vertical-align: inherit;">AI 网关处理请求、响应和错误转换，因此您无需对代码进行任何更改。</font><font style="vertical-align: inherit;">您可以使用 OpenAI SDK 本身连接到任何受支持的 LLM。
      <br><br>
      <img src="docs/images/openai.png" height=40 />&nbsp;&nbsp;&nbsp;<img src="docs/images/azure.png" height=40 />&nbsp;&nbsp;&nbsp;
      <img src="docs/images/anyscale.png" height=40 />&nbsp;&nbsp;&nbsp;
      <img src="https://upload.wikimedia.org/wikipedia/commons/2/2d/Google-favicon-2015.png" height=40 />&nbsp;&nbsp;&nbsp;<br><br>
      <img src="docs/images/anthropic.png" height=40 />&nbsp;&nbsp;&nbsp;
      <img src="docs/images/cohere.png" height=40 />&nbsp;&nbsp;&nbsp;
      <img src="https://assets-global.website-files.com/64f6f2c0e3f4c5a91c1e823a/654693d569494912cfc0c0d4_favicon.svg" height=40 />&nbsp;&nbsp;&nbsp;<br><br>
      <img src="https://www.perplexity.ai/favicon.svg" height=40 />&nbsp;&nbsp;&nbsp;
      <img src="https://docs.mistral.ai/img/favicon.ico" height=40 />&nbsp;&nbsp;&nbsp;
      <img src="https://1000logos.net/wp-content/uploads/2021/10/logo-Meta.png" height=40 />
     <br><br>
    </td>
    <td>
      <h4><a href="https://portkey.ai/docs/product/ai-gateway-streamline-llm-integrations/fallbacks">备份</a></h4>
      font style="vertical-align: inherit;"><font style="vertical-align: inherit;">
      不要让失败阻止你。</font><font style="vertical-align: inherit;">回退功能允许您按优先顺序指定语言模型 API (LLM) 列表。</font><font style="vertical-align: inherit;">如果主要的 LLM 无法响应或遇到错误，Portkey 将自动回退到列表中的下一个 LLM，确保您的应用程序的稳健性和可靠性。
      <br><br>
      <img src="https://framerusercontent.com/images/gmlOW8yeKP2pGuIsObM6gKLzeMI.png" height=200 />
    </td>
  </tr>
</table>
<table>
  <tr>
    <td>
      <h4><a href="https://portkey.ai/docs/product/ai-gateway-streamline-llm-integrations/automatic-retries">Automatic Retries</a></h4>
      Temporary issues shouldn't mean manual re-runs. AI Gateway can automatically retry failed requests upto 5 times. We apply an exponential backoff strategy, which spaces out retry attempts to prevent network overload.
      <br><br>
      <img src="https://github.com/roh26it/Rubeus/assets/971978/8a6e653c-94b2-4ba7-95c7-93544ee476b1" height=200 />
    </td>
    <td>
      <h4><a href="https://portkey.ai/docs/product/ai-gateway-streamline-llm-integrations/load-balancing">Load Balancing</a></h4>
      Distribute load effectively across multiple API keys or providers based on custom weights. This ensures high availability and optimal performance of your generative AI apps, preventing any single LLM from becoming a performance bottleneck.
      <br><br>
      <img src="https://framerusercontent.com/images/6EWuq3FWhqrPe3kKLqVspevi4.png" height=200 />
    </td>
  </tr>
</table>
<br>

## 配置AI网关

The AI gateway  支持 [configs](https://portkey.ai/docs/api-reference/config-object) 多种路由策略 **fallbacks**, **load balancing**, **retries** and more.
<br><br>
您可以在通过  configs 使得  OpenAI call through the `x-portkey-config` header
```js
// Using the OpenAI JS SDK
const client = new OpenAI({
  baseURL: "http://127.0.0.1:8787", // The gateway URL
  defaultHeaders: {
    'x-portkey-config': {.. your config here ..}, 
  }
});
```
<br>
<details><summary>Here's an example config that retries an OpenAI request 5 times before falling back to Gemini Pro</summary>

```js
{
  "retry": { "count": 5 },
  "strategy": { "mode": "fallback" },
  "targets": [{
      "provider": "openai",
      "api_key": "sk-***"
    },{
      "provider": "google",
      "api_key": "gt5***",
      "override_params": {"model": "gemini-pro"}
  }]
}
```
</details>
<details>
<summary>This config would enable load balancing equally between 2 OpenAI keys</summary>

```js
{
  "strategy": { "mode": "loadbalance" },
  "targets": [{
      "provider": "openai",
      "api_key": "sk-***",
      "weight": "0.5"
    },{
      "provider": "openai",
      "api_key": "sk-***",
      "weight": "0.5"
    }
  ]
}
```
</details>

> Read more about the [config object](https://portkey.ai/docs/api-reference/config-object).
<br>

## 支持的 SDKs

| Language | Supported SDKs |
|---|---|
| Node.js / JS / TS | [Portkey SDK](https://www.npmjs.com/package/portkey-ai) <br> [OpenAI SDK](https://www.npmjs.com/package/openai) <br> [LangchainJS](https://www.npmjs.com/package/langchain) <br> [LlamaIndex.TS](https://www.npmjs.com/package/llamaindex) |
| Python | [Portkey SDK](https://pypi.org/project/portkey-ai/) <br> [OpenAI SDK](https://pypi.org/project/openai/) <br> [Langchain](https://pypi.org/project/langchain/) <br> [LlamaIndex](https://pypi.org/project/llama-index/) |
| Go | [go-openai](https://github.com/sashabaranov/go-openai) |
| Java | [openai-java](https://github.com/TheoKanning/openai-java) |
| Rust | [async-openai](https://docs.rs/async-openai/latest/async_openai/) |
| Ruby | [ruby-openai](https://github.com/alexrudall/ruby-openai) |

<br>

## 部署 AI Gateway
[See docs](docs/installation-deployments.md) on installing the AI Gateway locally or deploying it on popular locations.

<br>

## ROADMAP

<ol dir="auto">
<li><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">支持更多提供商。</font><font style="vertical-align: inherit;">缺少提供商或 LLM 平台，</font></font><a href="https://github.com/Portkey-AI/gateway/issues"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">请提出功能请求</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">。</font></font></li>
<li><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">增强的负载平衡功能可优化不同模型和提供商之间的资源使用。</font></font></li>
<li><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">更稳健的回退和重试策略，进一步提高请求的可靠性。</font></font></li>
<li><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">提高了统一 A&ZeroWidthSpace;&ZeroWidthSpace;PI 签名的可定制性，以满足更多样化的用例。</font></font></li>
</ol>
<p dir="auto"><a href="https://github.com/Portkey-AI/gateway/projects/"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">💬 在此处参与路线图讨论。</font></font></a></p>

 

<br>

## 贡献

The easiest way to contribute is to pick any issue with the `good first issue` tag 💪. Read the Contributing guidelines [here](/CONTRIBUTING.md).

Bug Report? [File here](https://github.com/Portkey-AI/gateway/issues) | Feature Request? [File here](https://github.com/Portkey-AI/gateway/issues)

<br>

## 社区

Join our growing community around the world, for help, ideas, and discussions on AI.

- View our official [Blog](https://portkey.ai/blog)
- Chat live with us on [Discord](https://portkey.ai/community)
- Follow us on [Twitter](https://twitter.com/PortkeyAI)
- Connect with us on [LinkedIn](https://www.linkedin.com/company/portkey-ai/)
<!-- - Visit us on [YouTube](https://www.youtube.com/channel/UCZph50gLNXAh1DpmeX8sBdw) -->
<!-- - Join our [Dev community](https://dev.to/portkeyai) -->
<!-- - Questions tagged #portkey on [Stack Overflow](https://stackoverflow.com/questions/tagged/portkey) -->

![Rubeus Social Share (4)](https://github.com/Portkey-AI/gateway/assets/971978/89d6f0af-a95d-4402-b451-14764c40d03f)

