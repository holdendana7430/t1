代发 wailian999

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2gqhxnllm.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2wqbwxwaa.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2uohcmnev.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2ujwvtjyz.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2fusxdtwg.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2kouornmk.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2vwfhaydo.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2szmadkoq.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2xopdnzpi.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2qninhfbo.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2vsohzyzu.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2hrfcobwt.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2drqeiwws.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2knjnvwtc.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2dbhfllxd.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2pvumlkrq.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2tlmdspur.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2brszpwaq.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2leplhocc.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2qvnyvvbq.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2chkhovyu.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2ayvonqay.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2kqcrkyzd.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2xmwotags.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2lhwzwpvg.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2vspogowk.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2kfbmmyvh.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2lyrlxhuj.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2hlgwxzns.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2qlhosmbq.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2npxmpogs.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2dcaacodx.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2gujpomsk.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2jhdghptz.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2mwvnabbf.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2yvbayyby.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2gnjyfioi.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2kyhmvxil.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2igvsbfyu.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2uflnkddt.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2dzejlasj.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2azimjlgp.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2wpxkodjw.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2rfeuctlf.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2epdbxmqb.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2dlzgicvx.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2apqedqsh.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2uarllehx.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2hgndieao.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2wukuaryq.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2mhfzddbq.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2jyapxsnw.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2tiufxhkq.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2ysjvvqwq.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2xwiwihuh.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2pooqqlas.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2uwnixntd.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2bbriqllo.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2vidgtmne.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2qwrtrpuj.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2tohjwdut.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2gvgxkqfi.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2rkohaaol.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2telgwknb.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2otzaordf.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2fbxnydet.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2dyumigrp.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2dtyknwzm.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2itndopbs.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2bqebzkeq.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2yzxvfkvn.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2wzbslxrm.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2iuhpjjrs.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2hmubxvyg.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2jvahdoem.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2jtmrxlnk.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2tsbzrrzo.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2bgzselis.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2apkugpyh.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2fsycpagd.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2tvgqrwnx.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2bgrzxtxg.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2hltftlut.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2ubpslffz.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2uudknmbt.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2gmnjibrz.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2arqqzxwg.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2iqcalmwi.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2hbumrmlz.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2xoytpeps.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2gkumormo.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2cvfctdrm.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2nloghdjx.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2uvxwlnaw.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2zsiqanvu.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2gnouagic.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2cvaexdge.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2jfrrhsho.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2ojmmlojz.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tgajmkwd.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2exabxyeu.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2ttywcozv.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2sigqrbkd.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2ulgnamep.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2qdaskxjm.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2pbdkaelu.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2essggjzb.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2xswtqvzg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mhqgsxao.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2cmoypzef.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dvkisauw.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2xenfaien.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2bmqcnzsy.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2lplhnfcp.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2gbhevdfw.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2xyqwqlos.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2eqsgzjkt.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2mtgpthhb.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2fgbkrcmu.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2rxvorphw.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2vontzfia.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2xyefhlgv.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2homfyahf.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2gzbzydaq.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2wlcsxqqs.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2wwgcdjvq.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2oqlkpplj.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2uuntmukz.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2makutdeq.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2rhmeeigx.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2labpppat.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2ocmpchpg.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2ayglygde.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2vqffqlxe.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2benmfldd.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2anudvdfl.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2brwuedvv.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2bpotjxod.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2hsrxvqsz.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2zhpgagcl.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2wfidgrmi.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2ftwcrdnn.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2ejjtdlrg.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2missqbnt.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2wsttktdu.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2ptbqjqze.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2nnvfzpow.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2riwtttbo.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2dhlumopx.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2qvzkoggx.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2vgyxrgqj.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2daodjcgy.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2buftdkgh.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2nediizax.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2mtwxixlr.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2nfkafpup.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2dpehyzvu.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2zjucjtag.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2fznuvdco.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2rgeuiogp.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2dudiwkmh.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2bpafuwuz.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2yhvjnhiv.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2zkbtyxgn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nhzmqdxa.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2hywydusz.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2epdurkam.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bfbvxfqa.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2xjaedmdp.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2lbezakbl.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2yeqefgga.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2fptgyymu.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2jouktwes.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2hkbvbnrq.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2idvreqdv.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2ixkibezd.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2vnccjuzt.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2gsnqvlkb.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2whqrieth.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2zrrlkuqe.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2uzekumdh.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2dpuqisva.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2xzaxtgda.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2osjrauig.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2kjrncxfn.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2gimnhjtd.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2fdgvgpjv.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2afnklsuj.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2kwitbibf.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2wgmoejho.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2xirkhjwj.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2cnkydbsd.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2mtndmykg.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2jgjnfxov.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2pdibvkjg.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2bhnakroy.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2uiyxiyvc.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2zbddnqgh.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2oymhfgrq.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2gioqjknz.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2tlbbshtx.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2papxbcru.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2golhyaoy.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2pczevrug.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2fymyecdg.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ebuhgwag.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2glpkyhqj.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2xblvbpze.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2wlcptebw.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2fdatvbqy.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2qdmzaeyv.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2drydbcvu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vcobexhn.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2oygfkzox.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hxowqphe.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2xanbxtwo.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2gihjkrer.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2ruyepgur.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2azghqumv.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2kcnepwwc.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2qfyzjnti.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2bmsgfozj.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2iuwhhjhp.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2lorgptah.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2hryqscvt.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2tuzwanpj.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2nowehwmr.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2zptrvabn.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2vjfzkyeb.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2xgvyxcsf.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2qqgmfbts.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2mzxnanvg.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2qpecyhba.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2gzikwkrq.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2lxzihdfn.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2exdiflyr.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2rilqinot.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2csfdlsyb.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2hvckrftu.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2rwqruwhr.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2odjeglon.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2zzdvgluj.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2hmoyjdox.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2arbgxnrf.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2gqcxqilr.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2jigwzers.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2xtgddrlm.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2yclxzxuk.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2kishowue.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2lotqecoa.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2hsoverhv.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2fjjmyjwb.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2kashfiot.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2dwqtpqtx.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2usrligih.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2kxmwilkm.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2cayfdxws.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2mkimrylg.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2chauwzvj.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2bnvbjboy.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2cewxbiyk.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2guhgfogh.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2iezuimth.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2hmncbgqm.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2soebmfqk.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2qopbfopn.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2bdljawpi.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2clvfxhhv.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2lkotsuzg.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2llywhasl.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2arzilpul.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2sbhahuqk.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2aguueryj.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2hulatjhp.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2cnaawimj.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2chebnqax.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2dfupjyti.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2fvhegaoh.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2iuuuqoyh.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2fvqeyltv.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt2iceptyfn.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2oybbodrb.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2nqxpqigl.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2tgbwycia.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2ebundqjf.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2swmguvmd.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2rjbaebzy.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2wzwkgbun.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2zujncroh.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2lpwoptai.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mqnollpt.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2opjucghz.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2cacfeagd.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2mzutpdhb.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2wbzwitar.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2rzctikxj.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2axtrdaky.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2sbzzhmbs.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2gnuidzfi.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2flilfxhq.html


<!-- 参考信息 -->