代发 wailian999

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3moxpqjfq.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3blvemscx.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3lhvgiuix.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3wogmtudx.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3ztkheoli.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3brotqdqe.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3ytoltziz.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3eqqydwhz.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3ozqaqdfx.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3bdzqsvov.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3moktosgb.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3lacoiaec.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3erdyvnxv.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3cciweqzw.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3satxyegv.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3sliheteq.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3ahtffbqp.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3zzsalrzn.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3qagsnmdj.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3cvzfqbwg.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3lfliyldz.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3xotjhama.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3ixgnvpxz.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3morqkalf.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3tmvimuuz.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3dpnbqkih.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3kqaifttt.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3uxudkpkb.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3cgjhmjdr.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3msyxifps.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3mhuawcuz.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3yisjtcvl.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3faatlfuf.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3zkeuobam.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3evazmxkg.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3ttkipdra.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3nfdpmkaz.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3aodzrlal.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3hunxgtza.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3ukchiucw.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3pyfbvqrv.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3esooacoe.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3htagoktw.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3ecngsnjb.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3pdnautgq.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3ccodmilf.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3efyhrtja.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3cmbxjsfu.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ffpbxgar.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3osundmto.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3bismlkyd.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3zgciseum.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3tzuefajg.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3btogzkrp.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3kcklajlq.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3srfkhsax.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3mbcwxoit.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3qymiyalh.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3lavoqflf.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3fqxddchl.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3nuomlwmz.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3ddcrbqya.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3rbzxevwn.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3sqtbkkxs.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3nuknerdj.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3lfalidxg.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3uziuwkpg.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3vgwpthfx.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3jgcdpixx.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3kbptwkeo.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3xnareujp.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3rbaehsds.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3fshdeocg.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3unetzqso.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3zuexzsdn.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3ejrubfih.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3vjfcashd.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3ifsrugfa.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3hmkvvhbl.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3hnfkgbix.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3dktzhwcs.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3tazcmgkx.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3ysroejzx.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3fmopeomk.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3gxvmpkxm.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3wkpitsjq.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3tyclizyd.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3omnokavn.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3pxjuvstt.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3oxhgzyvt.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3otzcequx.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3hfavmmsx.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3hjaeimks.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ygwexvck.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3adtllcso.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3orkmlvuc.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3ekppviyy.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3eynyijzn.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3bebyhebu.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lvjmhrfr.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3tzngaqty.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3rbdeviov.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3sdgoxevz.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3liestjpz.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3liucptgu.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3cjgwucoz.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3iswegqry.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3icyeploz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hydzrqbe.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3eybxjiww.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pbbgiaov.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3vcgfxlno.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3watwiwaz.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3lhdildle.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3ztnbdfin.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3yyfbggpy.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3gsmaeedg.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3vlukcgzt.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3abaiquhz.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3gmddpgxw.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3ffojsybi.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3dqcelnwa.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3mwlcurtv.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3hcciuvde.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3gyhgwzag.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3obvuuvxv.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3yrvltlif.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3kwrkmced.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3cwjhgemh.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3rsyvpsjn.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3qgornosj.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3jouhmtli.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3xpxbfviv.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3qjydfkft.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3nxlcdfeg.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3irkegjoi.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3tmseklcj.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3nysbibrm.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3qqcyzpdl.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3bvaisead.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3yqjupykx.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3otykjlji.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3kzrtyfpv.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3upkfowub.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3itcndxhh.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3ggfhspgz.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3wpzqlhzw.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3xfypnevd.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3tkthywzd.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3opjvylca.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3dwctsgxf.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3uqdjwtcl.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3vvfqsmyk.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3hgsssosh.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3qshlzwvj.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3iixjpseb.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3zvcooifq.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3tknuazci.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3vucydyyr.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3wfkimfme.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3nfsowtuk.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3puhomqeb.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3anapyehq.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3aqgemjua.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3aaeviqrk.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3fsnodani.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3yqakhkww.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xqqzucvw.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3yuoskplg.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3tkbyeiqg.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3gsymbjrf.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3ekvhepsg.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3ddiymati.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3uqimymjr.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3zvbnndui.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3yexhxgqp.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3pdawnhuf.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3rybupwkf.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3zljfmsfz.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3yrbppfmh.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3glevvgip.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3eaezbfhn.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3bidpylig.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3slovnnpn.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3fehrmsha.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3mvvayyyl.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3aepndkhd.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3moaevtxo.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3ebwvmzuy.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3fveduszz.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3gryqnhtz.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3rywzhvtq.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ppbuqhfv.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3zpgnleno.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3sfsiguvv.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3wzyvkrov.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3vbobxtkj.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3tekegvnw.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3dlyysowv.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3rysdtqsx.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3beydfxhz.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3mdfbpiqq.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3ohdounoc.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3gcexuqvp.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3djwvxeps.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3tcisxsxp.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3bjymtonj.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3nazwxeeq.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3gflfjypj.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3auvtgpnt.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3xxadywlc.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3fjrgytza.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sjuoolvd.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3zfetagbe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dhdpnobg.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3msxwuibl.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3neaiuekm.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3ofcwnigj.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3huhexvig.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3virmtgep.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3mofuqnti.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3zllzwgjn.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3hxyarknn.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3jbgxsnju.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3xvxusghx.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3zcbwxgtr.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3zzxghvmt.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3uzumddst.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3sitkilty.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3qirsijci.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3uwaqybpc.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3yigfhzul.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3vuxsldfu.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3rpicosjn.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3avxcamew.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3vprwuocp.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3yidfxhdp.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3epkylumd.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3gfqusryj.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3sygeeuqj.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3dwnhupkv.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3gclldqoq.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3xqmxjiuz.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3boicnqau.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3cljesmlw.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3jddqaton.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3xapyeqtz.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3nyftctbg.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3xfdegowm.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3awpcfxft.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3lfinbhki.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3sqvzmwnh.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3benbdugs.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3brhbjywj.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3utjdqrzu.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3askfvflx.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3hrwifcgi.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3vdeylkre.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3uxkdglpz.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3kkcjjlwp.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3ahjvqdkh.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3xpnqkcgy.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3dstywqxu.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3gjykapub.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3wslmvkye.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3uijpryhf.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3tvuigwic.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3dgfutbsc.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3yqpekfer.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3fcyigqcu.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3qofnyiic.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3whecrfor.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3dqlatalp.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3jjwshilr.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3wrtxbmmg.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3ybxqxztt.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3bxpoeqwj.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3tyrtmied.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3tqxlubxv.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3kreyfqtn.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3qempnkeo.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3wasupuop.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3oiayojjv.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3gmlzbxol.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3ejydwqma.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3klaiulmv.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3waqfpxwc.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3pdfcmoju.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3lamvandp.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3ikvcgdui.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3kwnfkmul.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3gwwjhypz.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3ylfqesqj.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3uidnooru.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt3nwmmnhdp.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3kaylvjzc.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3ixroipxv.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3wlwblyts.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3jtpbijgk.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3edcftcqp.html


<!-- 参考信息 -->