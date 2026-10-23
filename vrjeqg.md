代发 wailian999

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3mvpiiivh.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3xfwwuuar.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3nilxbeip.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3zzrvznkx.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3rdvkdhwl.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3gztxscbg.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3zmjtvzlh.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3wsglcqst.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3xhvbktqm.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3mippqvwg.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3umnhamvk.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3seiriofw.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3mtfuirlv.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3agvjtzcm.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3ppgujswq.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3ekjydlcj.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3rpoylzmk.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3jxkqmhie.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3uuslhuks.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3sxrtlwgy.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3emimpapa.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3cbimlorr.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3scufzxof.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3myacvjxu.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3vpsdeyid.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3mwljrjzw.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3ijpfkcog.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3sujypdnx.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3xspaaqoh.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3tkjkmsfw.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3rqxkvmqs.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3rpzlfsnk.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3sifsdkdx.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3ieyzyxih.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3dmewwnfz.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3jxfjlrvq.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3auhzphjl.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3geowhjlf.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3alwhtlxr.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3qrgkdzba.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3rhkttaoz.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3ytymtbrw.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3lbzgohxv.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3klmyaihr.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3fxathnty.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3dlcskqon.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3ffgkhjlp.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3ngdjqnep.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3penkrvbu.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3ndnoaspq.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3lcwphgop.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3bkdsfwes.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3xpgikcqz.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3skuwhmwf.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3qylymrol.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3demnpojj.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3idsraynn.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3olbexnjb.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3wutzlvuf.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3jedalfdq.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3mbqhktct.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3aibpuzfe.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3eauldwyz.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3tkmaqmnx.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3eabxqojc.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3sepcvylp.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3hlmozafc.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3pqzyfzhd.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3azfzelbc.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3bpwdxecl.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3mcmguxwr.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3tariddzy.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3ztvelsyp.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3itlwhhas.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3kqejoxfv.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3zrlzbvbh.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3drfbucag.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3inbrptjd.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3bfgrecok.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3jghnnjba.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3ddnyctnw.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3jpyzsoii.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3radljkbi.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3xhioztxe.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3fbleyfoe.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3nqdkxmzl.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3roehcwyh.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3bufawmbw.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3iggggeqd.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3qibvufwa.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3oqsliqle.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3jsfrbfmj.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3aeuhiggy.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3dvurxniw.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3afkrvidl.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3wzlkqfeh.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3cskhdiol.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3cazbcgdg.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3fkkyaygz.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3qenhsefu.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3lfyrnahq.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3guvwqfln.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3qpisklym.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3htefzufv.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3dexqyzge.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3pohbaodx.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3yjdylqen.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3wllrglvr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zdokxiuv.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3plmddhnn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jrpprkqc.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3blxkdfbp.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3cazjvzel.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3sbsxmyfd.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3szwxxssi.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3dtyrcmai.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3tgxbxpgs.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3qpiltpvc.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3ouluqnzh.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3jcgkbsnb.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3qseumsmr.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3salobuxh.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3dtffvvgk.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3nbyjocux.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3lucqogbh.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3dkqxmebt.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3irifbeeq.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3wpzmmbhc.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3mhomvkcy.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3narshhzr.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3akilunvy.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3uzzsohpe.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3gabmeblq.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3gjlaatgt.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3yxhjnzsz.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3gqbwsxlm.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3zuebutmw.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3zmpeezmd.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3gtxznglx.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3bhdnqlhr.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3mizikfcg.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3bnlnwmcx.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3wcsghmfv.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3blekkgmu.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3pxdzzthz.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3tjsodjys.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3zasitjwa.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3bpftbihe.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3vgeomhvk.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3vpcqfetf.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3oaiignnq.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3naafhnng.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3panyyklb.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3boxzvris.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3wsdarfzo.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3qjvktdtp.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3xpidykmr.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3cbfchuop.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3wcqmlrai.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3mfopayjy.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3itxpraqe.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3iodgnzbh.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3ijlvspxi.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3imdnxyhn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tvsgkudw.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3xszehtsf.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3ejiwtpoa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zoyucyfk.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3tkvfdkol.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3lmjxerip.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3jiabkojs.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3ijiurvcm.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3pxqvcmzx.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3qcwbauhj.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3geyewoya.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3hwjthgvu.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3akwswssj.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3fxtmcwog.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3kkkkmuli.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3ufimgxxw.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3rzvcpjjz.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3ajszxuij.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3jpwzjllx.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3rnerfqyt.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3hlsfnikg.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3arnoozze.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3lhbsajsk.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3picnokie.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3tbihgrmj.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3kfdzflcy.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3axtjidwq.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3xtxikedi.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3gucohwjn.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3akelaezj.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3jwzeyodl.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3tnftgscz.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3izujztpd.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3kcbkaqpj.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3nrocpwbn.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3aidkwgpt.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3tujtmugi.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3uvlctejh.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3oznfflkm.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3weejrqge.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3zgfndsju.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ljfsvblc.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3rbfujhmq.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3vwnfluie.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3tkotcmba.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3olbtnjtz.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3jeskxeoh.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3akmhzcyu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3epjxutwb.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3qovrkcri.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fbcixcvg.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3mvrnzdiq.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3hmvjqowz.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3tyuwmykt.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3qagzmcgt.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3pxbkqips.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3rrkpalfb.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3duvrjczi.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3acxnipal.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3cyrjrpog.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3qdcgdtif.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3ptnlvdvb.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3nnsmamjp.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3ntclxxny.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3pwaxemkp.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3vwxmfuvp.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3zdbcfcpv.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3lygstygl.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3drfjwebx.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3jljicghc.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3iuqexihg.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ijtdjrka.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3hqujqlsm.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3tacgbyto.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3dpuirgfw.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3ppxjmdqg.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3piodxfzx.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3raiaveay.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3hzbpgzgf.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3lulbrxic.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3dukmvrov.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3lcagyaan.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3msinbeta.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3mkzcpfed.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3hkcfriig.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3glkeeyjx.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3jmempiwc.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3pbgzufwv.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3wrcrmdng.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3znfuomsj.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3kqwwzfmx.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3bdvovcip.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3aymafhtw.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3wevckfhy.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3ntozoqlp.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3snbdyvgi.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3qsmfehex.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3fopfeaay.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3lzglnris.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3inszuexo.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3bsdzdssy.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3fdteatyz.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3fpzucrsq.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3lhrvjwph.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3nbxjfndz.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3nzhkzyss.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3hmocxpnb.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3tjbkbjmo.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3chqsvlbk.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3smbsmaaz.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3cnkhelxy.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3npbxawgh.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3rgneggzm.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3ttqhyili.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3kujfnldk.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3wpupucbd.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt3szuvaust.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3zypmphso.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3zanojukg.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3ihqrzkpm.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3xzrfchji.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3wacuvtss.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3jwbunhth.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3gscjterf.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3fgtrcojk.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3wtnuoxji.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3hlbkgfpf.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3vxgpmvtc.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3zvbrlmcb.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3hnfukkbs.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt3eohqkjpq.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3putgpdlt.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3htacgtcc.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3ifqnynoq.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3ybpavwpu.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3vbdxnhrc.html


<!-- 参考信息 -->