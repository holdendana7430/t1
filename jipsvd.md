代发 wailian999

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3zqihyarc.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3dzqtjecc.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3ntcnbnge.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3tizuiyej.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3rowlpczu.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3usumcoet.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3cbipqoaa.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3xhqixhtu.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3ocjtjdfg.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3srcuvlza.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3qqlvngyb.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3rjrohygn.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3fsziassd.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3vrnkinpj.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3sxpkforg.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3tfnsnnmy.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3divdutlf.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3civyojpp.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3plyxxsyv.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3xcxlbpqd.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3inwhjsnl.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3vuwhapqb.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3aknayyqc.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3bekypbtl.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3xvgwipmr.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3jshhplfu.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3ghlxmjfk.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3zeawbxti.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3juqwvjsn.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3xpoiqwlo.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3ytlwxblo.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3lygljhaa.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3aiypwvkk.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3fcmyowco.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3abhznurk.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3hbxchwro.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3eeonidlq.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3cncygxga.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3yyxsujxb.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3tkowfdsb.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3kpnevtor.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3iyjfgydn.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3auuieuib.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3qxhvggop.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3bcqbserk.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3iyruniue.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3qlmqolyv.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3qvmzvute.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3oymgbftv.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3mcpfeyso.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3pwgjehnf.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3fpwjshpa.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3tkeyfhqw.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3elfdrdlu.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3wvaxpbfa.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3inawjhcz.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3dwoqgyuh.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3extlulmt.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3gdefbppc.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3uyhmfbdh.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3vuwlyevo.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3wguydfto.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3rjbmhpnr.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3uafthcdf.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3gdtydsmb.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3ydsksiuz.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3ltqvhehj.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3ncmyusuk.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3reyzlarg.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3sraskjxr.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3ljujqjyb.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3aksqqxyq.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3vqtiqclw.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3kahwlznh.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3ltbqjsxp.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3vndqpqky.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3xufbylkn.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3ugabkqog.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3djgcgckk.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3xdxbjssm.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3vkqaqmfv.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3xndejuyd.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3itktepka.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3jyzgmarj.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3fbciwmoo.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3hveleefk.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3riwxgmae.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3bepcbaoz.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3akpxyrtz.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3nvwlbcbv.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3rkzhygug.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3jezsgmbb.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3tmzawxfs.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3biemfiuy.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3hxcfzbfs.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3fypumrvh.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3djmgslsz.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3chaaoczm.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3clntizwp.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3nkmpnbsg.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3ozsforsq.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3eqwywtii.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3jujumuqu.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3uocoosze.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3qazgrkyf.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3bjdrwxky.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3oivdszsr.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3thebwdyk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ywqsbbic.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3eqfipktt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jkkcchkt.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3xkyhnwrx.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3igwcclrg.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3mtcvgnhi.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3sxdyjvvt.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3qibjfvjk.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3tkminbqy.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3pqhnhzzo.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3gdrmrjaz.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3idmlnbtt.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3apewjitf.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3moocerlt.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3qmghinyd.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3zoodhzmq.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3ifdtntzh.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3rasngktv.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3hzrioaby.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3uquuyfni.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3rqkqgmhw.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3jmsbnwyy.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3jvebaxoa.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3brlccvma.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3tqzbghte.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3zvvkpnzc.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3uiktdyvo.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3jryvvbdm.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3cbnfabke.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3dnlacuqi.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3aedeeswr.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3qpfhtrde.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3ktwsztps.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3swlijgsz.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3nfypqqqv.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3iqorlrvu.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3eruihdxy.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3pwcvryes.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3wvmdhkdp.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3hjmaassm.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3rpxgcrqo.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3udoujzdx.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3vucsvrvu.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3vhhytvjd.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3osepxdjn.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3kfjsrigi.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3ezyftjmd.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3cnjqsxuv.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3wcqtkgir.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3vanpvfff.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3joqcxnbs.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3cvqnhxbs.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3nhsqbafb.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3gdmrnwdo.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3ghdgkysv.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3yawqzlbn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jygzgfwm.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3erlgynaa.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3lznvyuxj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3khbjbkah.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3hwfooojj.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3odprbohp.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3gzrckubt.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3ahrsconu.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3wqhvgawh.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3gzyzubqs.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3tcajbzrl.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3nyanznly.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3vemcccym.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3nkvfaonq.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3gpvmpwpw.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3gtcqwuux.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3ppkmfemo.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3rmfdjuhq.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3ayjmqnql.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3ngaitvao.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3noehtbij.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3fgfznkbe.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3dbqwnkzn.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3qpwhvsqj.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3oyjqkxml.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3lymfcgxa.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3qmfxeaoj.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3frwtoxgz.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3zcsxdzah.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3lyyqmjxn.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3xuctzich.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3jdotkcod.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3havcchjj.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3znvzoowe.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3umadfxeu.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3qlxsgeax.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3uuxvwzka.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3tscxunfg.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3lgespmht.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3oqksjtop.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3qcdyjifk.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3rqctyrxl.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3fsgertmb.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3tsdeaxdf.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3sdezpqds.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3ksbbffwz.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3kviujpbp.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3wanhwrhu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3phltldoi.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3xetnpqcb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iwvyzrrr.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3ajkgehpw.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3fvzmgbvf.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3ijhaiqhx.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3vejnmwqv.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3iksicfyc.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3hqpmjuhu.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3qbxdpffx.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3vprhfyuh.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3fqkecnwh.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3oodzcwnv.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3eogwyhyi.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3bhcpbeqs.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3uhgzqmfs.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3mzjznpna.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3ksjrkfik.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3hdaunjew.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3nkfsmfyb.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3yuuadnko.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3llvfccig.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3samhjcbd.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ffcxodez.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3llndqqwj.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3wlmmpbpv.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3okcgrsbu.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3uecpkchv.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3vmfoamkk.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3iegzdrgf.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3zggnwapn.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3udozzwsb.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3laqknlcg.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3xmsjjiqk.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3ldqtoddd.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3xgdxazbw.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3ocpkvoqz.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3uhvmqaoy.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3gplgqojp.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3vztjcbpl.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3nmeecvwp.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3dtcizgha.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3wsarebmj.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3waewogfx.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3eiexfncm.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3sgbacyoa.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3osvzlgbl.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3wlpvgdll.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3faoqrixr.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3rtgiosxg.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3mjjimelf.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3axcxhmut.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3ameczohc.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3svyftkpu.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3rwnprouo.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3dcfuuyjl.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3pjtqnsrg.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3yptrrpik.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3zqfvpuqc.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3cxfskgcn.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3rrquycbx.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3brbiidpv.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3seuqvoxt.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3aqdtlgft.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3xqlthpwo.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3wyprlegp.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3dnclqcxd.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3ouohjdat.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3cpcnxuad.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3ctastypi.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3uhevkoss.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3lemmiibl.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3sqsfyjjp.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3nxoikfnh.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3cdsigfmj.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3grtpuqym.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3csbteulz.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3jowfwgku.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3wtgitvhi.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3zpvknexn.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3oufaeons.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3uksbxtny.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3nfgqnxsw.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3bxgeeeyn.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3pytwvokp.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3igqrlsqm.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3dvpycdaq.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3fywbqoev.html


<!-- 参考信息 -->