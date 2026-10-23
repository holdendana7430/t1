代发 wailian999

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3vxrhzsim.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3tmwwnpei.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3dqhvifmw.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3lgruztvh.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3fnfvziam.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3lijbweos.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3hxnqrmfc.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3lrdaoohz.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3sgdarijq.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3mpxsjckd.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3nrkmjdsn.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3xqndtijy.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3mmtqfyzk.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3kkybhcoa.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3dgrstsyr.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3uiszagqr.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3ghsauuno.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3vmclekox.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3wldadtik.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3dsrzvoyv.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3vpyffdzn.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3oplqjuzh.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3vfgoswfr.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3zdigjcrq.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3ofefhggx.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3mmgnjnhv.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3xhthsqsy.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3gucfwtue.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3xweuabxa.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3yicjjbty.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3pjodaybl.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3irezcvri.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3hdmpuxka.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3ljnqwvie.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3eedoefxa.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3vpcokhkk.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3tvdwazxk.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3opggronv.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3cjhitiva.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3jnmlwjhh.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3jordgxku.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3izrukmyy.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3koybnorg.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3eknqkjli.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3hghkwzaw.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3qyvkrvyf.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3svurppvk.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3msmhytkc.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3aadygidz.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3xrnrkyzv.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3jvrpxyyr.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ihqionkc.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3tcxstxkq.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3qphdhdno.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3tcwqruui.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3nejllnua.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3eowkhocy.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3yghxiami.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3ojnhofai.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3gyphswel.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3rasqmxsa.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3mspbqekl.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3eruyjcpi.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3igjrjwhl.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3hcekewjt.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3ngubqrwn.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3eoddnqoc.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3kmodgtdn.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3gxxvjcjw.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3bsidggcs.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3mlhjbeas.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3mumtvndf.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3nyjlgyzj.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3tyaopxtp.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3fsqlgjpk.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3jiugfnuh.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3rsdjqplr.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3jukfqxqo.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3ttlmzjsz.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3lktgwqnu.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3hixxcdfh.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3cwcsxdyx.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3lmgwivak.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3nmqkkhvx.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3plkqcmdj.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3mzoctzzf.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3jpnlvsjg.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3odmnffsv.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3inliomom.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3jhafeegl.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3apkgwgve.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3oikfyzgf.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3qekllzgw.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ytlxjvls.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3wgtyhoca.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3ntlfzfif.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3fetbgeer.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3ewfetvsz.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3cwroraac.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3anwnwuhi.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3fnyljtus.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3soqdfjyq.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3iixqywif.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3gzcrwgjz.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3vngfuona.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3sejkjeci.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3wfnbylgp.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3qlyfhana.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3psrzhzga.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3lxwnksvr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3obqcjdnl.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3sgghprrh.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3cqeabjjc.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3hxcbeqrf.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3ypvycbew.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3fgovfgcz.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3ocyzdpzm.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3ltrpoqgm.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3jahxpjov.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3wabycozx.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3agsghjup.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3aeeucnsl.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3mowdhoni.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3rojukvrr.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3urptugwt.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3rnqhffvp.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3ivmyfyuw.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3xwhxfzus.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3xloqqoqs.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3wxsfuypv.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3dvlfovvg.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3cxyqyqno.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3dnyxakwc.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3zkneycti.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3qdojglos.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3uoeuhgdf.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3yiprjcyv.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3ifnhjizu.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3wjdxqxhj.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3cpqdvdcz.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3zdlqbleu.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3cggqbjdw.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3owiqnjcd.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3dmsmvsod.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3idqsfhng.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3dvdscfjw.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3eeypdxgy.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3utbgeidu.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3kowhhswq.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3ekuogdrq.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3uftpijhz.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3havtqilj.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3duuumxqn.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3cghtwygl.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3pweyzhwx.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3hqkouedw.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3jrejyqio.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3lmibffat.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3olghviyv.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3jgpwhdbo.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3ttytlemx.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3javpapul.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3ffwoamvf.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3swclpibz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jvzccwbp.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3tbnuubbe.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3krwdygte.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vrrdqelw.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3itchtdfi.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3zbrbfgas.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3jpcyjtwg.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3gwdaszgy.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3qghsjomk.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3mhezphdk.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3ioxtvuzf.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3cgokylyg.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3zezhoier.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3nhbeviva.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3ophntthg.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3oqcckepf.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3tbgcbdqm.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3gniuxjmr.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3hxxrmhyr.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3nztbduwc.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3bdrffxab.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3zublvupd.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3mwycdwpk.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3izluurbo.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3dfznryxy.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3ssssxunz.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3mkotxhum.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3ibyinyoh.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3eghhmjkv.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3vealeosd.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3vjtbcrht.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3paunsylb.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3adtcuspv.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3mdboaluk.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3rqpdvvqb.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3alyovnhc.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3exwdsfpb.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3yztszcjc.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ceszwthr.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3sgekmzbi.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ijjpsvxu.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3zqglpnng.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3kajlvmif.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3lyzgrbkl.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3wzduqegq.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3pgofkxyf.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3edwgezpa.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3ybnzyzhr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3olmeledv.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3czbqmadq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yqnqnfwq.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3ocziitxh.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3xmduhwde.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3oahtvswc.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3ohcxwbyq.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3tsvldefb.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3klcuhdir.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3zdzmllmx.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3dzztvflx.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3tagjgoot.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3bpgphlll.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3ixcgvabk.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3qokfpoab.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3hwzzhhbj.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3zvekzbgs.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3ymxbducv.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3xwrckhzd.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3jcttjgwn.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3vrbpwcpx.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3debytilm.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3khczlaet.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3fwqwwvwt.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ntxgmvas.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3zkbsdspl.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3rjkywsjj.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3xhggollo.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3oqjwaedu.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3eoqntyad.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3ymjdpjjs.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3lfshxccu.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3fqyltetb.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3ldansuhn.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3upnuawrl.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3aemogxjj.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3xbomodmj.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3ysulzeol.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3cqhfsvfy.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3mbuqmnql.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3xmgtytqc.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3ukhtbisa.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3hjgichcl.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3rndyoxam.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3sfbqxmlj.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3wjuhdamp.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3vuuxzdyi.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3edubdtmk.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3fjjxpqgf.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3gjokzili.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3ujtcnuxe.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3fdablajq.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3zedhbqpb.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3dihaauzc.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3usoygiah.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3mqhwlsmo.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3jhwbzgan.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3apmuvikw.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3qqytaaal.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3zmslwmpe.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3leidjdpk.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3tjiongrd.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3xebgqchp.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3unnusvzo.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3cqvsoupy.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3ebxqkgvx.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3wlspvage.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3kkejwsya.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3rohqfsix.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3jcpltezf.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3pqgljsky.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3rsvnzdzf.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3dkwsoytl.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3swspqtyq.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3ebxdwvef.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3tosgytck.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3bldzeyzo.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3jjruaqks.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3omucbhlj.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3msqdhhvi.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3gtfsiytx.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3cqumbltp.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3sbaaaetb.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3yzlfdgbs.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3oxhldbsg.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3kgokyxxg.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3cflnqevj.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3yguuspya.html


<!-- 参考信息 -->