代发 wailian999

[U63] PHP：文件读写
来源：http://read.share.fehbvm.com/Article/details/gigpapypp.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.fehbvm.com/Article/details/gviwybcxn.sHtML

[U64] PHP：目录遍历
来源：http://www.m.share.hesvh.cn/Article/details/grhfvsgor.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.blog.zdbjq.cn/Article/details/gigphivlu.sHtML

[U65] PHP：会话
来源：http://www.m.share.zdbjq.cn/Article/details/gikyzkrkp.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.zdbjq.cn/Article/details/gxgnayntg.sHtML

[U66] PHP：设置 Cookie
来源：http://www.share.zdbjq.cn/Article/details/gsqpokyub.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.zdbjq.cn/Article/details/gpbkwfnxd.sHtML

[U67] PHP：处理文件上传
来源：http://www.share.fehbvm.com/Article/details/gdfxoevsd.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.blog.fehbvm.com/Article/details/gzilpreah.sHtML

[U68] PHP：PDO 连接
来源：http://www.blog.fehbvm.com/Article/details/gawwssarn.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://read.share.hesvh.cn/Article/details/gsliiudyu.sHtML

[U69] PHP：PDO 预处理
来源：http://3g.zdbjq.cn/Article/details/genhfhopl.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wap.hesvh.cn/Article/details/gswiepwtt.sHtML

[U70] PHP：PDO 事务
来源：http://m.share.hesvh.cn/Article/details/geiyompkc.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.share.hesvh.cn/Article/details/gfomdohwp.sHtML

[U71] PHP：抛出异常
来源：http://baike.fehbvm.com/Article/details/gzaapycgt.sHtML

throw new RuntimeException("失败", 500);
来源：http://read.share.fehbvm.com/Article/details/gkmlqkgrz.sHtML

[U72] PHP：写错误日志
来源：http://www.m.share.hesvh.cn/Article/details/gtgaxukku.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.m.share.fehbvm.com/Article/details/gsdljkkrb.sHtML

[U73] PHP：读取 ini 配置
来源：http://baike.hesvh.cn/Article/details/gqobxyjvk.sHtML

parse_ini_file("config.ini", true)
来源：http://mobile.fehbvm.com/Article/details/glqtbdzif.sHtML

[U74] PHP：读取环境变量
来源：http://mobile.fehbvm.com/Article/details/gcqotvkym.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.share.hesvh.cn/Article/details/gbotmzeky.sHtML

[U75] PHP：依赖注入
来源：http://3g.zdbjq.cn/Article/details/gzacfwwpr.sHtML

composer require psr/container
来源：http://www.blog.hesvh.cn/Article/details/gnrhfjgci.sHtML

[U76] PHP：简单路由
来源：http://m.share.fehbvm.com/Article/details/gbelefwsr.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.zdbjq.cn/Article/details/gotkscljr.sHtML

[U77] PHP：模板渲染
来源：http://m.share.fehbvm.com/Article/details/gdqtasbdy.sHtML

composer require twig/twig
来源：http://mobile.fehbvm.com/Article/details/gmvuxvjuu.sHtML

[U78] PHP：单元测试
来源：http://mobile.hesvh.cn/Article/details/gqbgowmvz.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.hesvh.cn/Article/details/gllspeyuz.sHtML

[U79] PHP：静态分析
来源：http://wap.hesvh.cn/Article/details/gbidgbcpg.sHtML

composer require --dev phpstan/phpstan
来源：http://3g.fehbvm.com/Article/details/gisykktiq.sHtML

[U80] PHP：代码规范修复
来源：http://m.share.zdbjq.cn/Article/details/ghwlhhkjh.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.share.hesvh.cn/Article/details/gmelwetwc.sHtML

[U81] JS：初始化项目
来源：http://www.share.hesvh.cn/Article/details/gypzwuzkf.sHtML

npm init -y;  npm i express
来源：http://3g.zdbjq.cn/Article/details/guwiroxun.sHtML

[U82] JS：package.json 脚本
来源：http://blog.hesvh.cn/Article/details/gcstwradz.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.share.fehbvm.com/Article/details/gpgxzbgiq.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.m.share.fehbvm.com/Article/details/gaqaistsj.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://blog.zdbjq.cn/Article/details/gqwdzifra.sHtML

[U84] JS：CommonJS 写法
来源：http://blog.fehbvm.com/Article/details/ghlnshfcc.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.share.hesvh.cn/Article/details/gddukehju.sHtML

[U85] JS：可选链
来源：http://mobile.zdbjq.cn/Article/details/gpijsoruc.sHtML

a?.b?.c
来源：http://www.m.share.hesvh.cn/Article/details/glakhplom.sHtML

[U86] JS：空值合并
来源：http://www.blog.hesvh.cn/Article/details/gqbhwkskz.sHtML

a ?? b
来源：http://www.m.share.fehbvm.com/Article/details/gffxlzkiy.sHtML

[U87] JS：解构默认值
来源：http://read.share.zdbjq.cn/Article/details/gbbkoqsrk.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.share.zdbjq.cn/Article/details/gyvnuidvf.sHtML

[U88] JS：对象展开合并
来源：http://3g.fehbvm.com/Article/details/gtrqvdcxu.sHtML

{ ...a, ...b }
来源：http://www.m.share.zdbjq.cn/Article/details/gxqbmjcsd.sHtML

[U89] JS：数组去重
来源：http://baike.hesvh.cn/Article/details/glxtefdrj.sHtML

[...new Set(arr)]
来源：http://wap.zdbjq.cn/Article/details/ggocowtid.sHtML

[U90] JS：数字数组排序
来源：http://www.blog.hesvh.cn/Article/details/ghlauafab.sHtML

[...arr].sort((a, b) => a - b)
来源：http://mobile.zdbjq.cn/Article/details/grzbxbeid.sHtML

[U91] JS：对象键值遍历
来源：http://baike.hesvh.cn/Article/details/gbbphowla.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://baike.hesvh.cn/Article/details/gmshjvucu.sHtML

[U92] JS：深拷贝
来源：http://baike.fehbvm.com/Article/details/gzygndncw.sHtML

structuredClone(obj)
来源：http://baike.zdbjq.cn/Article/details/gzzxgwgyi.sHtML

[U93] JS：模板字符串
来源：http://www.m.share.fehbvm.com/Article/details/glqdedhcj.sHtML

`共 ${n} 条`
来源：http://mobile.zdbjq.cn/Article/details/gwnviupdl.sHtML

[U94] JS：箭头函数
来源：http://www.m.share.hesvh.cn/Article/details/gfwgatqvw.sHtML

const double = x => x * 2;
来源：http://www.share.zdbjq.cn/Article/details/gidsixesx.sHtML

[U95] JS：Promise 包装
来源：http://m.share.hesvh.cn/Article/details/grxglmpem.sHtML

new Promise((resolve, reject) => {})
来源：http://read.share.hesvh.cn/Article/details/gzhwgdxlc.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.zdbjq.cn/Article/details/giwzmichk.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://blog.zdbjq.cn/Article/details/gqokslnrk.sHtML

[U97] JS：并发请求
来源：http://wap.zdbjq.cn/Article/details/gitkvycdb.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.zdbjq.cn/Article/details/geiklyrfo.sHtML

[U98] JS：fetch 带 JSON
来源：http://mobile.fehbvm.com/Article/details/ghxbqjxlg.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://baike.hesvh.cn/Article/details/giksrolzy.sHtML

[U99] JS：事件监听
来源：http://wap.zdbjq.cn/Article/details/gnjjdxgpe.sHtML

el.addEventListener("click", e => {})
来源：http://baike.zdbjq.cn/Article/details/gpuvsinqq.sHtML

[U100] JS：DOM 查询
来源：http://www.share.zdbjq.cn/Article/details/gjrsknztb.sHtML

document.querySelector(".item")
来源：http://baike.fehbvm.com/Article/details/gdaeqpcmu.sHtML

[U101] JS：classList 操作
来源：http://blog.fehbvm.com/Article/details/ginkajahd.sHtML

el.classList.toggle("active")
来源：http://baike.hesvh.cn/Article/details/gdnxskwip.sHtML

[U102] JS：本地存储
来源：http://blog.fehbvm.com/Article/details/gsbbpekjw.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://baike.hesvh.cn/Article/details/ghvshhyed.sHtML

[U103] JS：定时器
来源：http://blog.fehbvm.com/Article/details/gcpibozlb.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.fehbvm.com/Article/details/gqvdjvsti.sHtML

[U104] JS：防抖
来源：http://www.share.hesvh.cn/Article/details/gveabjbbd.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.zdbjq.cn/Article/details/gmjsclzpu.sHtML

[U105] JS：节流
来源：http://blog.zdbjq.cn/Article/details/godgsbzoq.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://blog.fehbvm.com/Article/details/gsxfsgbsh.sHtML

[U106] JS：日期格式化
来源：http://blog.fehbvm.com/Article/details/ggivazrot.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.hesvh.cn/Article/details/gcvinjawv.sHtML

[U107] JS：数字千分位
来源：http://www.blog.fehbvm.com/Article/details/gpnznbtko.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://baike.fehbvm.com/Article/details/getpregip.sHtML

[U108] JS：随机整数
来源：http://3g.zdbjq.cn/Article/details/gcdgwxzhe.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://blog.zdbjq.cn/Article/details/gfnirugkf.sHtML

[U109] JS：数组分组
来源：http://www.share.hesvh.cn/Article/details/gnmvyaute.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.m.share.hesvh.cn/Article/details/gqnkvaujb.sHtML

[U110] JS：数组分块
来源：http://blog.zdbjq.cn/Article/details/geqjbsksa.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.hesvh.cn/Article/details/gvntlqvbp.sHtML

[U111] JS：对象转 Map
来源：http://3g.fehbvm.com/Article/details/gaolivtad.sHtML

new Map(Object.entries(obj))
来源：http://read.share.hesvh.cn/Article/details/gqepoahbk.sHtML

[U112] JS：字符串补位
来源：http://baike.zdbjq.cn/Article/details/gaheehqqe.sHtML

"7".padStart(3, "0")
来源：http://www.blog.hesvh.cn/Article/details/gvvawylbk.sHtML

[U113] JS：正则替换全部
来源：http://m.share.zdbjq.cn/Article/details/gyqwtirgb.sHtML

s.replaceAll("a", "b")
来源：http://blog.fehbvm.com/Article/details/gcxpnmsvz.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.hesvh.cn/Article/details/gfvddcdri.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.hesvh.cn/Article/details/gdhjergic.sHtML

[U115] JS：生成 UUID
来源：http://baike.fehbvm.com/Article/details/gzzzatjup.sHtML

crypto.randomUUID()
来源：http://mobile.fehbvm.com/Article/details/gapaauzjq.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.hesvh.cn/Article/details/gwsrkaham.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.zdbjq.cn/Article/details/gdxvodidx.sHtML

[U117] JS：单元测试
来源：http://wap.hesvh.cn/Article/details/gwwqzsxso.sHtML

npm i -D vitest;  npx vitest
来源：http://blog.fehbvm.com/Article/details/gdbwoidjv.sHtML

[U118] JS：开发服务器
来源：http://wap.zdbjq.cn/Article/details/gvtfugmoe.sHtML

npm i -D vite;  npx vite
来源：http://read.share.hesvh.cn/Article/details/gyeazmhfl.sHtML

[U119] JS：生产构建
来源：http://blog.fehbvm.com/Article/details/gdhvmbxkd.sHtML

npx vite build
来源：http://wap.fehbvm.com/Article/details/gmobsgtby.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.zdbjq.cn/Article/details/gerkfjmov.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.zdbjq.cn/Article/details/gsvnsjrbv.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gpelmftqi.sHtML

统计汇总
来源：http://blog.hesvh.cn/Article/details/gczzqykhm.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gagziifaa.sHtML

按语言统计（条）：
来源：http://www.m.share.fehbvm.com/Article/details/gpuvxecwe.sHtML

Python ......... 252
来源：http://www.m.share.fehbvm.com/Article/details/gpoqvvzqr.sHtML

PHP ............ 252
来源：http://3g.fehbvm.com/Article/details/goyebrvgq.sHtML

JavaScript ..... 252
来源：http://read.share.zdbjq.cn/Article/details/gjxjmwljg.sHtML

TypeScript ..... 212
来源：http://mobile.zdbjq.cn/Article/details/gqhnodmnt.sHtML

Java ........... 212
来源：http://www.blog.hesvh.cn/Article/details/giqiabmtw.sHtML

Go ............. 212
来源：http://wap.fehbvm.com/Article/details/gqgaxtyur.sHtML

Ruby ........... 212
来源：http://read.share.fehbvm.com/Article/details/gulcqrnyg.sHtML

C# ............. 212
来源：http://m.share.fehbvm.com/Article/details/givckfuva.sHtML

C .............. 30
来源：http://m.share.hesvh.cn/Article/details/gwmxvulnr.sHtML

C++ ............ 30
来源：http://3g.zdbjq.cn/Article/details/gmsgpmdar.sHtML

SQL ............ 90
来源：http://www.m.share.zdbjq.cn/Article/details/gmygpkrbm.sHtML

Bash ........... 80
来源：http://baike.hesvh.cn/Article/details/godugdydr.sHtML

Kotlin ......... 15
来源：http://www.share.fehbvm.com/Article/details/gxjnhhptx.sHtML

Swift .......... 15
来源：http://blog.hesvh.cn/Article/details/gztvozwqg.sHtML

Lua ............ 10
来源：http://3g.fehbvm.com/Article/details/gtbljnuwj.sHtML

Perl ........... 10
来源：http://mobile.fehbvm.com/Article/details/ghsdvlqfk.sHtML

Scala .......... 10
来源：http://mobile.hesvh.cn/Article/details/gvlhfmief.sHtML

------------------------------------
来源：http://3g.fehbvm.com/Article/details/gtldyncnv.sHtML

合计 ........... 2106 条
来源：http://m.share.hesvh.cn/Article/details/gmnorwetx.sHtML

按章节统计：
来源：http://read.share.zdbjq.cn/Article/details/gwmjvewqh.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.fehbvm.com/Article/details/gnwjmcywl.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://m.share.hesvh.cn/Article/details/gjnozliyp.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://3g.fehbvm.com/Article/details/gkicqhvbc.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://read.share.fehbvm.com/Article/details/gmzvrfhtn.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.m.share.fehbvm.com/Article/details/gdztqsygy.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.m.share.fehbvm.com/Article/details/ghmaitptb.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://baike.zdbjq.cn/Article/details/gpweoscfq.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://blog.fehbvm.com/Article/details/gjckiprzr.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://baike.zdbjq.cn/Article/details/guxwslfbr.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wap.fehbvm.com/Article/details/gsoktrooe.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.share.fehbvm.com/Article/details/gdfnpegmo.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://read.share.hesvh.cn/Article/details/gbneddkin.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://3g.hesvh.cn/Article/details/gtxemgfpy.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://read.share.zdbjq.cn/Article/details/guhuzbori.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.share.fehbvm.com/Article/details/gtospdevg.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://read.share.zdbjq.cn/Article/details/gipvymwiu.sHtML

Q SQL 专题                              90
来源：http://wap.fehbvm.com/Article/details/gzgwmmaev.sHtML

R Bash 专题                             80
来源：http://www.share.fehbvm.com/Article/details/gbjdbolim.sHtML

S C / C++ 专题                          60
来源：http://wap.zdbjq.cn/Article/details/gkvpsdlxq.sHtML

T 其他语言补充                          60
来源：http://3g.hesvh.cn/Article/details/gcgmgjnxx.sHtML

U 高频实用片段                         120
来源：http://m.share.hesvh.cn/Article/details/gkrojxtfu.sHtML

------------------------------------
来源：http://www.m.share.hesvh.cn/Article/details/gqxgenxpm.sHtML

合计                                  2106 条
来源：http://www.m.share.fehbvm.com/Article/details/gkdkckjov.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.zdbjq.cn/Article/details/gqpignenm.sHtML

使用提醒
来源：http://www.share.hesvh.cn/Article/details/gntmcazbg.sHtML

--------------------------------------------------------------------------------
来源：http://wap.zdbjq.cn/Article/details/glmcedzgx.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://m.share.hesvh.cn/Article/details/gspvpclhq.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.m.share.fehbvm.com/Article/details/gpwtwalpo.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://blog.hesvh.cn/Article/details/gbroiyujp.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://blog.zdbjq.cn/Article/details/gbnovpiaw.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://read.share.zdbjq.cn/Article/details/garuwwfqh.sHtML

—— 文件结束 ——
来源：http://mobile.zdbjq.cn/Article/details/gfgriqfjf.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gzkwsmdij.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.share.hesvh.cn/Article/details/ganhkwymz.sHtML

Common Programming Examples Cheat Book
来源：http://m.share.hesvh.cn/Article/details/gbppyrhvk.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gzjkcfvfo.sHtML

【收录内容】
来源：http://www.share.hesvh.cn/Article/details/gkdpysmes.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://wap.zdbjq.cn/Article/details/gabcsptia.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.m.share.fehbvm.com/Article/details/gfggkqkuh.sHtML

SQL · Bash · C · C++
来源：http://blog.fehbvm.com/Article/details/gsnrjrayj.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.share.hesvh.cn/Article/details/gihbphrhx.sHtML

【使用说明】
来源：http://blog.zdbjq.cn/Article/details/gpvmjeeeg.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://m.share.hesvh.cn/Article/details/gvkilzrdj.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.share.zdbjq.cn/Article/details/gwusnzpes.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.blog.zdbjq.cn/Article/details/grotbstge.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://m.share.zdbjq.cn/Article/details/gbzvjjrxf.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://blog.hesvh.cn/Article/details/gtpalxuvo.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://m.share.hesvh.cn/Article/details/gcpghlnsb.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://baike.hesvh.cn/Article/details/gnttcjqdp.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://blog.hesvh.cn/Article/details/gkbflwkxg.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://read.share.fehbvm.com/Article/details/gthvcudib.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.blog.hesvh.cn/Article/details/gbegdycil.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.blog.hesvh.cn/Article/details/garsqvdqa.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://blog.zdbjq.cn/Article/details/gslfmnmsb.sHtML

【文件统计】
来源：http://baike.hesvh.cn/Article/details/gqxgudyjt.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://read.share.fehbvm.com/Article/details/gtikhffnu.sHtML

--------------------------------------------------------------------------------
来源：http://baike.hesvh.cn/Article/details/godmbueqm.sHtML

目  录
来源：http://mobile.hesvh.cn/Article/details/gfmvhbdpk.sHtML

--------------------------------------------------------------------------------
来源：http://blog.fehbvm.com/Article/details/ginhdkavc.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.blog.zdbjq.cn/Article/details/gkbwqsgia.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://wap.hesvh.cn/Article/details/gdutuhkpm.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://3g.zdbjq.cn/Article/details/gexejgsat.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://blog.hesvh.cn/Article/details/gzqpnryir.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://baike.fehbvm.com/Article/details/giimdxquv.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://mobile.fehbvm.com/Article/details/gubyxergn.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://wap.hesvh.cn/Article/details/gkrqsfijb.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://blog.fehbvm.com/Article/details/glofafqqs.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://baike.fehbvm.com/Article/details/gawzrgmqv.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://read.share.hesvh.cn/Article/details/ggibquzdg.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://mobile.fehbvm.com/Article/details/gpjyqfaen.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://m.share.fehbvm.com/Article/details/geffnkjst.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://blog.fehbvm.com/Article/details/guyyrtrsq.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.m.share.hesvh.cn/Article/details/ggakxfkqr.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://m.share.hesvh.cn/Article/details/gaundgqge.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://baike.fehbvm.com/Article/details/goiayhanb.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://read.share.fehbvm.com/Article/details/gtvqwoslb.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://blog.hesvh.cn/Article/details/gqugkiyby.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://read.share.fehbvm.com/Article/details/glnwfmism.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.zdbjq.cn/Article/details/gmxnmjwcr.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.share.zdbjq.cn/Article/details/gnyedosse.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/grigvmvlj.sHtML

A. 基础语法与类型
来源：http://mobile.zdbjq.cn/Article/details/gittvrwqc.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gucevsqcj.sHtML

[A01] Hello World
来源：http://baike.fehbvm.com/Article/details/gurugmwqr.sHtML

Py:   print("Hello, World!")
来源：http://read.share.fehbvm.com/Article/details/gswzbxoje.sHtML

PHP:  echo "Hello, World!";
来源：http://3g.hesvh.cn/Article/details/gkresiyey.sHtML

JS:   console.log("Hello, World!");
来源：http://blog.hesvh.cn/Article/details/gnbgnftao.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://blog.hesvh.cn/Article/details/gmemiejrb.sHtML

Java: System.out.println("Hello, World!");
来源：http://blog.hesvh.cn/Article/details/gkcqbtqgw.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://3g.fehbvm.com/Article/details/gkvxebmde.sHtML

Ruby: puts "Hello, World!"
来源：http://www.m.share.hesvh.cn/Article/details/gwnygurdc.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://read.share.fehbvm.com/Article/details/gvesjqpea.sHtML

[A02] 变量声明与赋值
来源：http://baike.zdbjq.cn/Article/details/gxomyujsw.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://read.share.fehbvm.com/Article/details/geohxzoum.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.m.share.zdbjq.cn/Article/details/gmwuqkvwo.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.m.share.hesvh.cn/Article/details/gatzbanuq.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://read.share.fehbvm.com/Article/details/gsakyzwhl.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://baike.fehbvm.com/Article/details/gcduzneyd.sHtML

Go:   name := "Alex"; age := 20
来源：http://wap.zdbjq.cn/Article/details/gihbuwfgo.sHtML

Ruby: name = "Alex"; age = 20
来源：http://wap.hesvh.cn/Article/details/gzbwdinqx.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://mobile.fehbvm.com/Article/details/gxbtspoil.sHtML

[A03] 常量定义
来源：http://m.share.zdbjq.cn/Article/details/gddlzcarx.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.share.zdbjq.cn/Article/details/gyvbyccrl.sHtML

PHP:  const PI = 3.14159;
来源：http://read.share.fehbvm.com/Article/details/gdhyeizqg.sHtML

JS:   const PI = 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gwvpoiksv.sHtML

TS:   const PI: number = 3.14159;
来源：http://baike.zdbjq.cn/Article/details/ggckqaabt.sHtML

Java: static final double PI = 3.14159;
来源：http://baike.hesvh.cn/Article/details/gjsrrpgqw.sHtML

Go:   const PI = 3.14159
来源：http://baike.fehbvm.com/Article/details/ggkvrifij.sHtML

Ruby: PI = 3.14159
来源：http://blog.fehbvm.com/Article/details/gyhspqamh.sHtML

C#:   const double PI = 3.14159;
来源：http://baike.hesvh.cn/Article/details/ggpwloqdw.sHtML

[A04] 判断变量类型
来源：http://baike.hesvh.cn/Article/details/gycnqohjj.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.m.share.hesvh.cn/Article/details/gnulopcro.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://m.share.hesvh.cn/Article/details/gighhuehn.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.m.share.fehbvm.com/Article/details/gtfyqxuci.sHtML

TS:   typeof x; x instanceof Date
来源：http://baike.hesvh.cn/Article/details/gykwtyoxl.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://wap.hesvh.cn/Article/details/gnicqrbei.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.blog.fehbvm.com/Article/details/gqubyrkqp.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.m.share.zdbjq.cn/Article/details/gteytznru.sHtML

C#:   x.GetType().Name; x is int
来源：http://read.share.zdbjq.cn/Article/details/gedzqhokw.sHtML

[A05] 整数除法与取模
来源：http://3g.hesvh.cn/Article/details/gfcjixlpl.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.blog.zdbjq.cn/Article/details/gykkdhqcl.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://read.share.fehbvm.com/Article/details/gpdjsyoar.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.fehbvm.com/Article/details/gkfxjkdhu.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://mobile.zdbjq.cn/Article/details/gvfzpbsuk.sHtML

Java: 7 / 2; 7 % 2
来源：http://3g.hesvh.cn/Article/details/gvmkxkrii.sHtML

Go:   7 / 2; 7 % 2
来源：http://read.share.hesvh.cn/Article/details/gillwhgdq.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://blog.zdbjq.cn/Article/details/gvvqmdazb.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.blog.fehbvm.com/Article/details/gsrzgsrzl.sHtML

[A06] 字符串转数字
来源：http://www.share.fehbvm.com/Article/details/guciibxji.sHtML

Py:   int("42"); float("3.14")
来源：http://3g.hesvh.cn/Article/details/grlhsbqlz.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://blog.zdbjq.cn/Article/details/gwdkpqzwc.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://3g.zdbjq.cn/Article/details/goecwufxb.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.blog.hesvh.cn/Article/details/gyekcyapv.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.blog.fehbvm.com/Article/details/gabophuqq.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.m.share.zdbjq.cn/Article/details/giofxklsa.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://baike.fehbvm.com/Article/details/gacuesouo.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://baike.hesvh.cn/Article/details/gzzviiaww.sHtML

[A07] 数字转字符串
来源：http://3g.zdbjq.cn/Article/details/gqjqtrevc.sHtML

Py:   str(42)
来源：http://3g.fehbvm.com/Article/details/gnuvjbkqu.sHtML

PHP:  (string) 42; strval(42)
来源：http://baike.fehbvm.com/Article/details/gpvuopmis.sHtML

JS:   String(42); (42).toString()
来源：http://3g.zdbjq.cn/Article/details/gpnoafpcp.sHtML

TS:   String(42)
来源：http://www.share.hesvh.cn/Article/details/gddfdzckp.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://m.share.hesvh.cn/Article/details/gzyhfhkvf.sHtML

Go:   strconv.Itoa(42)
来源：http://mobile.zdbjq.cn/Article/details/gktdvvwsc.sHtML

Ruby: 42.to_s
来源：http://www.m.share.fehbvm.com/Article/details/grabcgshb.sHtML

C#:   42.ToString()
来源：http://3g.fehbvm.com/Article/details/giicrwqul.sHtML

[A08] 取整与四舍五入
来源：http://www.m.share.fehbvm.com/Article/details/gmovtxpga.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://wap.hesvh.cn/Article/details/gecrvudlj.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.m.share.hesvh.cn/Article/details/gucbiwugv.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.m.share.hesvh.cn/Article/details/goaadpwme.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://m.share.fehbvm.com/Article/details/galyyfxpr.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://wap.hesvh.cn/Article/details/gtjzvroqi.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://blog.zdbjq.cn/Article/details/gupokznqe.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://mobile.hesvh.cn/Article/details/gbynyztbw.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://m.share.zdbjq.cn/Article/details/gcpliosqm.sHtML

[A09] 绝对值与最大最小值
来源：http://www.share.hesvh.cn/Article/details/gvdxhxulu.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gtvcriyjw.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gyvclwqgz.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://m.share.zdbjq.cn/Article/details/ghcccocwt.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://blog.hesvh.cn/Article/details/gugzlutbs.sHtML


<!-- 参考信息 -->