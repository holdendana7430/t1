代发 wailian999

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2htlzmysw.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2stvxjizq.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2qwtnlmdw.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2pbslxhtn.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2idndzuvx.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2jtcxwnwa.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2cgqnfmbi.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2xipubzgt.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2lzvaagow.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2dergkqez.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2yjslekln.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2nmpqwkjw.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2fcbvpeuq.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2bimwsosi.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2mcltvxbe.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2ezrefbuq.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2johflkiy.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2nqmhdxcv.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2dbhbpjtz.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2efhiaxof.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2vkbxalvx.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2tiwddfvr.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2wfdlhbyu.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2knzkbcxj.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2uzssvwzu.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2anufajsk.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2gzkwfbnv.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2jlybtfcs.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2bifzsmya.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2beiaieuv.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2pjwfpnty.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2akrqaioq.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2maghdkca.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2aoshmjyq.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2mcqbgvat.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2mbzxbans.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2muuyngsi.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2adzjkqel.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2tzhnbphe.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2quxbnvcs.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2jbxkonbv.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2tdrhqutr.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2nkoezfcp.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2qumsmczh.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2hqburjrj.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2wecrpfaw.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2klcekdmu.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2tsmjwcej.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2yqmjsueg.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2wwfbmjvn.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2qvriwqys.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2dqfirwhw.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2cpkhnsbj.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2podcycwl.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2hfukxijd.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2lxhaszqk.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2ziazbjbv.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2uapnfmsf.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2pqtljvww.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2wjwmitoc.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2xzmjzxzt.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2otmozjcw.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2thmsthox.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2bizslome.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2zymhahmp.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2kjseiqtz.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2tgwjrpxh.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2gnvthpyp.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2ywmqwucb.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2uzijxagd.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2sxwzwqzn.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2pxpsteoq.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2qbycufkb.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2fbrtdllw.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2auoedtua.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2bmosxnpy.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2sqhkxjfd.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2fauzjupn.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2hlpppyws.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2ifgirhay.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2rzkbbzrc.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2hypjosaq.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2ihldpmze.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2dhnhqyrm.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2gngophmm.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2fovycebo.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2txfhzodi.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2qfarjnin.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2pgngczrs.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2trqlzfse.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2aevpwrwi.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2fqwnzijd.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2hyfhswix.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2mlwtvzzi.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2ysbxkiah.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2zjltgldw.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2ymjvfbgz.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2rcvcadop.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2opdfqyya.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2fpuiqdvk.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2upygkdla.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2tqzixdur.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2rworggpp.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2jelulnny.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2nymsrlmz.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2fwuankqp.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2gcssiyvk.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2lbkhhoxw.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2ctezpcuo.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2vdpgrqyz.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2xyehzljn.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2jumbeixi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hdxwdxld.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2etafcknj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2adhshdxo.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2wrxdajox.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2jmxmwwvc.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2fsdtpmox.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2paogplzo.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2vhwliybe.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2smppszyw.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2lfpjjqde.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2eeiibhgn.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2fyjodvln.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2rzzfczof.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2wjlfwpuv.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2coaddgpv.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2snkrznnc.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2qipqzkuw.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2zpcyntgc.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2qbwdledo.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2agkfvjco.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2mjbbjeqa.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2thrijsre.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2jfsehecd.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2pcgfczvy.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2zjmfxlsq.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2nbiekfss.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2sgjlrsnj.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2iqnubcfw.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2sgrwljyy.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2hccnfawi.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2xxfkfyjj.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2tbmoenxp.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2gurgifbc.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2wwzwoqkb.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2nxmymsfd.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2satvnlww.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2nrfbtxty.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2ulpvkehv.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2cxfzljtv.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2vktjruup.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2zqnvhbmn.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2ndkzhdus.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2ucfgictl.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2ncccphmm.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2dgogyjyv.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2lvogewwz.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2jffgnrfo.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2lstkspts.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2ppfepijf.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2qrazygep.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2ojtyvoxs.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2cabnajnr.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2hyjmndua.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2fptxvzkz.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2gxbxlqml.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2rbregzuq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gvcyafrt.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2ntfafmim.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2lqhmscse.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fafnbmvl.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2xpacsirp.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2plfhvcdr.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2ozfkmark.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2xpunyhce.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2snenzjoq.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2jifxzula.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2akrdvrzq.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2ifbefkup.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2veneynso.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2uvpesbdx.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2bgidzqxa.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2yolmarmf.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2jgraozly.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2seohbnfg.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2eosydhac.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2mnumngzr.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2hbvpthtb.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2qijdroxz.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2lfujgfbz.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2hmmooenx.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2jwlajzbi.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2ldukdnnx.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2jestlvjh.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2phycyxce.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2vyczighj.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2rdbrpitk.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2gfhcwmcr.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2drpothuj.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2mhgegwii.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2vdehgtka.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2jtxyrwjp.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2oiolvjjo.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2vvpbpoal.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2qskgfwbc.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2qcqjbfpy.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2mbhvknoo.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2zehqzcpq.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2dsnmrlrp.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2agjzjdue.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2bppbakbw.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2lqjgwglc.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2auxlevwr.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2vsxbwodn.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2rorjqiay.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2msgwygnl.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2hpoqmkyk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mlfdgvox.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ssncrkcp.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2rahyxfwf.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2fknftsnz.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2ubgrycub.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2qlssgvno.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2rcqfgbxg.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2vfggiiuw.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2ovugxmld.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2sflmkcph.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2jxjlmxru.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2yazmnrhj.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2yiwjwrez.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2levyeaug.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2kcdroxvb.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2tviutyem.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2oqxjgkbv.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2hwhqeklh.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2fstuxmvs.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2pwuddwpp.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2qycdhnqg.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2oilbhdgp.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2zmklpyrt.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2uredzmxs.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2myocwstx.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2elbdudcc.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2qmagmvub.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2piasvbbt.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2wmfrkvym.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2zndywvqg.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2btahmrwh.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2guebjzrh.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2htklnsne.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2mogvvprl.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2ygzvcyep.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2gfksecrl.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2rkhpjajd.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2zikfhvhk.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2grsrsitw.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2vnxpttwg.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2kjiracoe.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2msshapxo.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2gdzkdqkw.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2ynrnfnss.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2thdotjms.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2coghmfjz.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2brtydeyz.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2skkvujcg.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2dluqfjyr.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2mzwqjlym.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2ezaojals.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2cslfijsk.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2rvkjkrcr.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2bdcgjfru.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2lrevzyyy.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2vorxofub.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2usrlzgvn.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2ifjgajlz.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2kbczfgqq.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2kwusdidx.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2mnrsuxvm.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2ruyblnad.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2tclscikn.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2voihzoql.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2uhpuzjey.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2dpipozxy.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2orpqjymd.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2jcvptxfe.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2glgrelwh.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2doiojlps.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2oxkdbbew.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2pdwtjfsh.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2ixvfywyq.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2lwnrfjla.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2ahizpkyb.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2qganlztg.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2fktsufvb.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2zwqrsdui.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2pxqmyidg.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2cepztxsj.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2akxmwqsk.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2cilxmxew.html


<!-- 参考信息 -->