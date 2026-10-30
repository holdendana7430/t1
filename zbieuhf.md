代发 wailian999

[U69] PHP：PDO 预处理
来源：http://mobile.zdbjq.cn/Article/details/geicuambm.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://3g.zdbjq.cn/Article/details/gummnlkng.sHtML

[U70] PHP：PDO 事务
来源：http://baike.hesvh.cn/Article/details/gzbhbndhw.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.m.share.zdbjq.cn/Article/details/gtmsmbvft.sHtML

[U71] PHP：抛出异常
来源：http://www.share.zdbjq.cn/Article/details/gxfjfyzvt.sHtML

throw new RuntimeException("失败", 500);
来源：http://baike.hesvh.cn/Article/details/glwtumviu.sHtML

[U72] PHP：写错误日志
来源：http://blog.zdbjq.cn/Article/details/gqjurqmfw.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.m.share.zdbjq.cn/Article/details/gncxffapp.sHtML

[U73] PHP：读取 ini 配置
来源：http://baike.fehbvm.com/Article/details/gdtxasidw.sHtML

parse_ini_file("config.ini", true)
来源：http://m.share.hesvh.cn/Article/details/gxzxmkihv.sHtML

[U74] PHP：读取环境变量
来源：http://3g.hesvh.cn/Article/details/gddokfrpx.sHtML

getenv("APP_ENV") ?: "production"
来源：http://m.share.hesvh.cn/Article/details/giybropfz.sHtML

[U75] PHP：依赖注入
来源：http://blog.fehbvm.com/Article/details/gbecvkszx.sHtML

composer require psr/container
来源：http://www.share.zdbjq.cn/Article/details/gpcgyekcx.sHtML

[U76] PHP：简单路由
来源：http://www.blog.fehbvm.com/Article/details/gwmsvqfws.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.zdbjq.cn/Article/details/gdszdxetv.sHtML

[U77] PHP：模板渲染
来源：http://baike.fehbvm.com/Article/details/gudqvpciz.sHtML

composer require twig/twig
来源：http://baike.hesvh.cn/Article/details/gyjahdzqn.sHtML

[U78] PHP：单元测试
来源：http://m.share.zdbjq.cn/Article/details/gpxmcebfg.sHtML

composer require --dev phpunit/phpunit
来源：http://blog.zdbjq.cn/Article/details/gqkxpdsoo.sHtML

[U79] PHP：静态分析
来源：http://wap.zdbjq.cn/Article/details/gsgnrrfyo.sHtML

composer require --dev phpstan/phpstan
来源：http://blog.hesvh.cn/Article/details/gyuthpoch.sHtML

[U80] PHP：代码规范修复
来源：http://www.share.zdbjq.cn/Article/details/gjchaykpv.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://wap.zdbjq.cn/Article/details/ggfbgnsxy.sHtML

[U81] JS：初始化项目
来源：http://m.share.fehbvm.com/Article/details/ggighgevl.sHtML

npm init -y;  npm i express
来源：http://www.share.hesvh.cn/Article/details/gekpounil.sHtML

[U82] JS：package.json 脚本
来源：http://read.share.zdbjq.cn/Article/details/goblhhdzk.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mobile.fehbvm.com/Article/details/gktbdtvgz.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.share.zdbjq.cn/Article/details/gciplmqid.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://wap.zdbjq.cn/Article/details/gvawkrhzm.sHtML

[U84] JS：CommonJS 写法
来源：http://wap.fehbvm.com/Article/details/gmjbrbivp.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://blog.fehbvm.com/Article/details/gpjvdzsrz.sHtML

[U85] JS：可选链
来源：http://www.m.share.fehbvm.com/Article/details/gblpqfszt.sHtML

a?.b?.c
来源：http://read.share.fehbvm.com/Article/details/ggsviuebe.sHtML

[U86] JS：空值合并
来源：http://baike.hesvh.cn/Article/details/ghxxrhcss.sHtML

a ?? b
来源：http://mobile.fehbvm.com/Article/details/ggsnnwvdp.sHtML

[U87] JS：解构默认值
来源：http://blog.fehbvm.com/Article/details/ggnwcypif.sHtML

const { a = 1, b = 2 } = obj;
来源：http://mobile.hesvh.cn/Article/details/gfffrlxrm.sHtML

[U88] JS：对象展开合并
来源：http://www.m.share.hesvh.cn/Article/details/gqkgfhrmp.sHtML

{ ...a, ...b }
来源：http://mobile.hesvh.cn/Article/details/grmemrfoy.sHtML

[U89] JS：数组去重
来源：http://read.share.zdbjq.cn/Article/details/gnwknjnkw.sHtML

[...new Set(arr)]
来源：http://read.share.fehbvm.com/Article/details/gizydaygg.sHtML

[U90] JS：数字数组排序
来源：http://3g.fehbvm.com/Article/details/gipvhalyq.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.blog.zdbjq.cn/Article/details/gtgeaubzo.sHtML

[U91] JS：对象键值遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gexrvmrsp.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://3g.zdbjq.cn/Article/details/gbjqqrvqa.sHtML

[U92] JS：深拷贝
来源：http://mobile.hesvh.cn/Article/details/grxlroqdj.sHtML

structuredClone(obj)
来源：http://blog.zdbjq.cn/Article/details/ggixkspzd.sHtML

[U93] JS：模板字符串
来源：http://wap.zdbjq.cn/Article/details/ggsfcxdwf.sHtML

`共 ${n} 条`
来源：http://www.m.share.zdbjq.cn/Article/details/gknfcghkn.sHtML

[U94] JS：箭头函数
来源：http://www.share.fehbvm.com/Article/details/gwdpntwcb.sHtML

const double = x => x * 2;
来源：http://www.blog.fehbvm.com/Article/details/gnxogganb.sHtML

[U95] JS：Promise 包装
来源：http://3g.zdbjq.cn/Article/details/gpjrtfphp.sHtML

new Promise((resolve, reject) => {})
来源：http://www.blog.hesvh.cn/Article/details/gkbmhjrcm.sHtML

[U96] JS：async/await 与异常
来源：http://baike.hesvh.cn/Article/details/gvfhaivru.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mobile.zdbjq.cn/Article/details/gfiwkofrs.sHtML

[U97] JS：并发请求
来源：http://www.blog.zdbjq.cn/Article/details/gfyxmdarn.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.fehbvm.com/Article/details/gtjppnszs.sHtML

[U98] JS：fetch 带 JSON
来源：http://3g.fehbvm.com/Article/details/gwpdzaijz.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.share.fehbvm.com/Article/details/gfsdqyrfy.sHtML

[U99] JS：事件监听
来源：http://3g.zdbjq.cn/Article/details/gemxzbwea.sHtML

el.addEventListener("click", e => {})
来源：http://www.m.share.zdbjq.cn/Article/details/gsvdmkpyv.sHtML

[U100] JS：DOM 查询
来源：http://baike.fehbvm.com/Article/details/goxnidtsf.sHtML

document.querySelector(".item")
来源：http://read.share.fehbvm.com/Article/details/gwkqrpnqi.sHtML

[U101] JS：classList 操作
来源：http://mobile.fehbvm.com/Article/details/giydddohq.sHtML

el.classList.toggle("active")
来源：http://read.share.hesvh.cn/Article/details/gboycjsgv.sHtML

[U102] JS：本地存储
来源：http://3g.zdbjq.cn/Article/details/gaswtfysi.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://baike.fehbvm.com/Article/details/gfleimabo.sHtML

[U103] JS：定时器
来源：http://m.share.hesvh.cn/Article/details/ghnrbnpge.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.hesvh.cn/Article/details/gtporepeg.sHtML

[U104] JS：防抖
来源：http://3g.zdbjq.cn/Article/details/grwbjubuu.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.hesvh.cn/Article/details/gsbcvjczt.sHtML

[U105] JS：节流
来源：http://wap.fehbvm.com/Article/details/ggxitonmi.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mobile.zdbjq.cn/Article/details/gcbkeoiio.sHtML

[U106] JS：日期格式化
来源：http://mobile.hesvh.cn/Article/details/gdpmctpaa.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.zdbjq.cn/Article/details/gzpmstdce.sHtML

[U107] JS：数字千分位
来源：http://baike.hesvh.cn/Article/details/gxhbhqdha.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.hesvh.cn/Article/details/gytkyepeu.sHtML

[U108] JS：随机整数
来源：http://read.share.fehbvm.com/Article/details/gwgiihqxc.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.zdbjq.cn/Article/details/gopqqytlj.sHtML

[U109] JS：数组分组
来源：http://baike.fehbvm.com/Article/details/gqyrrwegq.sHtML

Object.groupBy(arr, x => x.type)
来源：http://m.share.fehbvm.com/Article/details/gawzkztud.sHtML

[U110] JS：数组分块
来源：http://www.m.share.hesvh.cn/Article/details/gffpysikm.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://blog.hesvh.cn/Article/details/ggufiqhmy.sHtML

[U111] JS：对象转 Map
来源：http://blog.fehbvm.com/Article/details/gvlzingtr.sHtML

new Map(Object.entries(obj))
来源：http://blog.fehbvm.com/Article/details/gjjbcnkhe.sHtML

[U112] JS：字符串补位
来源：http://read.share.hesvh.cn/Article/details/gstrkycfc.sHtML

"7".padStart(3, "0")
来源：http://www.blog.zdbjq.cn/Article/details/gsiethafz.sHtML

[U113] JS：正则替换全部
来源：http://www.blog.fehbvm.com/Article/details/gnpyxyoja.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gycieafys.sHtML

[U114] JS：JSON 深比较
来源：http://m.share.fehbvm.com/Article/details/girytsxya.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.hesvh.cn/Article/details/gmljhvywt.sHtML

[U115] JS：生成 UUID
来源：http://www.share.hesvh.cn/Article/details/gquuilcxt.sHtML

crypto.randomUUID()
来源：http://www.share.hesvh.cn/Article/details/gmwlycrtf.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.hesvh.cn/Article/details/gwubrycvy.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.zdbjq.cn/Article/details/glurjivjk.sHtML

[U117] JS：单元测试
来源：http://3g.hesvh.cn/Article/details/gpkecxloo.sHtML

npm i -D vitest;  npx vitest
来源：http://blog.hesvh.cn/Article/details/gmuznmpwk.sHtML

[U118] JS：开发服务器
来源：http://blog.hesvh.cn/Article/details/gmkqrurqc.sHtML

npm i -D vite;  npx vite
来源：http://baike.zdbjq.cn/Article/details/gxzdellwu.sHtML

[U119] JS：生产构建
来源：http://baike.zdbjq.cn/Article/details/gmebtohch.sHtML

npx vite build
来源：http://www.share.fehbvm.com/Article/details/grakqeocg.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://3g.fehbvm.com/Article/details/glzzktypp.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.hesvh.cn/Article/details/giwbziclf.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gfwbflloa.sHtML

统计汇总
来源：http://blog.zdbjq.cn/Article/details/gwppcghvd.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gdzcpxdsv.sHtML

按语言统计（条）：
来源：http://wap.fehbvm.com/Article/details/gfootojrc.sHtML

Python ......... 252
来源：http://www.share.zdbjq.cn/Article/details/gveobslwg.sHtML

PHP ............ 252
来源：http://baike.hesvh.cn/Article/details/gbjfxobfh.sHtML

JavaScript ..... 252
来源：http://baike.hesvh.cn/Article/details/guaakvydi.sHtML

TypeScript ..... 212
来源：http://wap.zdbjq.cn/Article/details/gyyrnzbfd.sHtML

Java ........... 212
来源：http://www.m.share.fehbvm.com/Article/details/gmcolqmrt.sHtML

Go ............. 212
来源：http://mobile.fehbvm.com/Article/details/grdmtrnzc.sHtML

Ruby ........... 212
来源：http://www.m.share.zdbjq.cn/Article/details/gcvzkspeh.sHtML

C# ............. 212
来源：http://www.share.zdbjq.cn/Article/details/gwbpvjsxj.sHtML

C .............. 30
来源：http://www.share.fehbvm.com/Article/details/gmfanjerc.sHtML

C++ ............ 30
来源：http://www.m.share.fehbvm.com/Article/details/ghhnraayt.sHtML

SQL ............ 90
来源：http://www.share.fehbvm.com/Article/details/gjfdouvsw.sHtML

Bash ........... 80
来源：http://www.share.hesvh.cn/Article/details/ghrihdukb.sHtML

Kotlin ......... 15
来源：http://www.m.share.zdbjq.cn/Article/details/gcnazokhw.sHtML

Swift .......... 15
来源：http://www.blog.hesvh.cn/Article/details/gkcxdauoa.sHtML

Lua ............ 10
来源：http://m.share.fehbvm.com/Article/details/gkjtjuhvp.sHtML

Perl ........... 10
来源：http://3g.hesvh.cn/Article/details/gnbgvtdhq.sHtML

Scala .......... 10
来源：http://www.m.share.fehbvm.com/Article/details/gqsufhjls.sHtML

------------------------------------
来源：http://blog.hesvh.cn/Article/details/gswjqwkka.sHtML

合计 ........... 2106 条
来源：http://3g.fehbvm.com/Article/details/gsxzmbrxu.sHtML

按章节统计：
来源：http://baike.zdbjq.cn/Article/details/gwcaswkfo.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://baike.fehbvm.com/Article/details/gaklvxbop.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.share.hesvh.cn/Article/details/gmjmjlsuf.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://baike.hesvh.cn/Article/details/gdmqrepgq.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://m.share.fehbvm.com/Article/details/gxecoxkrd.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.m.share.zdbjq.cn/Article/details/geyakeoyf.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wap.hesvh.cn/Article/details/gfeyjmufd.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://baike.hesvh.cn/Article/details/ghyobjwma.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.blog.fehbvm.com/Article/details/ggbzphjap.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://blog.hesvh.cn/Article/details/gawnbmglh.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.share.zdbjq.cn/Article/details/gdmwkacps.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://3g.zdbjq.cn/Article/details/ghiuhzkvx.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.share.zdbjq.cn/Article/details/gobifjdcw.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wap.hesvh.cn/Article/details/gawyzmjkg.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://baike.fehbvm.com/Article/details/gwsccpmlh.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://blog.zdbjq.cn/Article/details/gvovpzzds.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://m.share.hesvh.cn/Article/details/govrqxakf.sHtML

Q SQL 专题                              90
来源：http://3g.fehbvm.com/Article/details/gbpyoerxi.sHtML

R Bash 专题                             80
来源：http://blog.fehbvm.com/Article/details/ghbdzngvy.sHtML

S C / C++ 专题                          60
来源：http://read.share.fehbvm.com/Article/details/gksplbvvw.sHtML

T 其他语言补充                          60
来源：http://www.blog.zdbjq.cn/Article/details/ghwwizbys.sHtML

U 高频实用片段                         120
来源：http://m.share.zdbjq.cn/Article/details/guhoatcbr.sHtML

------------------------------------
来源：http://mobile.zdbjq.cn/Article/details/gyamaksng.sHtML

合计                                  2106 条
来源：http://wap.zdbjq.cn/Article/details/gqfumixvs.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fehbvm.com/Article/details/gfqrcacey.sHtML

使用提醒
来源：http://read.share.fehbvm.com/Article/details/gxsehlkup.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fehbvm.com/Article/details/gpxtfrzng.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.share.hesvh.cn/Article/details/gvixazqeb.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.share.hesvh.cn/Article/details/gpalmrpmd.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://read.share.fehbvm.com/Article/details/gokcndgdr.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://read.share.hesvh.cn/Article/details/gmgwdwdnk.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://m.share.hesvh.cn/Article/details/gbxwsblbh.sHtML

—— 文件结束 ——
来源：http://baike.hesvh.cn/Article/details/gsqcucrgd.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gqpgwujzn.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.share.fehbvm.com/Article/details/gkzfscxqy.sHtML

Common Programming Examples Cheat Book
来源：http://baike.zdbjq.cn/Article/details/goygwqjec.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gpfhommtr.sHtML

【收录内容】
来源：http://wap.fehbvm.com/Article/details/gfeslybxh.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://wap.fehbvm.com/Article/details/gjbmgckdj.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.blog.fehbvm.com/Article/details/gqfnpwtcr.sHtML

SQL · Bash · C · C++
来源：http://3g.zdbjq.cn/Article/details/gzoxijpje.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://baike.hesvh.cn/Article/details/gsyrvxgdu.sHtML

【使用说明】
来源：http://wap.fehbvm.com/Article/details/gztlrmioi.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://wap.hesvh.cn/Article/details/gztrviqdw.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.m.share.fehbvm.com/Article/details/gzczlfnve.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://mobile.fehbvm.com/Article/details/gpvtzwxjo.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://read.share.zdbjq.cn/Article/details/gitntzkkw.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://wap.zdbjq.cn/Article/details/gcoxljkxm.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://3g.zdbjq.cn/Article/details/grdotfwhv.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://3g.zdbjq.cn/Article/details/gjwbekpvq.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://read.share.hesvh.cn/Article/details/gfsxivhyd.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://blog.zdbjq.cn/Article/details/gvoqsxlfs.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://mobile.hesvh.cn/Article/details/gyuxemkiq.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://read.share.hesvh.cn/Article/details/gndkjgznb.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://wap.hesvh.cn/Article/details/gljgmbhjd.sHtML

【文件统计】
来源：http://blog.hesvh.cn/Article/details/gmvjnbbft.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://mobile.hesvh.cn/Article/details/glncdxcxe.sHtML

--------------------------------------------------------------------------------
来源：http://3g.zdbjq.cn/Article/details/gddmwcdya.sHtML

目  录
来源：http://www.blog.zdbjq.cn/Article/details/gxvufbezv.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.zdbjq.cn/Article/details/gyfdtrxdh.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.blog.fehbvm.com/Article/details/gkfbmniqk.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://read.share.fehbvm.com/Article/details/gdykjvbqk.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.share.zdbjq.cn/Article/details/gprouzvlk.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://3g.zdbjq.cn/Article/details/giqgdlqec.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://read.share.zdbjq.cn/Article/details/gpfciptjp.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://wap.fehbvm.com/Article/details/gqjwuvvtm.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://blog.zdbjq.cn/Article/details/ganvobdrc.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://baike.hesvh.cn/Article/details/gibinvgiq.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://blog.fehbvm.com/Article/details/gzhqkuwou.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://m.share.hesvh.cn/Article/details/gijtxulpi.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://mobile.zdbjq.cn/Article/details/ghhypcgzt.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://wap.hesvh.cn/Article/details/girvmucsf.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://wap.hesvh.cn/Article/details/ghqgnrngh.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://m.share.hesvh.cn/Article/details/gluuflzxv.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://wap.fehbvm.com/Article/details/gzhbtpeir.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.blog.fehbvm.com/Article/details/gprabexck.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.m.share.hesvh.cn/Article/details/gdnexwifi.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://mobile.zdbjq.cn/Article/details/gzmnbowxw.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://3g.hesvh.cn/Article/details/gqqqbxjvi.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.zdbjq.cn/Article/details/gtrwqlwvs.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://blog.zdbjq.cn/Article/details/grrembuze.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gmnutphbs.sHtML

A. 基础语法与类型
来源：http://mobile.zdbjq.cn/Article/details/ghykwyouq.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gqpaozzky.sHtML

[A01] Hello World
来源：http://wap.hesvh.cn/Article/details/gzuvvdgts.sHtML

Py:   print("Hello, World!")
来源：http://www.blog.fehbvm.com/Article/details/gjggnpjcs.sHtML

PHP:  echo "Hello, World!";
来源：http://read.share.zdbjq.cn/Article/details/grvaavyyd.sHtML

JS:   console.log("Hello, World!");
来源：http://baike.fehbvm.com/Article/details/ghbmxsguc.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://blog.zdbjq.cn/Article/details/ghniyykej.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.m.share.zdbjq.cn/Article/details/gvgridjde.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://m.share.fehbvm.com/Article/details/gabmfoubp.sHtML

Ruby: puts "Hello, World!"
来源：http://blog.hesvh.cn/Article/details/gnxlvwgpv.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.blog.zdbjq.cn/Article/details/gypmaxnig.sHtML

[A02] 变量声明与赋值
来源：http://www.m.share.zdbjq.cn/Article/details/gxpnmryxu.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://read.share.zdbjq.cn/Article/details/gcwdcatyw.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://mobile.zdbjq.cn/Article/details/gqgwcgkbw.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://baike.hesvh.cn/Article/details/gakqwkcje.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.share.fehbvm.com/Article/details/gohtziqod.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://blog.hesvh.cn/Article/details/geqttztvm.sHtML

Go:   name := "Alex"; age := 20
来源：http://baike.zdbjq.cn/Article/details/gdieqpefm.sHtML

Ruby: name = "Alex"; age = 20
来源：http://mobile.fehbvm.com/Article/details/gyoeeefrb.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.share.zdbjq.cn/Article/details/gjfaihsli.sHtML

[A03] 常量定义
来源：http://read.share.zdbjq.cn/Article/details/gkrujttqj.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.m.share.fehbvm.com/Article/details/gffxenpff.sHtML

PHP:  const PI = 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/gvcvcrofg.sHtML

JS:   const PI = 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/gvqfaowlp.sHtML

TS:   const PI: number = 3.14159;
来源：http://blog.hesvh.cn/Article/details/gzbmddzph.sHtML

Java: static final double PI = 3.14159;
来源：http://baike.zdbjq.cn/Article/details/gpkpwubju.sHtML

Go:   const PI = 3.14159
来源：http://3g.fehbvm.com/Article/details/gjorxgqow.sHtML

Ruby: PI = 3.14159
来源：http://read.share.hesvh.cn/Article/details/gqpwhjjst.sHtML

C#:   const double PI = 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/gxmgvlwvw.sHtML

[A04] 判断变量类型
来源：http://wap.hesvh.cn/Article/details/goxfvqair.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://mobile.zdbjq.cn/Article/details/ghizmhdco.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://read.share.hesvh.cn/Article/details/gswxkjrjb.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.blog.fehbvm.com/Article/details/gqqcwnvas.sHtML

TS:   typeof x; x instanceof Date
来源：http://mobile.hesvh.cn/Article/details/ggzrarule.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://m.share.zdbjq.cn/Article/details/gxsxsmdbx.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.blog.fehbvm.com/Article/details/gixlieihs.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://baike.zdbjq.cn/Article/details/gepfxlcwi.sHtML

C#:   x.GetType().Name; x is int
来源：http://m.share.hesvh.cn/Article/details/gvlmwnqxw.sHtML

[A05] 整数除法与取模
来源：http://baike.hesvh.cn/Article/details/gyskwnowr.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://m.share.zdbjq.cn/Article/details/ghquwtywz.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://wap.fehbvm.com/Article/details/gpwuwlizr.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.fehbvm.com/Article/details/gcimylkvd.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.hesvh.cn/Article/details/gdbvzjwzh.sHtML

Java: 7 / 2; 7 % 2
来源：http://read.share.hesvh.cn/Article/details/gejkmndzo.sHtML

Go:   7 / 2; 7 % 2
来源：http://wap.hesvh.cn/Article/details/gprwwgrpt.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://3g.hesvh.cn/Article/details/gtjshgxqg.sHtML

C#:   7 / 2; 7 % 2
来源：http://wap.zdbjq.cn/Article/details/gebewfhln.sHtML

[A06] 字符串转数字
来源：http://wap.fehbvm.com/Article/details/giqdubgji.sHtML

Py:   int("42"); float("3.14")
来源：http://3g.hesvh.cn/Article/details/gjikktwvw.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.blog.fehbvm.com/Article/details/gleigfrcm.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://3g.fehbvm.com/Article/details/gshyoalma.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://m.share.hesvh.cn/Article/details/gbvaheitf.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://m.share.zdbjq.cn/Article/details/gkwjadphe.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.m.share.hesvh.cn/Article/details/glornbpwc.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.blog.fehbvm.com/Article/details/grosdtpbn.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.blog.zdbjq.cn/Article/details/gzrdnaegj.sHtML

[A07] 数字转字符串
来源：http://baike.fehbvm.com/Article/details/gmogjyvjt.sHtML

Py:   str(42)
来源：http://www.share.hesvh.cn/Article/details/ggfxkiill.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.share.fehbvm.com/Article/details/gqkyrdppt.sHtML

JS:   String(42); (42).toString()
来源：http://baike.zdbjq.cn/Article/details/ghjluqpmy.sHtML

TS:   String(42)
来源：http://www.blog.hesvh.cn/Article/details/gteeewyce.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://read.share.hesvh.cn/Article/details/gftdvfdmh.sHtML

Go:   strconv.Itoa(42)
来源：http://baike.fehbvm.com/Article/details/gygzjbubf.sHtML

Ruby: 42.to_s
来源：http://www.share.hesvh.cn/Article/details/gtewgoivt.sHtML

C#:   42.ToString()
来源：http://blog.hesvh.cn/Article/details/gbsxipsuy.sHtML

[A08] 取整与四舍五入
来源：http://blog.hesvh.cn/Article/details/gieouicro.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.m.share.hesvh.cn/Article/details/gepkgyztp.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://m.share.fehbvm.com/Article/details/gtuaseqvy.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.m.share.fehbvm.com/Article/details/gghfsfywo.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://blog.fehbvm.com/Article/details/gfpcuwtnd.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://read.share.fehbvm.com/Article/details/gwvnsuhfu.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.blog.fehbvm.com/Article/details/gjcxtblek.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://m.share.zdbjq.cn/Article/details/gkjbkgpco.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://mobile.hesvh.cn/Article/details/gnxnhhgoe.sHtML

[A09] 绝对值与最大最小值
来源：http://blog.hesvh.cn/Article/details/gcxayyccl.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://baike.zdbjq.cn/Article/details/ggzkaqevd.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://3g.fehbvm.com/Article/details/gwspjefjo.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://wap.fehbvm.com/Article/details/gofhjtzpr.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.share.hesvh.cn/Article/details/gktiycchr.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://mobile.zdbjq.cn/Article/details/gkhutidyw.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://wap.hesvh.cn/Article/details/gemsftxtl.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://m.share.fehbvm.com/Article/details/glnprhjnu.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://baike.zdbjq.cn/Article/details/gnttypcoc.sHtML

[A10] 生成随机数
来源：http://read.share.zdbjq.cn/Article/details/gtwphtkfj.sHtML

Py:   import random; random.randint(1, 100)
来源：http://baike.zdbjq.cn/Article/details/guexecarw.sHtML

PHP:  random_int(1, 100);
来源：http://www.m.share.hesvh.cn/Article/details/goiqenepf.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://mobile.hesvh.cn/Article/details/gvwkmqijr.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://mobile.fehbvm.com/Article/details/gfbfusget.sHtML

Java: new Random().nextInt(100) + 1
来源：http://read.share.zdbjq.cn/Article/details/gfspgvhyb.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://mobile.zdbjq.cn/Article/details/gvricqnir.sHtML

Ruby: rand(1..100)
来源：http://mobile.hesvh.cn/Article/details/gedpqiwvp.sHtML


<!-- 参考信息 -->