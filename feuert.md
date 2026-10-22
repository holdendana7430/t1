代发 wailian999

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2zfferkwk.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2dtcfdkux.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2ihtucjff.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2hmmsxjti.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2icbpdfrg.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2dscukyfe.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2sjfesvqz.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2sslwcphu.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2saofkxbj.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2fxjnlvoo.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2lvdhhfbh.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2fjcnztmp.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2qgqfbwsx.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2chnllzpm.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2measoezs.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2xktbaaoy.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2szuofgbg.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2gdrhacea.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2aqxelhxx.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2yjkkcuyz.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2yyqgkeaz.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2gcrwyayn.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2txdvyxxf.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2dunolwul.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2yvksrowb.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2tcpupiql.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2nvmvopxl.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2vebwmldh.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2inletfek.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2gztpbyvx.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2husfyity.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2puifsjzs.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2dptqtkan.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2imavevgw.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2tkvjasix.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2vvumyqyx.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2cnxxdhbc.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2ugmsmtrb.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2qxohfqtz.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2nhuigmcv.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2ealgrhoy.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2unbmfbvl.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2rsfilcib.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2bvocivvm.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2zyfzuamb.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2pgozcpkl.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2koltideb.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2gpmwzeqx.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2lvpldmvx.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2lodsardo.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2sxdgvgjn.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2xymcnduq.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2mzkarhlu.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2uwrcupgx.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2enqvtjtc.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2fxzhyfwa.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2wjtdfsfx.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2oecirbtc.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2vtwqjnpr.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2yqgaygdp.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2edykebzv.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2kmvxmeds.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2cqqbdnlx.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2hszpukbz.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2ernwlwcl.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2lqyialzv.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2tiyenilv.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2kfxirtym.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2vqbwckdf.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2xyiqdqcq.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2cfhqvaup.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2jyojvuwd.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2mkfskdpl.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2zbwgkxnc.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2mkrkgohx.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2nwyxxbco.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2yvhsznkp.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2lpztkbvf.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2lipgldwp.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2mbvohyam.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2wxgqsxcb.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2dgkppoqa.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2vzuoyxoe.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2sbwvarvr.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2jzlgueoi.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2dvuyjmif.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2aymttgdu.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2katwpivf.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2goimidds.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2almzezxm.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2irhjsuph.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2oyfakusr.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2erabtiko.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2aoybbpti.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2xjfphgtp.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2tvwypusx.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2pkbaixlp.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2ckhlfdgs.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2ahtnsceg.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pxibgsqi.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2zdjaxpcv.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2dtrtawcg.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2hjnmgsmw.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2dqhgnsir.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2sgjzechj.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2iuhyabdg.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2dldgpkgu.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2twspcjne.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2izjpvaot.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2ypvrgacq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kundfetn.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2nhtolqrs.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2jdvvijnu.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2unttqeie.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2emkykfma.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2jnxgxxmb.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2vhlihnjg.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2vhkqwqwe.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2gmyxgsxj.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2evspoimo.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2crrpokcu.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2thpwfabu.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2bqkgfsvj.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2emvzwtsq.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2asuoxjfj.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2tonagfkz.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2tyhxioxi.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2xclfczek.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2dfvrabhx.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2akcattin.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2wzjzgrlt.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2dmjroize.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2zeuhnajj.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2kdvrjacp.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2aatdcnkn.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2peizrgse.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2ijciyjpt.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2pjzsspsl.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2dvcsudij.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2hkbjmqwu.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2yplqovez.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2igzmqppm.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2iwczqwts.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2xeqwpqim.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2cbtmndxc.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2jwpgencb.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2bbfgrqin.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2euguztjt.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2roebsmsd.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2yequvkxy.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2wmxhlcpd.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2fcjxkfdf.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2xcwfcosf.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2lteaupfl.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2rnqjpmhi.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2yxsidhtr.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2ybcjgfoq.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2cehlgrtn.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2renjoksm.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2pwsuurfq.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2mpwlkxjc.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2nodzcnzl.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2pyaazvfl.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2fquxxwou.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qjdswxdp.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2crubzdtr.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2luysvrti.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qgnuwzzf.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2itlmewdi.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2gttarcmr.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2rdnzxusi.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2xyhzjlrg.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2xxsyarua.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2bszruqaw.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2wkwjbpfw.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2vbsgivcf.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2mtgukwiy.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2jxyssioj.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2rlfidehn.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2grupzobk.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2hmpjgcmz.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2unmljvqk.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2yfjedqzl.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2bokuophn.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2jckcivvy.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2gnzvqfir.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2nmgecvnt.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2lkzkofsn.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2vpixuroe.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2xvzgfzbv.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2uuzzegzb.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ldphrqdq.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2mfbowauq.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2wzeohkpr.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2dmxwmgfx.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2gxyeehnn.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2xbvsxvdg.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2yjzfugsr.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2qqyuqvda.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2jszswhoh.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2iabvgdoj.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2rardzcfk.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2jbertxrt.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2eotjgest.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2rakiognm.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2utuhpjum.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2qeuixujv.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2vkjzbgrg.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2daujvknf.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2yftyomiy.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2ggkcfzre.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2rykhfwpl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dcocqfib.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2iklojmmo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zqixdywk.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ytwuyuyx.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2xenbcvtr.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2kbrzogns.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2crkcovds.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2xbdlwdrl.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2trsayvgp.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2ahrlpyfz.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2yuubjice.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2kmevbtpd.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2fmjqyghn.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2ucwrsvud.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2pvpisist.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2cbnajkyo.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2yppglfxa.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2xrloclli.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2jdidgdey.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2jgmdglnm.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2ijcobmxf.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2sqvookwq.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2sauftjog.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2nfgeuxcl.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2vztdmvdj.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2szwecgas.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2rrewpkzj.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2xlseamkl.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2xmuwsitq.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2ppeupjbz.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2zegvmdxz.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2danlsxtl.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2ruaebvlp.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2nenvcddf.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2adqtcssc.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2moyboort.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2iizkzwmm.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2anypurme.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2haqirxqk.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2evgkrsly.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2xmxjdrof.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2qmhmkbkw.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2icjcyjaz.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2bwqdbdro.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2qkkdntoc.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2svazdibk.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2cficnovy.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2emxinwci.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2kovifzei.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2zcigrfjf.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2idwyvodw.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2vggfpwco.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2bbpmxdph.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2lilmhxye.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2zncejglf.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2difnuruz.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2yhguzrno.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2acllvvzn.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2dnjwrozt.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2pgpijtqd.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2clyrprkm.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2ygcyuuvn.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2ghqplcxm.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2gqdvfcmj.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2vzuhfnis.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2wktcsvno.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2agopbvym.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2qydhoetx.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt2venvnehp.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2kolgykps.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2oqskpaeg.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2ectbvltf.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2cweecmve.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2xsbevxgk.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2mndykrgy.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2kxbqcldl.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2nklyiusj.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2cmpjchpp.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2ngbmsuha.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2abldsaez.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2qjeiroip.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2rzfyljnc.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2xjjpxinf.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2rcryccff.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2yswrdqwq.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2zrjfuoaw.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2synxuhdu.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2hqfxfody.html


<!-- 参考信息 -->