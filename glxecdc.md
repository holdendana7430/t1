代发 wailian999

[U69] PHP：PDO 预处理
来源：http://baike.zdbjq.cn/Article/details/gwbkgqjgy.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://m.share.fehbvm.com/Article/details/gakgknmbm.sHtML

[U70] PHP：PDO 事务
来源：http://www.share.fehbvm.com/Article/details/glsgdbcbp.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wap.zdbjq.cn/Article/details/ghwpwmzch.sHtML

[U71] PHP：抛出异常
来源：http://baike.fehbvm.com/Article/details/gyayhvpdy.sHtML

throw new RuntimeException("失败", 500);
来源：http://baike.zdbjq.cn/Article/details/gnwkzhude.sHtML

[U72] PHP：写错误日志
来源：http://mobile.zdbjq.cn/Article/details/gakyldiur.sHtML

error_log("失败: " . $e->getMessage());
来源：http://m.share.fehbvm.com/Article/details/gzqewdqwq.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.m.share.hesvh.cn/Article/details/guqtzhdkm.sHtML

parse_ini_file("config.ini", true)
来源：http://www.blog.hesvh.cn/Article/details/gngiwjvpb.sHtML

[U74] PHP：读取环境变量
来源：http://blog.hesvh.cn/Article/details/gqxusdeil.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.share.zdbjq.cn/Article/details/glpyzoipg.sHtML

[U75] PHP：依赖注入
来源：http://www.m.share.fehbvm.com/Article/details/gmrgeavjt.sHtML

composer require psr/container
来源：http://www.share.zdbjq.cn/Article/details/glmianukx.sHtML

[U76] PHP：简单路由
来源：http://www.m.share.fehbvm.com/Article/details/gunyyttkz.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.share.zdbjq.cn/Article/details/gdfbqdfug.sHtML

[U77] PHP：模板渲染
来源：http://blog.zdbjq.cn/Article/details/guqbldhzb.sHtML

composer require twig/twig
来源：http://www.blog.zdbjq.cn/Article/details/gvzecimlp.sHtML

[U78] PHP：单元测试
来源：http://wap.zdbjq.cn/Article/details/guhyljotx.sHtML

composer require --dev phpunit/phpunit
来源：http://3g.zdbjq.cn/Article/details/gwfozlcjg.sHtML

[U79] PHP：静态分析
来源：http://3g.hesvh.cn/Article/details/glsqxwdpt.sHtML

composer require --dev phpstan/phpstan
来源：http://blog.hesvh.cn/Article/details/gwcwynpxu.sHtML

[U80] PHP：代码规范修复
来源：http://3g.fehbvm.com/Article/details/gazsbttdo.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://m.share.fehbvm.com/Article/details/gbggfkmsi.sHtML

[U81] JS：初始化项目
来源：http://blog.zdbjq.cn/Article/details/gymtyltrx.sHtML

npm init -y;  npm i express
来源：http://mobile.fehbvm.com/Article/details/gnwkjzvdk.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.hesvh.cn/Article/details/guyetrclx.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.zdbjq.cn/Article/details/gonylgciq.sHtML

[U83] JS：ES Module 导入导出
来源：http://3g.zdbjq.cn/Article/details/gousifjpi.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.share.zdbjq.cn/Article/details/gaxmiwyfk.sHtML

[U84] JS：CommonJS 写法
来源：http://mobile.hesvh.cn/Article/details/gaorqbkzw.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://read.share.hesvh.cn/Article/details/gbtbpdunk.sHtML

[U85] JS：可选链
来源：http://baike.zdbjq.cn/Article/details/gjyplbbvy.sHtML

a?.b?.c
来源：http://www.m.share.zdbjq.cn/Article/details/gzxapzyiu.sHtML

[U86] JS：空值合并
来源：http://wap.fehbvm.com/Article/details/guadezhrl.sHtML

a ?? b
来源：http://mobile.fehbvm.com/Article/details/grbbysuqj.sHtML

[U87] JS：解构默认值
来源：http://blog.fehbvm.com/Article/details/gbvazbisv.sHtML

const { a = 1, b = 2 } = obj;
来源：http://baike.hesvh.cn/Article/details/gpxgjxpng.sHtML

[U88] JS：对象展开合并
来源：http://read.share.hesvh.cn/Article/details/gsvyjknuk.sHtML

{ ...a, ...b }
来源：http://baike.fehbvm.com/Article/details/gymjvprco.sHtML

[U89] JS：数组去重
来源：http://www.blog.hesvh.cn/Article/details/gtshblbve.sHtML

[...new Set(arr)]
来源：http://3g.hesvh.cn/Article/details/gradokfum.sHtML

[U90] JS：数字数组排序
来源：http://wap.hesvh.cn/Article/details/gdxdxufmr.sHtML

[...arr].sort((a, b) => a - b)
来源：http://blog.hesvh.cn/Article/details/gabslcrww.sHtML

[U91] JS：对象键值遍历
来源：http://www.blog.hesvh.cn/Article/details/gnlcfxqst.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://3g.hesvh.cn/Article/details/giwegbduk.sHtML

[U92] JS：深拷贝
来源：http://www.share.hesvh.cn/Article/details/gntpokslp.sHtML

structuredClone(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/grmtwmtul.sHtML

[U93] JS：模板字符串
来源：http://www.m.share.zdbjq.cn/Article/details/grfbqbpyu.sHtML

`共 ${n} 条`
来源：http://m.share.zdbjq.cn/Article/details/gcoxcupjn.sHtML

[U94] JS：箭头函数
来源：http://www.blog.fehbvm.com/Article/details/gqnkfkxbe.sHtML

const double = x => x * 2;
来源：http://mobile.fehbvm.com/Article/details/gkgsbpxsd.sHtML

[U95] JS：Promise 包装
来源：http://m.share.zdbjq.cn/Article/details/griowiogl.sHtML

new Promise((resolve, reject) => {})
来源：http://3g.hesvh.cn/Article/details/gfbfmsldx.sHtML

[U96] JS：async/await 与异常
来源：http://www.blog.hesvh.cn/Article/details/gmpoxmftr.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://m.share.zdbjq.cn/Article/details/gnxtjxeck.sHtML

[U97] JS：并发请求
来源：http://blog.zdbjq.cn/Article/details/guvwdbznl.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.hesvh.cn/Article/details/gdbvuobqv.sHtML

[U98] JS：fetch 带 JSON
来源：http://mobile.fehbvm.com/Article/details/gzgwrfajn.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://baike.zdbjq.cn/Article/details/gktkxpujo.sHtML

[U99] JS：事件监听
来源：http://wap.zdbjq.cn/Article/details/gwezkcxfh.sHtML

el.addEventListener("click", e => {})
来源：http://read.share.zdbjq.cn/Article/details/gxvwwrned.sHtML

[U100] JS：DOM 查询
来源：http://mobile.zdbjq.cn/Article/details/grkzwsfaa.sHtML

document.querySelector(".item")
来源：http://blog.zdbjq.cn/Article/details/grfmdagty.sHtML

[U101] JS：classList 操作
来源：http://www.blog.hesvh.cn/Article/details/ghhuqhjti.sHtML

el.classList.toggle("active")
来源：http://baike.hesvh.cn/Article/details/gothgbiyf.sHtML

[U102] JS：本地存储
来源：http://www.blog.hesvh.cn/Article/details/ghneyzeyz.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.hesvh.cn/Article/details/gbrebcbzo.sHtML

[U103] JS：定时器
来源：http://m.share.fehbvm.com/Article/details/gkutjidgf.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blog.hesvh.cn/Article/details/glyhgxbal.sHtML

[U104] JS：防抖
来源：http://wap.hesvh.cn/Article/details/gjkcwptwm.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.hesvh.cn/Article/details/gzuetqtxo.sHtML

[U105] JS：节流
来源：http://www.m.share.zdbjq.cn/Article/details/gmebrytqe.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.zdbjq.cn/Article/details/gwhdisrpi.sHtML

[U106] JS：日期格式化
来源：http://blog.fehbvm.com/Article/details/grzyocgzm.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.hesvh.cn/Article/details/ghxzlasot.sHtML

[U107] JS：数字千分位
来源：http://wap.hesvh.cn/Article/details/glulpplvx.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.hesvh.cn/Article/details/gvruaxmwy.sHtML

[U108] JS：随机整数
来源：http://www.blog.hesvh.cn/Article/details/gqctssbkt.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.zdbjq.cn/Article/details/gslodguyi.sHtML

[U109] JS：数组分组
来源：http://www.blog.hesvh.cn/Article/details/gwqdedkef.sHtML

Object.groupBy(arr, x => x.type)
来源：http://3g.hesvh.cn/Article/details/gviawfobl.sHtML

[U110] JS：数组分块
来源：http://m.share.zdbjq.cn/Article/details/gncyydzxn.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.fehbvm.com/Article/details/gwjwjqjzj.sHtML

[U111] JS：对象转 Map
来源：http://www.share.zdbjq.cn/Article/details/gnrjhatxs.sHtML

new Map(Object.entries(obj))
来源：http://baike.zdbjq.cn/Article/details/gnvdrsekq.sHtML

[U112] JS：字符串补位
来源：http://mobile.fehbvm.com/Article/details/gmloijmft.sHtML

"7".padStart(3, "0")
来源：http://m.share.zdbjq.cn/Article/details/gzesgjccj.sHtML

[U113] JS：正则替换全部
来源：http://mobile.fehbvm.com/Article/details/gbqoaodfe.sHtML

s.replaceAll("a", "b")
来源：http://blog.fehbvm.com/Article/details/gdkvhosfc.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.fehbvm.com/Article/details/glsdimwpe.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gsbqallkt.sHtML

[U115] JS：生成 UUID
来源：http://mobile.hesvh.cn/Article/details/gvmjeqwru.sHtML

crypto.randomUUID()
来源：http://www.share.fehbvm.com/Article/details/gfyfdgfob.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.fehbvm.com/Article/details/gbprjqtcs.sHtML

/** @param {string} name */ function f(name) {}
来源：http://baike.fehbvm.com/Article/details/gydgvxlwz.sHtML

[U117] JS：单元测试
来源：http://www.share.fehbvm.com/Article/details/gamynivhv.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.zdbjq.cn/Article/details/gpodjicff.sHtML

[U118] JS：开发服务器
来源：http://mobile.fehbvm.com/Article/details/gftdaqsln.sHtML

npm i -D vite;  npx vite
来源：http://3g.fehbvm.com/Article/details/gjvkamcdp.sHtML

[U119] JS：生产构建
来源：http://blog.fehbvm.com/Article/details/gfmwodltg.sHtML

npx vite build
来源：http://m.share.hesvh.cn/Article/details/gpuvvdyai.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://3g.hesvh.cn/Article/details/glqjnkwpq.sHtML

import.meta.env.VITE_API_URL
来源：http://baike.fehbvm.com/Article/details/glgwfinhu.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gtpovctct.sHtML

统计汇总
来源：http://www.m.share.zdbjq.cn/Article/details/gotperoyo.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gsuhugfvp.sHtML

按语言统计（条）：
来源：http://wap.zdbjq.cn/Article/details/gebocohgn.sHtML

Python ......... 252
来源：http://www.m.share.fehbvm.com/Article/details/gbkdvdgie.sHtML

PHP ............ 252
来源：http://baike.hesvh.cn/Article/details/gjeihvxkr.sHtML

JavaScript ..... 252
来源：http://read.share.fehbvm.com/Article/details/guoelhjre.sHtML

TypeScript ..... 212
来源：http://www.share.hesvh.cn/Article/details/gcwbiswew.sHtML

Java ........... 212
来源：http://3g.fehbvm.com/Article/details/gclpgrezm.sHtML

Go ............. 212
来源：http://www.share.zdbjq.cn/Article/details/gufmtksgu.sHtML

Ruby ........... 212
来源：http://www.blog.hesvh.cn/Article/details/gmmmjkxvu.sHtML

C# ............. 212
来源：http://3g.fehbvm.com/Article/details/gzvzjojnp.sHtML

C .............. 30
来源：http://www.share.fehbvm.com/Article/details/gqhzbhxcc.sHtML

C++ ............ 30
来源：http://www.m.share.zdbjq.cn/Article/details/gviygzkph.sHtML

SQL ............ 90
来源：http://3g.hesvh.cn/Article/details/gsfvawolk.sHtML

Bash ........... 80
来源：http://www.share.hesvh.cn/Article/details/gdqvljlbv.sHtML

Kotlin ......... 15
来源：http://blog.hesvh.cn/Article/details/gliudcrtr.sHtML

Swift .......... 15
来源：http://baike.fehbvm.com/Article/details/gchijcfee.sHtML

Lua ............ 10
来源：http://3g.zdbjq.cn/Article/details/gavrqiztp.sHtML

Perl ........... 10
来源：http://baike.fehbvm.com/Article/details/gmuxnxgow.sHtML

Scala .......... 10
来源：http://mobile.zdbjq.cn/Article/details/gfaornhup.sHtML

------------------------------------
来源：http://m.share.hesvh.cn/Article/details/grljxzjdh.sHtML

合计 ........... 2106 条
来源：http://3g.zdbjq.cn/Article/details/gdzewnnto.sHtML

按章节统计：
来源：http://m.share.hesvh.cn/Article/details/gzhwscmlt.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.fehbvm.com/Article/details/gjcmmqxsp.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wap.zdbjq.cn/Article/details/gszfmrwoe.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://m.share.hesvh.cn/Article/details/gpsmxklyw.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://m.share.zdbjq.cn/Article/details/glxdyirey.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.m.share.hesvh.cn/Article/details/gnmvvzknv.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://baike.hesvh.cn/Article/details/gravkshzh.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.share.hesvh.cn/Article/details/giobefxln.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.blog.zdbjq.cn/Article/details/gmpmiktaq.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.blog.fehbvm.com/Article/details/ghdtadkfk.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.share.hesvh.cn/Article/details/giivrfgkl.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.m.share.zdbjq.cn/Article/details/glrtjddsi.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.share.zdbjq.cn/Article/details/gawufteoe.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.m.share.zdbjq.cn/Article/details/gdpdgrnuf.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://baike.hesvh.cn/Article/details/gpuoavafo.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.blog.fehbvm.com/Article/details/gvgsjekxd.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://blog.fehbvm.com/Article/details/gkwzvjrmd.sHtML

Q SQL 专题                              90
来源：http://read.share.zdbjq.cn/Article/details/gqtuuvnfz.sHtML

R Bash 专题                             80
来源：http://blog.zdbjq.cn/Article/details/gtioztbur.sHtML

S C / C++ 专题                          60
来源：http://wap.fehbvm.com/Article/details/gfifjjtwy.sHtML

T 其他语言补充                          60
来源：http://read.share.zdbjq.cn/Article/details/gtwhswhnw.sHtML

U 高频实用片段                         120
来源：http://3g.zdbjq.cn/Article/details/gzcpvmvre.sHtML

------------------------------------
来源：http://www.share.hesvh.cn/Article/details/gqczcjtjc.sHtML

合计                                  2106 条
来源：http://read.share.hesvh.cn/Article/details/gwxdnpzkw.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fehbvm.com/Article/details/gztrczldk.sHtML

使用提醒
来源：http://www.share.zdbjq.cn/Article/details/ggmbpqrun.sHtML

--------------------------------------------------------------------------------
来源：http://baike.hesvh.cn/Article/details/gdlbrqubx.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.blog.hesvh.cn/Article/details/gtgulotkb.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://blog.fehbvm.com/Article/details/gduikoyqo.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.share.hesvh.cn/Article/details/gmevrfqen.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.m.share.zdbjq.cn/Article/details/gqggrnmzc.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.blog.hesvh.cn/Article/details/glzfkqjvv.sHtML

—— 文件结束 ——
来源：http://www.blog.hesvh.cn/Article/details/gwskyotja.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gcjmxgmwf.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.share.hesvh.cn/Article/details/gispzhbnn.sHtML

Common Programming Examples Cheat Book
来源：http://m.share.zdbjq.cn/Article/details/gpbgzutzg.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gftauxxth.sHtML

【收录内容】
来源：http://read.share.hesvh.cn/Article/details/gponnwsie.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.share.hesvh.cn/Article/details/glhiqpqiu.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://baike.fehbvm.com/Article/details/gtbhkwwbg.sHtML

SQL · Bash · C · C++
来源：http://mobile.fehbvm.com/Article/details/gtdtrldil.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.share.zdbjq.cn/Article/details/gwbwhkrdl.sHtML

【使用说明】
来源：http://www.blog.fehbvm.com/Article/details/glpnpjrjz.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://m.share.hesvh.cn/Article/details/ggcybekcb.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.share.hesvh.cn/Article/details/ggpqxltpg.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://baike.hesvh.cn/Article/details/gkonqnikm.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://m.share.zdbjq.cn/Article/details/ghyrhikva.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://m.share.zdbjq.cn/Article/details/gadfzopij.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://read.share.fehbvm.com/Article/details/gqclqkqxv.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://baike.fehbvm.com/Article/details/ggrpqwchv.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.share.fehbvm.com/Article/details/gohtejxhe.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://mobile.fehbvm.com/Article/details/gvwwzewzs.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://blog.fehbvm.com/Article/details/geamwatlb.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://read.share.fehbvm.com/Article/details/gatiwrlnp.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://wap.fehbvm.com/Article/details/ghwljvzvu.sHtML

【文件统计】
来源：http://www.blog.zdbjq.cn/Article/details/gqglodiif.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://3g.fehbvm.com/Article/details/gdziosjis.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.hesvh.cn/Article/details/gajkkicpv.sHtML

目  录
来源：http://www.m.share.hesvh.cn/Article/details/gzlteqkax.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.zdbjq.cn/Article/details/gqmdxoqni.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://wap.hesvh.cn/Article/details/gyznwmxpg.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://baike.zdbjq.cn/Article/details/gqikjksxc.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://read.share.fehbvm.com/Article/details/gomuwvfiu.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.m.share.fehbvm.com/Article/details/gdxvqhwcu.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://m.share.zdbjq.cn/Article/details/gwohjjgno.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://wap.hesvh.cn/Article/details/gtzhvdnej.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.blog.zdbjq.cn/Article/details/gktzchrpg.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://blog.fehbvm.com/Article/details/gaqpccfiy.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://blog.zdbjq.cn/Article/details/gphryqywc.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://3g.hesvh.cn/Article/details/glutvvtsv.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.blog.zdbjq.cn/Article/details/gvtxdxfni.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.share.zdbjq.cn/Article/details/gpkozmosh.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://3g.hesvh.cn/Article/details/geiwmatls.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://wap.fehbvm.com/Article/details/gbsxgbouy.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://blog.hesvh.cn/Article/details/gqtpkcgup.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://mobile.zdbjq.cn/Article/details/gapfxoupl.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://blog.zdbjq.cn/Article/details/gyzsnupgz.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://m.share.fehbvm.com/Article/details/gaczpqtvj.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://blog.hesvh.cn/Article/details/gxzuleopt.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.zdbjq.cn/Article/details/gvrsonjuc.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://3g.hesvh.cn/Article/details/gtkpzirnk.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gitfuaquo.sHtML

A. 基础语法与类型
来源：http://wap.hesvh.cn/Article/details/gtdbrqeye.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gtasqkvyy.sHtML

[A01] Hello World
来源：http://wap.fehbvm.com/Article/details/gnhdgrsly.sHtML

Py:   print("Hello, World!")
来源：http://wap.zdbjq.cn/Article/details/gunauuqch.sHtML

PHP:  echo "Hello, World!";
来源：http://wap.zdbjq.cn/Article/details/gmhdfsvba.sHtML

JS:   console.log("Hello, World!");
来源：http://blog.zdbjq.cn/Article/details/ghmrlxvuq.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://m.share.zdbjq.cn/Article/details/gpiexsaqo.sHtML

Java: System.out.println("Hello, World!");
来源：http://blog.fehbvm.com/Article/details/gemkewabo.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.m.share.hesvh.cn/Article/details/gckmdjmet.sHtML

Ruby: puts "Hello, World!"
来源：http://m.share.hesvh.cn/Article/details/gptfdxpvi.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://blog.hesvh.cn/Article/details/gylhqxyuz.sHtML

[A02] 变量声明与赋值
来源：http://3g.zdbjq.cn/Article/details/gbbljgrtq.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://3g.zdbjq.cn/Article/details/gulmngxzz.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://wap.hesvh.cn/Article/details/glzcumjgg.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://read.share.zdbjq.cn/Article/details/gogfbatox.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://read.share.hesvh.cn/Article/details/gzudmnfvw.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://3g.fehbvm.com/Article/details/gwlxxmuka.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.blog.zdbjq.cn/Article/details/goqbscuzs.sHtML

Ruby: name = "Alex"; age = 20
来源：http://blog.fehbvm.com/Article/details/gbotkrvjs.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://baike.zdbjq.cn/Article/details/guiyvztyu.sHtML

[A03] 常量定义
来源：http://mobile.hesvh.cn/Article/details/gawpbmsdy.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://baike.fehbvm.com/Article/details/gykimliaa.sHtML

PHP:  const PI = 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/gpmxaqlis.sHtML

JS:   const PI = 3.14159;
来源：http://blog.fehbvm.com/Article/details/grknykheg.sHtML

TS:   const PI: number = 3.14159;
来源：http://blog.hesvh.cn/Article/details/gpagtetsy.sHtML

Java: static final double PI = 3.14159;
来源：http://3g.zdbjq.cn/Article/details/gfltnvoyf.sHtML

Go:   const PI = 3.14159
来源：http://m.share.fehbvm.com/Article/details/gouwjxspi.sHtML

Ruby: PI = 3.14159
来源：http://www.share.hesvh.cn/Article/details/gdagpofgc.sHtML

C#:   const double PI = 3.14159;
来源：http://mobile.fehbvm.com/Article/details/ggxtjorzs.sHtML

[A04] 判断变量类型
来源：http://m.share.zdbjq.cn/Article/details/gbtbnztgy.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.m.share.fehbvm.com/Article/details/ghwxqmlxq.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://m.share.fehbvm.com/Article/details/gstsegbgb.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://m.share.fehbvm.com/Article/details/gezaflera.sHtML

TS:   typeof x; x instanceof Date
来源：http://blog.hesvh.cn/Article/details/gdgvbxhec.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://baike.fehbvm.com/Article/details/ggqtqynns.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.share.fehbvm.com/Article/details/gnctflksn.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.blog.hesvh.cn/Article/details/gcatpydbh.sHtML

C#:   x.GetType().Name; x is int
来源：http://3g.hesvh.cn/Article/details/gaozywxmo.sHtML

[A05] 整数除法与取模
来源：http://www.blog.hesvh.cn/Article/details/gzmoxofjf.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.share.hesvh.cn/Article/details/glxjzacek.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://m.share.hesvh.cn/Article/details/gnculmxik.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.blog.hesvh.cn/Article/details/gxzjuecll.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.zdbjq.cn/Article/details/grmuvukdc.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.blog.zdbjq.cn/Article/details/gvshudrma.sHtML

Go:   7 / 2; 7 % 2
来源：http://read.share.hesvh.cn/Article/details/gndeldkzd.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.blog.zdbjq.cn/Article/details/gghmigxiw.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.m.share.zdbjq.cn/Article/details/gzpkjglnb.sHtML

[A06] 字符串转数字
来源：http://m.share.fehbvm.com/Article/details/gmpiuyvnb.sHtML

Py:   int("42"); float("3.14")
来源：http://www.share.zdbjq.cn/Article/details/gfbkeljfg.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://wap.zdbjq.cn/Article/details/gphjrqdde.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://blog.fehbvm.com/Article/details/gtvktamwy.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.share.fehbvm.com/Article/details/gxrmoeijj.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.m.share.fehbvm.com/Article/details/grafcczth.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://read.share.hesvh.cn/Article/details/ggiovpmvh.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://3g.zdbjq.cn/Article/details/gzxrsnmxk.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://blog.hesvh.cn/Article/details/gmjuysrwo.sHtML

[A07] 数字转字符串
来源：http://mobile.hesvh.cn/Article/details/gjemdtgho.sHtML

Py:   str(42)
来源：http://www.share.hesvh.cn/Article/details/gthlxomuq.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.m.share.hesvh.cn/Article/details/gvoshzuky.sHtML

JS:   String(42); (42).toString()
来源：http://wap.hesvh.cn/Article/details/gmdkzqqaj.sHtML

TS:   String(42)
来源：http://3g.zdbjq.cn/Article/details/gxnaxllev.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.share.hesvh.cn/Article/details/gdxowhosb.sHtML

Go:   strconv.Itoa(42)
来源：http://baike.fehbvm.com/Article/details/ggupnjweg.sHtML

Ruby: 42.to_s
来源：http://read.share.fehbvm.com/Article/details/ggfqxkpgh.sHtML

C#:   42.ToString()
来源：http://www.share.hesvh.cn/Article/details/gvevlujaa.sHtML

[A08] 取整与四舍五入
来源：http://www.blog.zdbjq.cn/Article/details/gdkmjhgxy.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://read.share.hesvh.cn/Article/details/gvoebuvpf.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://blog.zdbjq.cn/Article/details/gvcvijtzk.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.blog.zdbjq.cn/Article/details/ghbqdalvm.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://3g.fehbvm.com/Article/details/glgowznzp.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://mobile.hesvh.cn/Article/details/gkvetviyv.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://baike.fehbvm.com/Article/details/gdspnnwuo.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://blog.hesvh.cn/Article/details/gnuoexmqf.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://3g.fehbvm.com/Article/details/gidudwnan.sHtML

[A09] 绝对值与最大最小值
来源：http://www.share.zdbjq.cn/Article/details/gfuunrjpn.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.share.fehbvm.com/Article/details/gbgsdoies.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.m.share.hesvh.cn/Article/details/gcrsvbggk.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.m.share.fehbvm.com/Article/details/gramkxvqo.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://baike.hesvh.cn/Article/details/geajmubad.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://m.share.fehbvm.com/Article/details/grlecaodg.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.share.zdbjq.cn/Article/details/gkimdixxq.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.blog.fehbvm.com/Article/details/gmmfcgtam.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.share.fehbvm.com/Article/details/ghurvkbyb.sHtML

[A10] 生成随机数
来源：http://www.share.zdbjq.cn/Article/details/ggnuvacli.sHtML

Py:   import random; random.randint(1, 100)
来源：http://mobile.fehbvm.com/Article/details/gdacnkkox.sHtML

PHP:  random_int(1, 100);
来源：http://m.share.zdbjq.cn/Article/details/gruaolhht.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://baike.zdbjq.cn/Article/details/gzvprufvp.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://mobile.fehbvm.com/Article/details/gdczzstza.sHtML

Java: new Random().nextInt(100) + 1
来源：http://baike.zdbjq.cn/Article/details/gsodegbie.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://blog.fehbvm.com/Article/details/gwduibrnh.sHtML

Ruby: rand(1..100)
来源：http://m.share.zdbjq.cn/Article/details/gfmdiggcy.sHtML


<!-- 参考信息 -->