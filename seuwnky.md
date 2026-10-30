代发 wailian999

[U67] PHP：处理文件上传
来源：http://3g.fehbvm.com/Article/details/gmmejwhtq.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://baike.fehbvm.com/Article/details/gcaoiolgf.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.hesvh.cn/Article/details/grzwjcior.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.m.share.hesvh.cn/Article/details/gvkdcvkai.sHtML

[U69] PHP：PDO 预处理
来源：http://mobile.fehbvm.com/Article/details/gpsxcxsyq.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://read.share.hesvh.cn/Article/details/gygdusabn.sHtML

[U70] PHP：PDO 事务
来源：http://wap.fehbvm.com/Article/details/ghvwwvzhm.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://3g.zdbjq.cn/Article/details/gpuoxcrcf.sHtML

[U71] PHP：抛出异常
来源：http://blog.hesvh.cn/Article/details/gzntvqxqk.sHtML

throw new RuntimeException("失败", 500);
来源：http://m.share.fehbvm.com/Article/details/gvxdqfyte.sHtML

[U72] PHP：写错误日志
来源：http://wap.fehbvm.com/Article/details/guucqmaca.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.blog.zdbjq.cn/Article/details/gsvboezyu.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.blog.fehbvm.com/Article/details/grsxhwoaz.sHtML

parse_ini_file("config.ini", true)
来源：http://www.m.share.fehbvm.com/Article/details/ghykppasu.sHtML

[U74] PHP：读取环境变量
来源：http://wap.fehbvm.com/Article/details/givauehed.sHtML

getenv("APP_ENV") ?: "production"
来源：http://read.share.zdbjq.cn/Article/details/gapzofunw.sHtML

[U75] PHP：依赖注入
来源：http://3g.fehbvm.com/Article/details/gbxqguyvg.sHtML

composer require psr/container
来源：http://www.share.fehbvm.com/Article/details/ghqlhehgk.sHtML

[U76] PHP：简单路由
来源：http://blog.hesvh.cn/Article/details/gjugiktyv.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://m.share.hesvh.cn/Article/details/gqjhicpxm.sHtML

[U77] PHP：模板渲染
来源：http://3g.zdbjq.cn/Article/details/gfubofaus.sHtML

composer require twig/twig
来源：http://read.share.fehbvm.com/Article/details/gugrtdvng.sHtML

[U78] PHP：单元测试
来源：http://wap.zdbjq.cn/Article/details/gfirmjqai.sHtML

composer require --dev phpunit/phpunit
来源：http://baike.fehbvm.com/Article/details/gvzrnyltt.sHtML

[U79] PHP：静态分析
来源：http://mobile.zdbjq.cn/Article/details/gztkfmnrm.sHtML

composer require --dev phpstan/phpstan
来源：http://www.m.share.hesvh.cn/Article/details/gpbgxtxnr.sHtML

[U80] PHP：代码规范修复
来源：http://wap.fehbvm.com/Article/details/gwcmzzqnm.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://baike.zdbjq.cn/Article/details/gdeqqwxtr.sHtML

[U81] JS：初始化项目
来源：http://wap.zdbjq.cn/Article/details/gpozcwolf.sHtML

npm init -y;  npm i express
来源：http://wap.zdbjq.cn/Article/details/gbgkhtaad.sHtML

[U82] JS：package.json 脚本
来源：http://3g.zdbjq.cn/Article/details/goyhwjasj.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mobile.hesvh.cn/Article/details/gptjgsxfc.sHtML

[U83] JS：ES Module 导入导出
来源：http://blog.hesvh.cn/Article/details/gvficfvug.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://m.share.zdbjq.cn/Article/details/gwbrdjpkp.sHtML

[U84] JS：CommonJS 写法
来源：http://mobile.hesvh.cn/Article/details/gcisjmyfi.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://wap.fehbvm.com/Article/details/gzrwatlma.sHtML

[U85] JS：可选链
来源：http://read.share.zdbjq.cn/Article/details/gfmywxwxs.sHtML

a?.b?.c
来源：http://3g.zdbjq.cn/Article/details/gjpdtybnq.sHtML

[U86] JS：空值合并
来源：http://baike.hesvh.cn/Article/details/ggpvcgwnw.sHtML

a ?? b
来源：http://www.m.share.fehbvm.com/Article/details/gnibfyzfm.sHtML

[U87] JS：解构默认值
来源：http://www.blog.hesvh.cn/Article/details/giuxqrtva.sHtML

const { a = 1, b = 2 } = obj;
来源：http://read.share.hesvh.cn/Article/details/gbnqxfxys.sHtML

[U88] JS：对象展开合并
来源：http://wap.hesvh.cn/Article/details/gumwxsuee.sHtML

{ ...a, ...b }
来源：http://www.share.fehbvm.com/Article/details/grdkdglyf.sHtML

[U89] JS：数组去重
来源：http://wap.zdbjq.cn/Article/details/geogmzrva.sHtML

[...new Set(arr)]
来源：http://www.blog.hesvh.cn/Article/details/gmsrhuazy.sHtML

[U90] JS：数字数组排序
来源：http://wap.fehbvm.com/Article/details/glckoeirk.sHtML

[...arr].sort((a, b) => a - b)
来源：http://m.share.hesvh.cn/Article/details/gsddjeyev.sHtML

[U91] JS：对象键值遍历
来源：http://wap.zdbjq.cn/Article/details/gqbyerfjj.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mobile.zdbjq.cn/Article/details/gmqswwghr.sHtML

[U92] JS：深拷贝
来源：http://mobile.fehbvm.com/Article/details/giqyuzifq.sHtML

structuredClone(obj)
来源：http://www.share.hesvh.cn/Article/details/ggtylowhu.sHtML

[U93] JS：模板字符串
来源：http://www.blog.fehbvm.com/Article/details/gaeznnatz.sHtML

`共 ${n} 条`
来源：http://blog.hesvh.cn/Article/details/gfnlnhfqi.sHtML

[U94] JS：箭头函数
来源：http://www.blog.zdbjq.cn/Article/details/gkiotqeqg.sHtML

const double = x => x * 2;
来源：http://wap.hesvh.cn/Article/details/gbkktedpl.sHtML

[U95] JS：Promise 包装
来源：http://read.share.hesvh.cn/Article/details/gnbjhdiqj.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.zdbjq.cn/Article/details/gtlsutsnp.sHtML

[U96] JS：async/await 与异常
来源：http://www.share.zdbjq.cn/Article/details/gzapulzfv.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://baike.hesvh.cn/Article/details/gbwmyovji.sHtML

[U97] JS：并发请求
来源：http://m.share.zdbjq.cn/Article/details/gpalruxad.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fehbvm.com/Article/details/gwzjgcgsq.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.m.share.hesvh.cn/Article/details/gxbxjszxe.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.share.fehbvm.com/Article/details/goedrmthn.sHtML

[U99] JS：事件监听
来源：http://m.share.zdbjq.cn/Article/details/gkxvoflui.sHtML

el.addEventListener("click", e => {})
来源：http://read.share.fehbvm.com/Article/details/gapvbtklx.sHtML

[U100] JS：DOM 查询
来源：http://www.m.share.fehbvm.com/Article/details/gxdouqfur.sHtML

document.querySelector(".item")
来源：http://www.share.zdbjq.cn/Article/details/gcrzlojaj.sHtML

[U101] JS：classList 操作
来源：http://m.share.fehbvm.com/Article/details/gjznakpjp.sHtML

el.classList.toggle("active")
来源：http://mobile.zdbjq.cn/Article/details/gcfnvfklj.sHtML

[U102] JS：本地存储
来源：http://read.share.zdbjq.cn/Article/details/gcbvqsubp.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://3g.zdbjq.cn/Article/details/gadxbfnth.sHtML

[U103] JS：定时器
来源：http://blog.fehbvm.com/Article/details/gvmeyduno.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://3g.fehbvm.com/Article/details/gtrsobphb.sHtML

[U104] JS：防抖
来源：http://blog.fehbvm.com/Article/details/gtyhujjvq.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.zdbjq.cn/Article/details/glzizkisk.sHtML

[U105] JS：节流
来源：http://www.share.hesvh.cn/Article/details/gpttowyml.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mobile.fehbvm.com/Article/details/guianoppv.sHtML

[U106] JS：日期格式化
来源：http://3g.fehbvm.com/Article/details/gwpudjuhy.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://baike.zdbjq.cn/Article/details/gjlzsmehf.sHtML

[U107] JS：数字千分位
来源：http://mobile.zdbjq.cn/Article/details/gnczziyzm.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://baike.zdbjq.cn/Article/details/gnuakfnkp.sHtML

[U108] JS：随机整数
来源：http://read.share.fehbvm.com/Article/details/gjazzpbgz.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.hesvh.cn/Article/details/gmfjojjjy.sHtML

[U109] JS：数组分组
来源：http://wap.fehbvm.com/Article/details/gconuqrfl.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.m.share.hesvh.cn/Article/details/gjfpsrzur.sHtML

[U110] JS：数组分块
来源：http://www.blog.zdbjq.cn/Article/details/gvedetels.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://m.share.zdbjq.cn/Article/details/gkzrigfwx.sHtML

[U111] JS：对象转 Map
来源：http://wap.zdbjq.cn/Article/details/gqautxohg.sHtML

new Map(Object.entries(obj))
来源：http://m.share.fehbvm.com/Article/details/gmfqcpqfh.sHtML

[U112] JS：字符串补位
来源：http://blog.hesvh.cn/Article/details/gqnqtuluk.sHtML

"7".padStart(3, "0")
来源：http://mobile.fehbvm.com/Article/details/gqtdivsri.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.zdbjq.cn/Article/details/gcusnuchz.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/glwvddovm.sHtML

[U114] JS：JSON 深比较
来源：http://wap.zdbjq.cn/Article/details/gxortqeps.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.fehbvm.com/Article/details/gsyuanywf.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.zdbjq.cn/Article/details/gppslbxdy.sHtML

crypto.randomUUID()
来源：http://3g.zdbjq.cn/Article/details/gkoyaudvl.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.hesvh.cn/Article/details/gzcswmltr.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.m.share.zdbjq.cn/Article/details/ghlwgobxo.sHtML

[U117] JS：单元测试
来源：http://mobile.zdbjq.cn/Article/details/gopjcdnzd.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.hesvh.cn/Article/details/ganktqwxk.sHtML

[U118] JS：开发服务器
来源：http://baike.fehbvm.com/Article/details/gabydzeud.sHtML

npm i -D vite;  npx vite
来源：http://www.share.zdbjq.cn/Article/details/gwamxxrbj.sHtML

[U119] JS：生产构建
来源：http://read.share.fehbvm.com/Article/details/gfezrbgry.sHtML

npx vite build
来源：http://mobile.fehbvm.com/Article/details/gazmfggga.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://read.share.hesvh.cn/Article/details/gnejqejjx.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.hesvh.cn/Article/details/girviodqv.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gcdxbopkl.sHtML

统计汇总
来源：http://wap.fehbvm.com/Article/details/ghkfnoevv.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/ghhluqthb.sHtML

按语言统计（条）：
来源：http://www.blog.hesvh.cn/Article/details/gmzgbnxos.sHtML

Python ......... 252
来源：http://3g.hesvh.cn/Article/details/gqptplpai.sHtML

PHP ............ 252
来源：http://mobile.zdbjq.cn/Article/details/giegcevla.sHtML

JavaScript ..... 252
来源：http://www.share.zdbjq.cn/Article/details/goquekiif.sHtML

TypeScript ..... 212
来源：http://read.share.hesvh.cn/Article/details/ghqhwifml.sHtML

Java ........... 212
来源：http://blog.hesvh.cn/Article/details/gdfkonuui.sHtML

Go ............. 212
来源：http://wap.fehbvm.com/Article/details/grgshjksw.sHtML

Ruby ........... 212
来源：http://3g.fehbvm.com/Article/details/grkfhpqju.sHtML

C# ............. 212
来源：http://wap.zdbjq.cn/Article/details/gnbprkfeg.sHtML

C .............. 30
来源：http://3g.zdbjq.cn/Article/details/ghwnillpj.sHtML

C++ ............ 30
来源：http://www.m.share.fehbvm.com/Article/details/gvjmrnvph.sHtML

SQL ............ 90
来源：http://www.share.hesvh.cn/Article/details/gdjoiblcf.sHtML

Bash ........... 80
来源：http://www.blog.hesvh.cn/Article/details/gswuxyjck.sHtML

Kotlin ......... 15
来源：http://blog.hesvh.cn/Article/details/gzmttojlv.sHtML

Swift .......... 15
来源：http://3g.hesvh.cn/Article/details/ghxykzwud.sHtML

Lua ............ 10
来源：http://mobile.hesvh.cn/Article/details/gwiexgxfb.sHtML

Perl ........... 10
来源：http://baike.fehbvm.com/Article/details/gpcbzdyya.sHtML

Scala .......... 10
来源：http://wap.hesvh.cn/Article/details/gbdtbxiqg.sHtML

------------------------------------
来源：http://www.blog.zdbjq.cn/Article/details/gznqegavi.sHtML

合计 ........... 2106 条
来源：http://www.blog.fehbvm.com/Article/details/gunslogmn.sHtML

按章节统计：
来源：http://baike.fehbvm.com/Article/details/gnlbzrkab.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://baike.hesvh.cn/Article/details/gcsbyjatp.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mobile.fehbvm.com/Article/details/gvcqlmosy.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://3g.zdbjq.cn/Article/details/giwhzvbbt.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.share.fehbvm.com/Article/details/gxtbwfopw.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.share.hesvh.cn/Article/details/ggjuwxujh.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.blog.fehbvm.com/Article/details/gfykesmfo.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mobile.fehbvm.com/Article/details/girkfnuyt.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.m.share.zdbjq.cn/Article/details/gnijnyqhe.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://m.share.hesvh.cn/Article/details/ggaoulbhb.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wap.fehbvm.com/Article/details/gozudftgu.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://blog.fehbvm.com/Article/details/gfguxjnoj.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.share.hesvh.cn/Article/details/gkqrawtvi.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://read.share.hesvh.cn/Article/details/gimevweoe.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://m.share.hesvh.cn/Article/details/gwrheybaa.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://3g.fehbvm.com/Article/details/gvzuanylo.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.blog.fehbvm.com/Article/details/gzkspkhzz.sHtML

Q SQL 专题                              90
来源：http://m.share.zdbjq.cn/Article/details/gtsemxdkn.sHtML

R Bash 专题                             80
来源：http://baike.fehbvm.com/Article/details/gptdnzyju.sHtML

S C / C++ 专题                          60
来源：http://3g.hesvh.cn/Article/details/gobpvaaaw.sHtML

T 其他语言补充                          60
来源：http://baike.hesvh.cn/Article/details/gbjheplhg.sHtML

U 高频实用片段                         120
来源：http://www.m.share.zdbjq.cn/Article/details/gcboutvtw.sHtML

------------------------------------
来源：http://m.share.zdbjq.cn/Article/details/gimwaeglf.sHtML

合计                                  2106 条
来源：http://3g.fehbvm.com/Article/details/gkddxlofx.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/gkddigsfq.sHtML

使用提醒
来源：http://read.share.fehbvm.com/Article/details/ghmyxjeot.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.zdbjq.cn/Article/details/gvurobwip.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.blog.zdbjq.cn/Article/details/gwvpmgoyj.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://read.share.hesvh.cn/Article/details/gorsolihq.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://wap.fehbvm.com/Article/details/gwdlwbmbz.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://m.share.zdbjq.cn/Article/details/gddhzfvmf.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://3g.zdbjq.cn/Article/details/giarrlaed.sHtML

—— 文件结束 ——
来源：http://read.share.zdbjq.cn/Article/details/ggrfgcupm.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gdxjbnuhg.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://blog.fehbvm.com/Article/details/guwwfqpii.sHtML

Common Programming Examples Cheat Book
来源：http://www.blog.fehbvm.com/Article/details/gydsnpjtg.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gsvqucuyp.sHtML

【收录内容】
来源：http://wap.fehbvm.com/Article/details/ghnllavqr.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://mobile.fehbvm.com/Article/details/gtuosgsxg.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.share.hesvh.cn/Article/details/gwxrmbqmi.sHtML

SQL · Bash · C · C++
来源：http://m.share.hesvh.cn/Article/details/gxrokiyvg.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.share.zdbjq.cn/Article/details/gjcajzaqg.sHtML

【使用说明】
来源：http://read.share.fehbvm.com/Article/details/gdtxjjslz.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.blog.hesvh.cn/Article/details/gnsfhgomf.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://mobile.hesvh.cn/Article/details/gbbrgjmwa.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://3g.zdbjq.cn/Article/details/ggcfpvoyy.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://m.share.fehbvm.com/Article/details/gcjppuyjy.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.m.share.hesvh.cn/Article/details/gwbtyecqd.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://mobile.fehbvm.com/Article/details/gdwlampbo.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.m.share.fehbvm.com/Article/details/gaenhligz.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://wap.fehbvm.com/Article/details/gjqxgabvc.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.blog.hesvh.cn/Article/details/gubjchqdd.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://baike.zdbjq.cn/Article/details/gsyranvuz.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mobile.fehbvm.com/Article/details/grniljezn.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.share.zdbjq.cn/Article/details/guryerfje.sHtML

【文件统计】
来源：http://m.share.fehbvm.com/Article/details/glzdmpsoe.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://mobile.hesvh.cn/Article/details/gvcxhvtix.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.fehbvm.com/Article/details/gnfbcpmhy.sHtML

目  录
来源：http://www.share.fehbvm.com/Article/details/gvkzxprhw.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fehbvm.com/Article/details/gvusgfjti.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.share.hesvh.cn/Article/details/gmnryovhq.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.blog.hesvh.cn/Article/details/glxrhwbjg.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://wap.fehbvm.com/Article/details/gbfawtelj.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.m.share.hesvh.cn/Article/details/gtvihqcdr.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.share.zdbjq.cn/Article/details/gxfjgcnnm.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://blog.hesvh.cn/Article/details/gajmysnit.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://wap.hesvh.cn/Article/details/gemhsobnc.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://wap.zdbjq.cn/Article/details/gzplfxkee.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://wap.zdbjq.cn/Article/details/gvzgwnpai.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://baike.hesvh.cn/Article/details/ggwkgfquy.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://read.share.hesvh.cn/Article/details/gphhqgmyv.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://read.share.hesvh.cn/Article/details/gzrgarbar.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://blog.fehbvm.com/Article/details/ggiusmbei.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://blog.zdbjq.cn/Article/details/gpzsjedab.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://read.share.hesvh.cn/Article/details/gwhdjvnhn.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://baike.hesvh.cn/Article/details/gqimuohnw.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.share.hesvh.cn/Article/details/grmcwefif.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.share.fehbvm.com/Article/details/gpqspdpoa.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.m.share.fehbvm.com/Article/details/gofpkejel.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.fehbvm.com/Article/details/gdelotvze.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://read.share.zdbjq.cn/Article/details/gijzfemyu.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gnvqwfzns.sHtML

A. 基础语法与类型
来源：http://read.share.zdbjq.cn/Article/details/ggimcgazp.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/ggdweixba.sHtML

[A01] Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gudndpkgk.sHtML

Py:   print("Hello, World!")
来源：http://baike.fehbvm.com/Article/details/grcpqaeqp.sHtML

PHP:  echo "Hello, World!";
来源：http://m.share.zdbjq.cn/Article/details/gvnlvaldi.sHtML

JS:   console.log("Hello, World!");
来源：http://read.share.zdbjq.cn/Article/details/gckqaaxww.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://wap.hesvh.cn/Article/details/gjevshyyy.sHtML

Java: System.out.println("Hello, World!");
来源：http://m.share.hesvh.cn/Article/details/gkaivcoqe.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.blog.fehbvm.com/Article/details/gnjkzklwc.sHtML

Ruby: puts "Hello, World!"
来源：http://baike.zdbjq.cn/Article/details/gjicnvgub.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://mobile.hesvh.cn/Article/details/gmvarpuxk.sHtML

[A02] 变量声明与赋值
来源：http://mobile.fehbvm.com/Article/details/gktjlflqt.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://3g.zdbjq.cn/Article/details/gaquubojn.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://m.share.zdbjq.cn/Article/details/gzyimujnb.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://read.share.zdbjq.cn/Article/details/ghqjriijk.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.share.hesvh.cn/Article/details/gvetifslz.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://wap.fehbvm.com/Article/details/giphraqos.sHtML

Go:   name := "Alex"; age := 20
来源：http://baike.hesvh.cn/Article/details/gusmtmtlc.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.share.hesvh.cn/Article/details/gfpynwdwq.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://baike.fehbvm.com/Article/details/ghshpypds.sHtML

[A03] 常量定义
来源：http://wap.fehbvm.com/Article/details/ggolfnvek.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://read.share.zdbjq.cn/Article/details/gdviwbzyw.sHtML

PHP:  const PI = 3.14159;
来源：http://m.share.fehbvm.com/Article/details/ghdgavxaa.sHtML

JS:   const PI = 3.14159;
来源：http://blog.zdbjq.cn/Article/details/gradmqsuh.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.share.fehbvm.com/Article/details/gtqmicdrg.sHtML

Java: static final double PI = 3.14159;
来源：http://baike.zdbjq.cn/Article/details/gnkgbduvt.sHtML

Go:   const PI = 3.14159
来源：http://mobile.zdbjq.cn/Article/details/gpywucdhj.sHtML

Ruby: PI = 3.14159
来源：http://www.share.zdbjq.cn/Article/details/gjjzpbggy.sHtML

C#:   const double PI = 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/ggjdsasqi.sHtML

[A04] 判断变量类型
来源：http://www.blog.hesvh.cn/Article/details/gxcetoglc.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://3g.hesvh.cn/Article/details/gjgdmqssn.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.m.share.hesvh.cn/Article/details/gaeloqbtk.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.blog.fehbvm.com/Article/details/gkuhuwzcb.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.m.share.hesvh.cn/Article/details/gmwspotvx.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.share.zdbjq.cn/Article/details/gpgecnzyf.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://wap.hesvh.cn/Article/details/gtphmcscx.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://m.share.zdbjq.cn/Article/details/gefglsrjo.sHtML

C#:   x.GetType().Name; x is int
来源：http://mobile.fehbvm.com/Article/details/gflyyeuxv.sHtML

[A05] 整数除法与取模
来源：http://mobile.fehbvm.com/Article/details/gdqgeqhhs.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://read.share.zdbjq.cn/Article/details/gtkmppjdo.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://read.share.hesvh.cn/Article/details/goefcjnxo.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.fehbvm.com/Article/details/gyaqlujqj.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.fehbvm.com/Article/details/gukwahgsz.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.blog.zdbjq.cn/Article/details/gokbfujzl.sHtML

Go:   7 / 2; 7 % 2
来源：http://m.share.hesvh.cn/Article/details/gwpvgimru.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://blog.hesvh.cn/Article/details/gpvstdzak.sHtML

C#:   7 / 2; 7 % 2
来源：http://wap.fehbvm.com/Article/details/gnwbmnkeb.sHtML

[A06] 字符串转数字
来源：http://3g.hesvh.cn/Article/details/gdqxapccj.sHtML

Py:   int("42"); float("3.14")
来源：http://www.blog.fehbvm.com/Article/details/ghbjubcqk.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.blog.hesvh.cn/Article/details/gmfuarngo.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.share.fehbvm.com/Article/details/ghqjurqco.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://baike.zdbjq.cn/Article/details/ggghgpgsd.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://baike.hesvh.cn/Article/details/ggpkahbqr.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.m.share.fehbvm.com/Article/details/ggeoavmmg.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://blog.zdbjq.cn/Article/details/gmljentin.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://read.share.zdbjq.cn/Article/details/ghuysoeiz.sHtML

[A07] 数字转字符串
来源：http://read.share.fehbvm.com/Article/details/gzvrevnkx.sHtML

Py:   str(42)
来源：http://wap.zdbjq.cn/Article/details/gyhptvdcx.sHtML

PHP:  (string) 42; strval(42)
来源：http://baike.fehbvm.com/Article/details/gjlmokcsi.sHtML

JS:   String(42); (42).toString()
来源：http://read.share.zdbjq.cn/Article/details/gzaokssvm.sHtML

TS:   String(42)
来源：http://m.share.hesvh.cn/Article/details/gytwnbkvy.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://3g.zdbjq.cn/Article/details/gxneoarii.sHtML

Go:   strconv.Itoa(42)
来源：http://read.share.fehbvm.com/Article/details/glvgrzfhn.sHtML

Ruby: 42.to_s
来源：http://blog.zdbjq.cn/Article/details/gltexrguf.sHtML

C#:   42.ToString()
来源：http://www.share.fehbvm.com/Article/details/gkopjhthr.sHtML

[A08] 取整与四舍五入
来源：http://3g.fehbvm.com/Article/details/gacsxdqmg.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://read.share.fehbvm.com/Article/details/gotqjvsqg.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.share.fehbvm.com/Article/details/givwylewy.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://m.share.zdbjq.cn/Article/details/gifcthfsl.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.blog.fehbvm.com/Article/details/gijhxfuyt.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.blog.hesvh.cn/Article/details/glpphfshe.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://m.share.zdbjq.cn/Article/details/ghkqzuunv.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://mobile.zdbjq.cn/Article/details/gkefjdqjl.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://wap.fehbvm.com/Article/details/gtsfucjki.sHtML

[A09] 绝对值与最大最小值
来源：http://www.share.zdbjq.cn/Article/details/gycrekwsw.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://blog.fehbvm.com/Article/details/gzoixagcj.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://mobile.fehbvm.com/Article/details/gpzjkepji.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://read.share.hesvh.cn/Article/details/glijnazya.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://read.share.zdbjq.cn/Article/details/gzqpjncgf.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://read.share.hesvh.cn/Article/details/ghdwoumdm.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.m.share.fehbvm.com/Article/details/goizexkvn.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.blog.zdbjq.cn/Article/details/gtkgvdajv.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://3g.hesvh.cn/Article/details/gpslhkogw.sHtML

[A10] 生成随机数
来源：http://www.m.share.hesvh.cn/Article/details/gkdyolveu.sHtML

Py:   import random; random.randint(1, 100)
来源：http://m.share.fehbvm.com/Article/details/gdqhxemdu.sHtML

PHP:  random_int(1, 100);
来源：http://m.share.zdbjq.cn/Article/details/gxlgbirjt.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://baike.hesvh.cn/Article/details/gzxucbter.sHtML


<!-- 参考信息 -->