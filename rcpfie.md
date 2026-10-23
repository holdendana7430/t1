代发 wailian999

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3ctdumdnj.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3xbjnipjy.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3lchwnjtn.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3ahydzktd.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3ocffwwvf.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3bdziceph.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3scgjgpev.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3jvtqnscx.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3unshqiqv.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3xhigqcrb.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3yvywhvjw.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3mkcxdvlj.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3sunppnmx.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3qsdzorhu.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3gmngqlfk.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3dgpquwiv.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3aphagcax.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3xsdlngbb.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3qeyfkvqs.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3abhleizh.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3ujhwelsl.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3nvspjrzo.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3ecqkoxls.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3dkudjcxt.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3onhdattb.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3agslgdhs.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3azgqktzj.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3sajkiqbi.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3djcyesii.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3mogvvmzw.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3beiybseb.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3moeclnmz.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3ddbotorl.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3sgtkszsl.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3jigmwyyr.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3nyztxcqj.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3lidcvacn.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3lmeyoden.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3ndcgswha.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3rgjdwwhk.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3mrpymmlu.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3algdradv.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3yofcnvjy.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3lipxoyna.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3qtgwadys.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3fivzqozs.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3mwjqzcma.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3iszmaixm.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3dahccywc.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3wqghiqxe.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3uhxkhlrq.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3mjyyewpf.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3riiofsen.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3kqxviucz.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3yriuyfzq.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3xvncpucl.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3arcyuwnw.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3npwlmifw.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3qcbuvarl.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3risxwwmu.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3jnueystb.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3alsxobao.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3zdzpxdix.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3bjgyviha.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3znodkgye.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3xwvgesiu.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3ofeuslhi.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3mdhupxfx.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3ggdlmxae.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3rcwigmix.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3yixgjzcb.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3gjplgyfs.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3txegoewr.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3kammfqns.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3qofcalgy.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3dghwlsni.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3oscimeqv.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3ytgfedav.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3tzinqphr.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3qfnmfdoz.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3rfwghgwx.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3mybelbio.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3axsvvvtz.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3sfkzuklj.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3wkcxyaui.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3ubbnrisi.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3pylfuplp.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3sdbwkjmm.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3ojyzcwmj.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3cteqqkch.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3sswwjssg.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3hnqqapiq.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3wbbziiil.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3ovwdpyze.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3esxwypcf.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3nyjpgonk.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3vtuxxuzj.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3jthigvvl.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3iuhqlbrz.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3ffjtbntr.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3tbwkqrgy.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3lriesvua.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3xwimwsvi.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3krhlfdqa.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3bvcdqpay.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3qteybmcv.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3byerjkuf.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tyyoacrq.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3ajxmyqtq.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3hbqlends.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3istemomn.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3vwfghnia.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3kwlobhia.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3vqytcido.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3fdnskzfe.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3edsiedjf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iqtvzxix.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3vzthbfxh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zhxgoqkh.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3bkspqhgs.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3jnoavogr.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3plsuhsoz.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3zaevexri.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3usgrlrac.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3ruyyhnlv.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3aengveze.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3qwoixwis.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3drvmrlig.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3khvvepre.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3xrwqetcw.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3coihzolf.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3xkfltsgi.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3xmnitgjy.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3tjcuqltj.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3xjjlynjm.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3jxzzgcwu.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3kgnczsng.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3magvmthh.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3kdmxngvt.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3nvswliav.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3gzprpndj.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3pcuuryna.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3pdowhgxv.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3zwprlrhe.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3jqxbkfiq.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3ndqlavbe.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3ylswezbu.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3nanxoekz.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3bxbomapg.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3vifkjksb.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3pwfeosmr.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3hablpanx.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3xrptrkfx.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3lwldakxt.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3uwlklxnu.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3xdxavvap.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3dypszcto.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3hwksarvy.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3tlsjmkwh.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3cdzwlqhf.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3ecwielpa.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3wubtneev.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3cenueofw.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3ralvbtjw.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3nikvyftj.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3hwwldizo.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3jqjifred.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3tcvpjqbn.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3jmulzvad.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3dmpkxsgw.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3ichlxdqy.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3kabocdzk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3imjunvgr.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3bosgercm.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3hcadagpi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lftlwrro.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3jgjpsdhi.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3oczuirps.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3nzbkfdgh.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3fxpehgzx.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3mnaectst.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3xgqtdjdd.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3qqsftwoq.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3nstdygsx.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3ziilxqew.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3qqsemlyb.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3lmvqigon.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3cyxusltw.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3rzunkrlg.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3ccotcvgy.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3wlxsfzua.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3uinftfyn.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3wymvljzd.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3tmwpdoox.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3qtdirnky.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3udionosq.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3zjafxnfr.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3jzckkkyp.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3rstflmod.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3vhmimqpc.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ajiyqovn.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3gibqglte.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3fzfbsyuf.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3tgbabjxa.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3cjphztjp.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3satipidr.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3ptjhhnxr.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3rczizhqh.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3xpcaebhl.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3wizrqmwe.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3pyzyfokc.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3imxruuet.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3aoeveqbg.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3wrwtafcu.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3nhvqacgu.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ajlmxxyi.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3pzdcpapo.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3vkjldeqn.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3mflgryed.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3jyikxywe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yptwikcn.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3febhvjrk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3eemmafnx.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3qsbnbnee.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3kyfkjdvx.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3sbqbjoeo.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3iqpcrthx.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3zxftlsdp.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3ncwtzlea.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3hzsovtsj.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3wvtgdnks.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3ucdiwhpk.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3voyycubx.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3ttapjmhs.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3betklbuh.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3kbvsdpwt.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3igryswzg.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3htzbnfuh.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3dlhysdtu.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3daeomebz.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3zjdsxzwj.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3zxjgtylv.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3hibphikc.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3wcepqfje.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3baemnpnb.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3qhmrxazh.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3jbmmoiey.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3yqwqgake.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3extjzhas.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3tczeoxjr.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3rbbrhptw.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3mkawovwf.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3ywehpvbz.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3pchblkjv.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3oyoqmoxl.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3nsawzxct.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3drerpmir.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3wwjuwbqj.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3ppcmwdkb.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3jwkvzvla.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3nugzmsks.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3qxcdzljm.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3hbjnfizq.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3dgvkkjzg.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3cnpiazyh.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3wdxxlptk.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3dslhvpvx.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3vdhgahtj.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3wthuhrmh.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3qdwoudsj.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3gwattyrk.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3sdegfhcf.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3xbzwlmks.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3qnipqqnv.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3vfnrmrdi.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3lwppypda.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3lqzwqtol.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3zynexigm.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3fmcvdshh.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3sntlmbbr.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3taywzlab.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3mtzoyvfq.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3jflqtxhs.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3cwplcynr.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3yecbyfvp.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3vcwhgiir.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3uevaeqhq.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3nlszymjp.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt3wjqcukel.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3vidwpclr.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3tngqfzxd.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3blluciga.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3jqhpmbfh.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3juxtmdyj.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3skhdalsy.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3bglwsajc.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3qviuftav.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ofeppyuq.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3vaevkmyp.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3ivqnjenc.html


<!-- 参考信息 -->