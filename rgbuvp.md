代发 wailian999

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3dkyjuzdo.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3htmjieyy.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3ycprusue.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3ursyfszl.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3lasnfwqo.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3egwpqcig.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3loprpugk.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3ptpaozsm.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3wuavjago.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3qoqskrwf.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3sjilwzws.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3ugqktpwx.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3gmdaqwik.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3hvhzzgru.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3pdqsztdc.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3uekmdyjv.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3ajfwaajn.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3rqbrrfje.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3qitihnfh.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3oqoshfhw.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3wcefqebf.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3wskbsmzx.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3ozabunut.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3bckmjmjg.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3qyqfaoge.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3wqdoijhu.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3peiavoip.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3zqsgmtwy.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3shshfgnp.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3urlikdlv.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3jowfugif.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3lqbpldum.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3xyvfsdfv.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3jddzygwn.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3yaquxzrf.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3ugpzbilc.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3vbqqndau.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3bbwffirk.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3tcphxfce.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3kfsbyhir.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3hsdojnqu.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3recygzbj.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3ydruoumt.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3vsjwnjen.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3vfklmzmm.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3dfcpqiez.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3cllirlhr.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3mjugagbv.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3crthremm.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3fbqkzntm.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3qzfndurt.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3vpjsbxxy.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3yjtbqaur.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3qqaibvvm.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3hfczpghn.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3qeypguvn.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3xnqdchba.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3hicopbvo.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3wbvevbxc.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3gyuxvore.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3lvrtiqud.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3eqkresjr.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3luuiyhxp.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3cflpcuyy.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3pbwvkgbz.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3afxmlzip.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3wnbvinht.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3qielsbiw.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3cmwtngsp.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3uckgkpua.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3hbrhefhq.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3mnjferuf.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3obezeqzh.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3ejteonkp.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3pebdvsyp.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3ynnsprkm.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3gojwspmu.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3pvlwrome.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3ryxquvwi.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3imatynwi.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3fwcwejwn.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3iumyyuhu.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3iwdspxwv.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3pciucauc.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3ifpaznoe.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3fsxnbjqk.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3vbjepxim.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3fzvbqntp.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3jncgczkc.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3oabcpmgs.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3rqmmbsxy.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3nijorxxs.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3yxjyamhw.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3zkicyusy.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3edwccgwz.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3krspvpwx.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3qihinltw.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3flmrjccj.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3szsdjgev.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3iggeocoh.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3xsdhgvdl.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3vvxsjawo.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3mfdzbxjl.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3zlecsttv.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3qptfpuvj.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3bmukbayq.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3btfxorue.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3ybsxtuou.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hpfywyzb.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3adyrizge.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bkwidnpi.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3xfwnjfsb.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3cxknyjgr.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3mieffext.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3qjbjpsjf.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3mrwqndrx.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3fdztqywf.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3kuffkjcg.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3opyovoro.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3wuytoywo.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3hohdrmqh.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3rlazvjoq.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3sfafxzzj.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3pkdhlhtw.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3pmszsuxa.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3dfaheczu.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3uzljtgmx.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3olojmwkc.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3buwebiul.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3owuohydb.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3aipkdmvo.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3uvuxdqho.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3tafpjjsw.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3uwiazutb.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3ylurazpq.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3mlqwfqjf.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3yvdxsmed.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3dmfbuznf.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3htbqtxvm.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3ebtxrbpl.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3tsvyrjeh.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3sptqicht.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3kmoyyviq.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3msbbgzwi.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3vhdlzzew.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3kiihrosf.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3lvbbqwww.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3pzjhwtxt.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3niouhwkl.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3ckwtthzj.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3ianearjm.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3mqwaqjtk.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3qecapbzu.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3ygqflfsz.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3avbztarg.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3sbxowmze.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3emvglnwx.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3cxvvsmki.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3uovbbaqx.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3tlzcwcai.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3jrofoeqc.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3eyswfubv.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3lblhaqdu.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3ekbabigv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cqdwnvlb.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3smiurvsy.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3wugsyoit.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uammqiis.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3sjywdief.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3ikuvbxws.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3gflvoybe.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3ygjeappp.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3yaifflbx.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3mghpeafe.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3btlrtpcr.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3rspldvid.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3nrblwafw.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3voomtnbf.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3sdojwkig.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3dmclnwwe.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3hrnlmpac.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3mdegoyan.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3oytvolav.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3mrqjxggn.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3dauztssw.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3ltwoupit.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3gpqdhpvj.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3kpcxkebt.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3vyrxgaos.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3cexjjxte.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3nelastgf.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ojekqypd.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3dkllcmmk.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3wvgxdwja.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3twtgfknh.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3xmyzmnet.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3gdivhcvz.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3fcferwwb.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3mcjahgws.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3ildqmhjz.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3dpjszaxk.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3jemcuhno.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3onketnst.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3bzpbaiyv.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3uosjxcbo.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3pnupzpdx.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3zzenynqv.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3nzsepxwt.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3vuglvvjd.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3edpebdhv.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3lfrbuwpe.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3ruwtjjpm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3frnprcrw.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3sazqtbyp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3whljiudf.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3wwuudgol.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3cqiafqib.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3luqdyjns.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3fzupkkte.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3xcsvgbqr.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3jsotdojk.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3xsvnoqgh.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3utqalodi.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3idhzqxpo.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3bskjvftv.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3tzsmqure.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3qwfvppxa.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3gstdbkqi.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3llzbzagb.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3xwdmbmmx.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3brhxiwup.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3mxurjyox.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3bywvyytm.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3yezvvjjy.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3fjnnwvum.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3vbepchjj.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3wuaadgpo.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3ujesrdxn.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3rlobesqo.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3vltxgbgu.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3tedssuca.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3mboznqov.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3mpouaquz.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3dkgzupbz.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3vkwyaiiz.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3ecqxubeq.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3jahogwxs.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3yknntpil.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3cyfopukq.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3vlpnxpod.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3ijhwwpuy.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3xugfvhow.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3luyzcjqo.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3nguugiba.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3fcjtgiyf.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3hyufhkln.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3eoagdbti.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3upvugllb.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3ydemzspp.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3zcldkuzo.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3kcfeabey.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3nkygsygd.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3yrawyfcq.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3gfxuxnvz.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3jevutkrf.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3mvuepife.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3jlkschgu.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3xjejrzry.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3mxpdagyl.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ziyiepza.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3uxmhezdy.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3xfbaqtzw.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3ddsytczx.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3yszdptfl.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3quucszai.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3uscgfghu.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3zpmtdoqy.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3hlwpscyb.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3zsesdvnl.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3zewpdrlh.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3gbixegbe.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3sdwcoljy.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3hbpwocnj.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3pkprffxr.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3eauslwow.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3exkoiwuv.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3zaorvuab.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3klcobrbh.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qxeckrbp.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ofewvpol.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3cocackjn.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3bzapuicn.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3gnlzjovh.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3qryautgf.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt3yuizhsho.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3onzmpncq.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3ecbfhpyw.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3xngetojc.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3zkpafzgv.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3tcenwxme.html


<!-- 参考信息 -->