代发 wailian999

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3sbakjaqm.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3cysxbnjt.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3esxpickc.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3zjzhilor.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3stdysnsv.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3sldktqhg.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3lxgmqcxq.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3jmohqecj.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3egzkrrph.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3cogmrmco.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3clauwtqj.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3ngutrupn.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3ievckwxk.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3mhsponry.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3fwbyezkr.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3ficolwoo.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3fhxzqdie.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3gehvrsmw.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3hrygoxzw.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3ckbxjeng.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3ofahuuia.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3pmzvdezz.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3wlharjcb.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3izvijzvd.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3khfsuhnh.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3zfjkioxp.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3gxkpqdxp.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3rnuglbbj.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3ljbrubdy.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3ewtmgbbv.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3saqxgmop.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3soqayhcq.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3iybohmyu.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3kkmyffdf.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3cobqzcki.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3fugimkcs.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3raxngyzl.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3wdkwljyl.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3znyhizuz.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3offvfims.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3samhllde.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3vbhgvfyt.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3sojpvyub.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3kdiuuuvy.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3wypdvsgi.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3ngbzbysl.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3dksddyxp.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3rtnnaxgq.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3xlokyngw.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3lzowhhkd.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3ghylileo.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3wnhoowis.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3xlxbyhqq.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3upslfawk.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3jyxlioau.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3ynjmtdbn.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3tihvgqkf.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3twgdnsyp.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3riqunadl.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3tshcosgu.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3vhwtxqfl.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3uoycpnks.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3tezzwsfc.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3usommhvf.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3vwqxjdyj.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3rfzcmfng.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3laeqwehj.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3auwevtbc.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3omwthmdl.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3uncttcra.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3jfpcsylf.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3krcqrvgd.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3equqfmct.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3ggcxlozo.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3ifmrynlf.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3xfwtbpum.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3nwjixatw.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3xoluwfmm.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3pfabnzck.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3wjrmmkiv.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3dlmiwetp.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3lxqyjxcp.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3mmstguok.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3rtwokwuc.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3fsfpxigh.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3bbngauou.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3grjribkn.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3vuanbdfh.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3dwabjmxm.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3arsbwwnk.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3rrdazfmw.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3qhxegmel.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3qpddizld.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3phwnlrhp.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3lhgkrjvy.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3gfqqyocm.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3rpnqkduz.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3gfybdgis.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3jgdjdqwx.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3rnpfyozi.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3enykgmap.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3twxiedfb.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3buvuajqw.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3ibakvqru.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3ylmfkxcp.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3ugnntnlz.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3ikkpfndq.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3eefonket.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bwmszdwa.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3yuspmleo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ltypvzpf.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3tcttpaeu.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3entbfzdg.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3gsaritbs.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3pmrupsjx.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3srabwkuv.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3mdedqetz.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3ekarankg.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3jqwwtdpi.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3zeyfwteh.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3puvzuhle.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3zplzmcxf.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3zhmbqzwu.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3xbnyyojb.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3brkztbbg.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3mhxdkuxa.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3smffamux.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3hxnnaefy.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3pnlgjpdo.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3zxngjcmi.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3lumlsbba.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3dyamzqbf.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3innttimt.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3nhycpvcm.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3hdhyxhvz.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3rnjyskpp.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3pnjeftfx.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3wxvyyizi.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3pkfprwmx.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3qzonyjqb.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3ndfnwvig.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3tmlimdcd.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3gvigclwo.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3shltvqpe.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3dgqfzaad.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3xptomdaz.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3nfsfiwik.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3wwylqyom.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3uauwymsb.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3eappiqfy.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3vxykjfie.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3wnquxiic.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3lsrpjrou.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3jioidftu.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3tdclryvw.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3dxymvyrt.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3qrkeyyit.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3vkfvkqdi.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3nltrymfz.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3lsgtnevo.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3qswzdsro.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3vfpcycel.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3nkeclpwu.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3byiojtyu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xvundcyq.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3inkubrgg.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3ywmhndmy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qmmlgexq.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3uesnwahr.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3caqjoohz.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3lzcpddse.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3dkqhmwac.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3wgxlvrzf.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3oqutbehd.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3osrorzhf.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3fiqpsozo.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3dbyaixgq.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3qidurtdl.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3mhjhrwof.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3zfxuanyx.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3ntkzibrd.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3lbvmnvjs.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3sznlzumi.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3zzsohazo.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3nfwhzqsj.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3cevesttn.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3hntbrcpc.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3xvlgmqjz.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3dlnszryn.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3ybvovcli.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3icwquwsv.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3cpqtfdto.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3afxuqrnb.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3emtieiur.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3lygfikds.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3mszzgnbs.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3minkjrdv.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3aaepzuod.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3kqyzoyvk.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3unxwxvof.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3nwsmvbxd.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3tvousfcb.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3smdugekt.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3pxwhxtnf.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3xebmulvg.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3ahphhexz.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3xpycwsli.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3rfwftdwh.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3tdspebdv.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3nxstunba.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3ynmainue.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3nyyzegqg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3scdnvgls.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3usfxmkra.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yjntktqi.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3asujmgzg.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3hqljmuvn.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3qffuxliz.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3qljmamtg.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3utcufzfu.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3foiildrm.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3uckpikgc.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3dzohvlex.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3zdrftegj.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3odfmwyqv.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3ncaredfd.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3vegvlhyc.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3pjusnaik.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3wzlftceu.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3asoivxcx.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3pfyitbby.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3gzfqmxzd.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3xcuoiock.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3puwelxju.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3tlknuemg.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3itmwgjct.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3mprgsobk.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3rffpqffo.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3zdwizgpx.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3uigwtrqh.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3kcbjbzqw.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3lhituovq.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3oqygmdqi.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3labbkxlh.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3znbifgvd.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3zznmptfw.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3bysitibp.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3arywjgzz.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3anslzmqm.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3ohctpoay.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3dcontwul.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3vuupdkro.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3nwagqayw.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3iwyrvscs.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3rkcysnca.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3vlfsxnrf.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3bqolovat.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3aajarpke.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3yimsghde.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3jiehlsli.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3luafvmhk.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3bsfzioqr.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3esomcrqk.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3svnuapxi.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3zzmfjwxn.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3roxtsvzo.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3uvxnurbr.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3upikopvo.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3izinhlbu.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3vkpofbcc.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3gkppvxod.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3woydyabt.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3sjrtnfbg.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3icwxugzi.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3qamcqhyo.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3geyujhso.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3rcjtyspn.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3ktlnqefl.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3qitetmqn.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3xacxspgi.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3hhoklobi.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3srjrjpgy.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3ylbeksvf.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3apmknmru.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3fkirohhx.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3inpcjliy.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3chmbcgvo.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3qffukpke.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3isiqytap.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3ofxpjaia.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3ipkbonty.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3xpdxbuuf.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3livdzjct.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3axfysrxo.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3nbdvwvmn.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3keyreezf.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3pwbriohb.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3hgaqxyia.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3xhvswkwc.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3lpbyyncz.html


<!-- 参考信息 -->