代发 wailian999

[U69] PHP：PDO 预处理
来源：http://3g.hesvh.cn/Article/details/gttssjtxw.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mobile.zdbjq.cn/Article/details/gctzbrxib.sHtML

[U70] PHP：PDO 事务
来源：http://www.m.share.hesvh.cn/Article/details/gouytiphd.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://baike.hesvh.cn/Article/details/gfdisoive.sHtML

[U71] PHP：抛出异常
来源：http://blog.fehbvm.com/Article/details/ghckkypss.sHtML

throw new RuntimeException("失败", 500);
来源：http://read.share.hesvh.cn/Article/details/gvtofzwwj.sHtML

[U72] PHP：写错误日志
来源：http://read.share.zdbjq.cn/Article/details/gsuudgyyh.sHtML

error_log("失败: " . $e->getMessage());
来源：http://3g.zdbjq.cn/Article/details/ggprrqhzk.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.share.zdbjq.cn/Article/details/gbxljjtdz.sHtML

parse_ini_file("config.ini", true)
来源：http://blog.fehbvm.com/Article/details/gxorfeeiw.sHtML

[U74] PHP：读取环境变量
来源：http://mobile.zdbjq.cn/Article/details/gyjwxgcjs.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.zdbjq.cn/Article/details/gzgkpkqdz.sHtML

[U75] PHP：依赖注入
来源：http://read.share.hesvh.cn/Article/details/gxaqtomox.sHtML

composer require psr/container
来源：http://wap.hesvh.cn/Article/details/gvzowsweh.sHtML

[U76] PHP：简单路由
来源：http://baike.hesvh.cn/Article/details/gbjnfolmy.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://blog.fehbvm.com/Article/details/gxjkgllix.sHtML

[U77] PHP：模板渲染
来源：http://wap.fehbvm.com/Article/details/gfwzrgsji.sHtML

composer require twig/twig
来源：http://read.share.zdbjq.cn/Article/details/giykdavej.sHtML

[U78] PHP：单元测试
来源：http://www.blog.zdbjq.cn/Article/details/gxzdqvlnn.sHtML

composer require --dev phpunit/phpunit
来源：http://mobile.hesvh.cn/Article/details/gckvsurgo.sHtML

[U79] PHP：静态分析
来源：http://read.share.zdbjq.cn/Article/details/gxhvimssp.sHtML

composer require --dev phpstan/phpstan
来源：http://www.share.zdbjq.cn/Article/details/gqluqxyrl.sHtML

[U80] PHP：代码规范修复
来源：http://www.share.zdbjq.cn/Article/details/grsqscglc.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://mobile.hesvh.cn/Article/details/ggrcpzadu.sHtML

[U81] JS：初始化项目
来源：http://www.m.share.zdbjq.cn/Article/details/gquvpqxxo.sHtML

npm init -y;  npm i express
来源：http://blog.fehbvm.com/Article/details/gkcsiokgt.sHtML

[U82] JS：package.json 脚本
来源：http://wap.hesvh.cn/Article/details/gdsiuzhfb.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://m.share.fehbvm.com/Article/details/gdniyotbq.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.share.zdbjq.cn/Article/details/gurxptthk.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://read.share.fehbvm.com/Article/details/galnrnnqc.sHtML

[U84] JS：CommonJS 写法
来源：http://baike.hesvh.cn/Article/details/gykbtwcbb.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://baike.zdbjq.cn/Article/details/gdatrfdbl.sHtML

[U85] JS：可选链
来源：http://3g.zdbjq.cn/Article/details/gfkcuerpe.sHtML

a?.b?.c
来源：http://www.m.share.hesvh.cn/Article/details/gmiihkxzc.sHtML

[U86] JS：空值合并
来源：http://read.share.hesvh.cn/Article/details/glfvrpgio.sHtML

a ?? b
来源：http://www.share.hesvh.cn/Article/details/gtrjziqaf.sHtML

[U87] JS：解构默认值
来源：http://wap.fehbvm.com/Article/details/gbhwlzitf.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.fehbvm.com/Article/details/gwflcfivo.sHtML

[U88] JS：对象展开合并
来源：http://mobile.zdbjq.cn/Article/details/gqmxfuvwz.sHtML

{ ...a, ...b }
来源：http://3g.hesvh.cn/Article/details/gstsmttgx.sHtML

[U89] JS：数组去重
来源：http://www.share.fehbvm.com/Article/details/guvgxquiy.sHtML

[...new Set(arr)]
来源：http://3g.fehbvm.com/Article/details/gatqxwchk.sHtML

[U90] JS：数字数组排序
来源：http://www.blog.hesvh.cn/Article/details/gxycypwoz.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.share.fehbvm.com/Article/details/gtzqlsaul.sHtML

[U91] JS：对象键值遍历
来源：http://blog.fehbvm.com/Article/details/gwvskrfoc.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.m.share.fehbvm.com/Article/details/giwnwvrsd.sHtML

[U92] JS：深拷贝
来源：http://read.share.zdbjq.cn/Article/details/getgmismv.sHtML

structuredClone(obj)
来源：http://www.blog.fehbvm.com/Article/details/gpewwrwxd.sHtML

[U93] JS：模板字符串
来源：http://blog.zdbjq.cn/Article/details/glfrrbvhg.sHtML

`共 ${n} 条`
来源：http://www.blog.hesvh.cn/Article/details/gwungmxkf.sHtML

[U94] JS：箭头函数
来源：http://m.share.hesvh.cn/Article/details/gppbuyxun.sHtML

const double = x => x * 2;
来源：http://blog.hesvh.cn/Article/details/ghhqhslwc.sHtML

[U95] JS：Promise 包装
来源：http://m.share.hesvh.cn/Article/details/gqipjbdme.sHtML

new Promise((resolve, reject) => {})
来源：http://www.share.fehbvm.com/Article/details/gcalwneho.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.zdbjq.cn/Article/details/gavnfyuxr.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.share.hesvh.cn/Article/details/grthfniiu.sHtML

[U97] JS：并发请求
来源：http://blog.hesvh.cn/Article/details/gnymdddlr.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.zdbjq.cn/Article/details/gkwnopfjd.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.hesvh.cn/Article/details/gafdsnxno.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mobile.hesvh.cn/Article/details/gqdlhflfm.sHtML

[U99] JS：事件监听
来源：http://www.m.share.hesvh.cn/Article/details/gngujjngn.sHtML

el.addEventListener("click", e => {})
来源：http://www.m.share.zdbjq.cn/Article/details/gghaboiui.sHtML

[U100] JS：DOM 查询
来源：http://www.blog.fehbvm.com/Article/details/gocwbmtkk.sHtML

document.querySelector(".item")
来源：http://mobile.fehbvm.com/Article/details/gprdlsppt.sHtML

[U101] JS：classList 操作
来源：http://read.share.hesvh.cn/Article/details/gagasbcby.sHtML

el.classList.toggle("active")
来源：http://wap.hesvh.cn/Article/details/gslydgrua.sHtML

[U102] JS：本地存储
来源：http://baike.zdbjq.cn/Article/details/gqtohtjel.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.blog.fehbvm.com/Article/details/gbbxdnrbv.sHtML

[U103] JS：定时器
来源：http://3g.hesvh.cn/Article/details/ggppyxrnn.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.share.fehbvm.com/Article/details/gtwwabvkb.sHtML

[U104] JS：防抖
来源：http://blog.fehbvm.com/Article/details/gjpfobeku.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.hesvh.cn/Article/details/gqbunadqe.sHtML

[U105] JS：节流
来源：http://baike.fehbvm.com/Article/details/grcsrvaau.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://read.share.fehbvm.com/Article/details/gvayhwgax.sHtML

[U106] JS：日期格式化
来源：http://www.blog.hesvh.cn/Article/details/gaojxbbyk.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://baike.zdbjq.cn/Article/details/gulgpzkdr.sHtML

[U107] JS：数字千分位
来源：http://www.blog.fehbvm.com/Article/details/gmnyyhknd.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.hesvh.cn/Article/details/gumbzpams.sHtML

[U108] JS：随机整数
来源：http://3g.fehbvm.com/Article/details/gwzanpnvr.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.fehbvm.com/Article/details/gyklbsgcg.sHtML

[U109] JS：数组分组
来源：http://read.share.fehbvm.com/Article/details/glntixtpj.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.hesvh.cn/Article/details/ggukersia.sHtML

[U110] JS：数组分块
来源：http://3g.zdbjq.cn/Article/details/glrsukpef.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.share.fehbvm.com/Article/details/gswznavmh.sHtML

[U111] JS：对象转 Map
来源：http://blog.zdbjq.cn/Article/details/gwfnxczhg.sHtML

new Map(Object.entries(obj))
来源：http://mobile.zdbjq.cn/Article/details/gqidbqxom.sHtML

[U112] JS：字符串补位
来源：http://wap.zdbjq.cn/Article/details/gxpoaclay.sHtML

"7".padStart(3, "0")
来源：http://mobile.zdbjq.cn/Article/details/golhkoqyp.sHtML

[U113] JS：正则替换全部
来源：http://mobile.zdbjq.cn/Article/details/gcfpjcghh.sHtML

s.replaceAll("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gjrlrpiyu.sHtML

[U114] JS：JSON 深比较
来源：http://m.share.hesvh.cn/Article/details/gwjxhbvkj.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.fehbvm.com/Article/details/gtmrnruec.sHtML

[U115] JS：生成 UUID
来源：http://blog.zdbjq.cn/Article/details/gkepajria.sHtML

crypto.randomUUID()
来源：http://blog.zdbjq.cn/Article/details/glzrkfdws.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://m.share.zdbjq.cn/Article/details/gsmsyssyw.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.fehbvm.com/Article/details/gnlyaxkun.sHtML

[U117] JS：单元测试
来源：http://3g.fehbvm.com/Article/details/grwjtdwjc.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.fehbvm.com/Article/details/gerwsftao.sHtML

[U118] JS：开发服务器
来源：http://www.share.hesvh.cn/Article/details/gbdqgruhv.sHtML

npm i -D vite;  npx vite
来源：http://mobile.zdbjq.cn/Article/details/gkthiqvss.sHtML

[U119] JS：生产构建
来源：http://www.share.zdbjq.cn/Article/details/gfpzzykkw.sHtML

npx vite build
来源：http://mobile.hesvh.cn/Article/details/gmulbnldc.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.fehbvm.com/Article/details/gvneiiwhh.sHtML

import.meta.env.VITE_API_URL
来源：http://www.share.fehbvm.com/Article/details/gpvfqnxwl.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/ghsysknjg.sHtML

统计汇总
来源：http://m.share.zdbjq.cn/Article/details/gbbenybjr.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gpxdtqftu.sHtML

按语言统计（条）：
来源：http://www.blog.hesvh.cn/Article/details/ggctrpwkr.sHtML

Python ......... 252
来源：http://www.m.share.zdbjq.cn/Article/details/gtxtrfcbz.sHtML

PHP ............ 252
来源：http://baike.zdbjq.cn/Article/details/gavhoczcp.sHtML

JavaScript ..... 252
来源：http://www.blog.hesvh.cn/Article/details/gpqarqahz.sHtML

TypeScript ..... 212
来源：http://blog.zdbjq.cn/Article/details/gxnfqsjtm.sHtML

Java ........... 212
来源：http://read.share.fehbvm.com/Article/details/gvhlgywhc.sHtML

Go ............. 212
来源：http://www.share.fehbvm.com/Article/details/gznkuymcx.sHtML

Ruby ........... 212
来源：http://m.share.zdbjq.cn/Article/details/gedvlfizb.sHtML

C# ............. 212
来源：http://3g.fehbvm.com/Article/details/gernlozma.sHtML

C .............. 30
来源：http://www.share.zdbjq.cn/Article/details/geqemeaoq.sHtML

C++ ............ 30
来源：http://baike.fehbvm.com/Article/details/grtpxmxmh.sHtML

SQL ............ 90
来源：http://www.m.share.zdbjq.cn/Article/details/gzaxawuwq.sHtML

Bash ........... 80
来源：http://www.share.hesvh.cn/Article/details/gsqzqwrda.sHtML

Kotlin ......... 15
来源：http://www.share.fehbvm.com/Article/details/gnrdbqywt.sHtML

Swift .......... 15
来源：http://wap.fehbvm.com/Article/details/guchpxgjg.sHtML

Lua ............ 10
来源：http://www.share.hesvh.cn/Article/details/gctmgppnp.sHtML

Perl ........... 10
来源：http://baike.fehbvm.com/Article/details/gyjaulgnr.sHtML

Scala .......... 10
来源：http://baike.hesvh.cn/Article/details/gcxjpvetl.sHtML

------------------------------------
来源：http://m.share.fehbvm.com/Article/details/ghzwxhgfd.sHtML

合计 ........... 2106 条
来源：http://www.blog.fehbvm.com/Article/details/gwckiopwc.sHtML

按章节统计：
来源：http://3g.hesvh.cn/Article/details/gdkgbcpfh.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.share.zdbjq.cn/Article/details/gzcqelols.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://baike.zdbjq.cn/Article/details/gyqblgqjg.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://3g.fehbvm.com/Article/details/gksvjidns.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.m.share.zdbjq.cn/Article/details/glgaxvoyt.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.share.zdbjq.cn/Article/details/goxwpjwhs.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://3g.zdbjq.cn/Article/details/grimhofnw.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://read.share.zdbjq.cn/Article/details/givyxebsu.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wap.hesvh.cn/Article/details/gcllqygfl.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://baike.hesvh.cn/Article/details/gnzqwtmwm.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.m.share.fehbvm.com/Article/details/gmffvadbc.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mobile.fehbvm.com/Article/details/gmdymooxa.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://m.share.fehbvm.com/Article/details/gmsrogxkr.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wap.zdbjq.cn/Article/details/gcqkfjpsr.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wap.zdbjq.cn/Article/details/gximhgulr.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://blog.hesvh.cn/Article/details/gomqumksh.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wap.zdbjq.cn/Article/details/glotzmwoi.sHtML

Q SQL 专题                              90
来源：http://read.share.hesvh.cn/Article/details/gsjkkncdz.sHtML

R Bash 专题                             80
来源：http://www.blog.zdbjq.cn/Article/details/ggcfmwybs.sHtML

S C / C++ 专题                          60
来源：http://www.m.share.fehbvm.com/Article/details/gumnsaoeq.sHtML

T 其他语言补充                          60
来源：http://www.share.hesvh.cn/Article/details/gmvdjpxae.sHtML

U 高频实用片段                         120
来源：http://blog.zdbjq.cn/Article/details/gilbpvaxv.sHtML

------------------------------------
来源：http://mobile.fehbvm.com/Article/details/ghmwdtnra.sHtML

合计                                  2106 条
来源：http://mobile.fehbvm.com/Article/details/gnhxjpomt.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.zdbjq.cn/Article/details/gtzbhkbsv.sHtML

使用提醒
来源：http://m.share.zdbjq.cn/Article/details/gkolakpgf.sHtML

--------------------------------------------------------------------------------
来源：http://3g.hesvh.cn/Article/details/gokzotjyg.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.blog.zdbjq.cn/Article/details/gtmrcxkuz.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://m.share.zdbjq.cn/Article/details/gstufbeyn.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.blog.fehbvm.com/Article/details/gkidolbor.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.share.hesvh.cn/Article/details/goifyovxn.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wap.hesvh.cn/Article/details/grhkgndqt.sHtML

—— 文件结束 ——
来源：http://www.share.hesvh.cn/Article/details/gononbukn.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gajtogbdf.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://mobile.zdbjq.cn/Article/details/gtzkozpit.sHtML

Common Programming Examples Cheat Book
来源：http://read.share.hesvh.cn/Article/details/gzzwxsgmx.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/grqmuobfy.sHtML

【收录内容】
来源：http://read.share.hesvh.cn/Article/details/goiazflix.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://read.share.fehbvm.com/Article/details/gtnyxnlxo.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.share.fehbvm.com/Article/details/gisncgava.sHtML

SQL · Bash · C · C++
来源：http://3g.zdbjq.cn/Article/details/gjfjsexbi.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.blog.zdbjq.cn/Article/details/ganxftvhv.sHtML

【使用说明】
来源：http://baike.fehbvm.com/Article/details/gbihoboxd.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.share.fehbvm.com/Article/details/gbfknpkad.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://3g.zdbjq.cn/Article/details/gaoixjalk.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://blog.hesvh.cn/Article/details/gnrzztlpg.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.m.share.zdbjq.cn/Article/details/grlqmwjry.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://mobile.zdbjq.cn/Article/details/gavzuqrjn.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wap.hesvh.cn/Article/details/gxlaqvzcz.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://mobile.fehbvm.com/Article/details/gskbpqkfs.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://blog.hesvh.cn/Article/details/gresxcmuq.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://3g.fehbvm.com/Article/details/gbwsmrqjv.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://read.share.zdbjq.cn/Article/details/gydjbilmc.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.m.share.hesvh.cn/Article/details/gwzbhskwi.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://read.share.fehbvm.com/Article/details/gzauhawki.sHtML

【文件统计】
来源：http://m.share.zdbjq.cn/Article/details/gjofjfjgb.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://mobile.hesvh.cn/Article/details/guzyrpyjm.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fehbvm.com/Article/details/gchndlhav.sHtML

目  录
来源：http://mobile.zdbjq.cn/Article/details/glqgglteb.sHtML

--------------------------------------------------------------------------------
来源：http://3g.zdbjq.cn/Article/details/gohbsjxmm.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://baike.hesvh.cn/Article/details/giitebhww.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://3g.zdbjq.cn/Article/details/gwyhbydgd.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://m.share.fehbvm.com/Article/details/gitrnquxx.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://baike.fehbvm.com/Article/details/glvwijtcc.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://3g.zdbjq.cn/Article/details/gpaeuzwkq.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://read.share.fehbvm.com/Article/details/goocmhtzi.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.share.hesvh.cn/Article/details/gucsbtzxj.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://read.share.zdbjq.cn/Article/details/gkjjufpmi.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://m.share.zdbjq.cn/Article/details/ghdcstuxn.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://baike.hesvh.cn/Article/details/gjksycyhu.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://m.share.hesvh.cn/Article/details/gjnieicat.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://m.share.hesvh.cn/Article/details/ghgnquwbk.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://blog.zdbjq.cn/Article/details/gfikhcyxy.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.blog.fehbvm.com/Article/details/gkoadmzyf.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.blog.zdbjq.cn/Article/details/gxbsjmgkq.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://m.share.zdbjq.cn/Article/details/gwpwcrtgl.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://baike.hesvh.cn/Article/details/gxzbgpgnr.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://m.share.zdbjq.cn/Article/details/gaycolpfr.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://read.share.fehbvm.com/Article/details/gpbkyruxx.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.fehbvm.com/Article/details/gfplezypu.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://read.share.fehbvm.com/Article/details/gbtiperxp.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/ghdtxjlok.sHtML

A. 基础语法与类型
来源：http://blog.zdbjq.cn/Article/details/ggckkhulr.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gcgacbdvy.sHtML

[A01] Hello World
来源：http://mobile.hesvh.cn/Article/details/govwyeuip.sHtML

Py:   print("Hello, World!")
来源：http://www.m.share.zdbjq.cn/Article/details/gvvipcral.sHtML

PHP:  echo "Hello, World!";
来源：http://baike.hesvh.cn/Article/details/ggoxtqqoh.sHtML

JS:   console.log("Hello, World!");
来源：http://www.m.share.zdbjq.cn/Article/details/gorziuqig.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://m.share.zdbjq.cn/Article/details/gthfmoatd.sHtML

Java: System.out.println("Hello, World!");
来源：http://wap.fehbvm.com/Article/details/gsrfmkppu.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://read.share.hesvh.cn/Article/details/gbjffpnnn.sHtML

Ruby: puts "Hello, World!"
来源：http://m.share.fehbvm.com/Article/details/gecrqxevk.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.share.fehbvm.com/Article/details/gyafzghqw.sHtML

[A02] 变量声明与赋值
来源：http://read.share.fehbvm.com/Article/details/gjrjafvwt.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://m.share.hesvh.cn/Article/details/glwdwyfmw.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://baike.hesvh.cn/Article/details/gtyodqmkc.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://blog.hesvh.cn/Article/details/gvnoixbov.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.blog.fehbvm.com/Article/details/gkxflhztk.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.share.zdbjq.cn/Article/details/grfjaewkz.sHtML

Go:   name := "Alex"; age := 20
来源：http://blog.hesvh.cn/Article/details/gpartxdrs.sHtML

Ruby: name = "Alex"; age = 20
来源：http://mobile.hesvh.cn/Article/details/gkejjjrfy.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://blog.zdbjq.cn/Article/details/gmwdupnni.sHtML

[A03] 常量定义
来源：http://www.blog.fehbvm.com/Article/details/grluykfjh.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.blog.hesvh.cn/Article/details/gqpmeeoiw.sHtML

PHP:  const PI = 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/gugljakle.sHtML

JS:   const PI = 3.14159;
来源：http://3g.fehbvm.com/Article/details/gkjqrqcyk.sHtML

TS:   const PI: number = 3.14159;
来源：http://3g.hesvh.cn/Article/details/gaaadzqmc.sHtML

Java: static final double PI = 3.14159;
来源：http://wap.fehbvm.com/Article/details/gzxpssvwm.sHtML

Go:   const PI = 3.14159
来源：http://www.blog.fehbvm.com/Article/details/goxntkhlp.sHtML

Ruby: PI = 3.14159
来源：http://wap.zdbjq.cn/Article/details/ggggtmwza.sHtML

C#:   const double PI = 3.14159;
来源：http://read.share.fehbvm.com/Article/details/gakohwiqu.sHtML

[A04] 判断变量类型
来源：http://www.blog.hesvh.cn/Article/details/gqqtsrtgk.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://mobile.hesvh.cn/Article/details/gjsboeljl.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.share.fehbvm.com/Article/details/gmjbqgslr.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.blog.hesvh.cn/Article/details/gktwgvrbd.sHtML

TS:   typeof x; x instanceof Date
来源：http://read.share.hesvh.cn/Article/details/gxiswaddx.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://m.share.hesvh.cn/Article/details/guftuntlx.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://m.share.hesvh.cn/Article/details/grdbzjeqk.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://read.share.fehbvm.com/Article/details/gatqxbanm.sHtML

C#:   x.GetType().Name; x is int
来源：http://wap.fehbvm.com/Article/details/gamwsmaml.sHtML

[A05] 整数除法与取模
来源：http://www.blog.fehbvm.com/Article/details/gsydpdrsm.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.blog.zdbjq.cn/Article/details/gvqeldhjc.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.m.share.fehbvm.com/Article/details/gvguvlrxn.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.hesvh.cn/Article/details/gjephfbgj.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://m.share.hesvh.cn/Article/details/gdfsofosf.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.blog.fehbvm.com/Article/details/grfbcnozi.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.share.fehbvm.com/Article/details/gqrknyhxi.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.blog.fehbvm.com/Article/details/gydlpwrbd.sHtML

C#:   7 / 2; 7 % 2
来源：http://read.share.fehbvm.com/Article/details/gqgdhvomw.sHtML

[A06] 字符串转数字
来源：http://wap.hesvh.cn/Article/details/gmwyccnra.sHtML

Py:   int("42"); float("3.14")
来源：http://www.share.zdbjq.cn/Article/details/gvqjizbtm.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.blog.fehbvm.com/Article/details/gogbmwcqo.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://m.share.hesvh.cn/Article/details/gpnvdsibp.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.m.share.zdbjq.cn/Article/details/gpbvthnlw.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://mobile.zdbjq.cn/Article/details/gqxixscox.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://read.share.hesvh.cn/Article/details/gejuypaea.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.m.share.zdbjq.cn/Article/details/grhyjbbww.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://wap.zdbjq.cn/Article/details/gqsiudyug.sHtML

[A07] 数字转字符串
来源：http://wap.fehbvm.com/Article/details/gdojbnsgg.sHtML

Py:   str(42)
来源：http://www.m.share.zdbjq.cn/Article/details/goeiufeky.sHtML

PHP:  (string) 42; strval(42)
来源：http://read.share.hesvh.cn/Article/details/gxjnlwhiy.sHtML

JS:   String(42); (42).toString()
来源：http://baike.hesvh.cn/Article/details/gtxoxegfc.sHtML

TS:   String(42)
来源：http://mobile.hesvh.cn/Article/details/gxsibolev.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://mobile.fehbvm.com/Article/details/gyzfiawam.sHtML

Go:   strconv.Itoa(42)
来源：http://3g.zdbjq.cn/Article/details/gadppejdw.sHtML

Ruby: 42.to_s
来源：http://www.m.share.hesvh.cn/Article/details/giyvdbpka.sHtML

C#:   42.ToString()
来源：http://m.share.hesvh.cn/Article/details/gtzacluzn.sHtML

[A08] 取整与四舍五入
来源：http://www.share.hesvh.cn/Article/details/gwytmzrha.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://m.share.zdbjq.cn/Article/details/gckobmktz.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://read.share.hesvh.cn/Article/details/gvdzugunb.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.share.fehbvm.com/Article/details/gdtdsthti.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://read.share.fehbvm.com/Article/details/ggowuirjn.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://wap.hesvh.cn/Article/details/gwinmtirl.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://blog.hesvh.cn/Article/details/geenyiiev.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://3g.zdbjq.cn/Article/details/gbqofnrla.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.m.share.hesvh.cn/Article/details/gkgnddens.sHtML

[A09] 绝对值与最大最小值
来源：http://wap.fehbvm.com/Article/details/gzxzyosxc.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://baike.fehbvm.com/Article/details/gobrossua.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://3g.fehbvm.com/Article/details/gzjrgoehw.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.share.zdbjq.cn/Article/details/golaefzvm.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://3g.fehbvm.com/Article/details/gseyndnxa.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.m.share.hesvh.cn/Article/details/gncrnvfsr.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.share.fehbvm.com/Article/details/geoknttfz.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://read.share.zdbjq.cn/Article/details/gkxnncrrm.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.blog.hesvh.cn/Article/details/gcolqeipb.sHtML

[A10] 生成随机数
来源：http://m.share.zdbjq.cn/Article/details/gybxzqsgu.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.share.fehbvm.com/Article/details/grgrmuhrl.sHtML

PHP:  random_int(1, 100);
来源：http://blog.zdbjq.cn/Article/details/gqtowywfv.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.share.hesvh.cn/Article/details/gfvsdcuqk.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://3g.fehbvm.com/Article/details/gmkrktidg.sHtML

Java: new Random().nextInt(100) + 1
来源：http://3g.zdbjq.cn/Article/details/gxfqeyapz.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://mobile.fehbvm.com/Article/details/gqsjkpdyy.sHtML

Ruby: rand(1..100)
来源：http://read.share.zdbjq.cn/Article/details/gaaasewbe.sHtML


<!-- 参考信息 -->