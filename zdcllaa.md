代发 wailian999

[U63] PHP：文件读写
来源：http://www.share.hesvh.cn/Article/details/grgpvouac.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.hesvh.cn/Article/details/gtppgfdiz.sHtML

[U64] PHP：目录遍历
来源：http://3g.zdbjq.cn/Article/details/gkgoindlz.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://3g.fehbvm.com/Article/details/ggczodiyf.sHtML

[U65] PHP：会话
来源：http://mobile.fehbvm.com/Article/details/gudyflqvz.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://m.share.zdbjq.cn/Article/details/ghgnxbzik.sHtML

[U66] PHP：设置 Cookie
来源：http://mobile.zdbjq.cn/Article/details/gyrrelxbo.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://m.share.zdbjq.cn/Article/details/gehvklhdl.sHtML

[U67] PHP：处理文件上传
来源：http://m.share.fehbvm.com/Article/details/gyuugqqfp.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.m.share.zdbjq.cn/Article/details/gglyjiqcp.sHtML

[U68] PHP：PDO 连接
来源：http://wap.zdbjq.cn/Article/details/gqmmederk.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://m.share.fehbvm.com/Article/details/gcnwznlwj.sHtML

[U69] PHP：PDO 预处理
来源：http://3g.fehbvm.com/Article/details/gokeijiax.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.fehbvm.com/Article/details/gyrswlowz.sHtML

[U70] PHP：PDO 事务
来源：http://mobile.zdbjq.cn/Article/details/gqjhpgwkc.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://3g.fehbvm.com/Article/details/gbzfusspn.sHtML

[U71] PHP：抛出异常
来源：http://www.blog.zdbjq.cn/Article/details/gncoczvft.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.share.zdbjq.cn/Article/details/ghfdnlife.sHtML

[U72] PHP：写错误日志
来源：http://mobile.hesvh.cn/Article/details/gymtupdes.sHtML

error_log("失败: " . $e->getMessage());
来源：http://3g.zdbjq.cn/Article/details/glzrbiyve.sHtML

[U73] PHP：读取 ini 配置
来源：http://read.share.zdbjq.cn/Article/details/guobgwgnv.sHtML

parse_ini_file("config.ini", true)
来源：http://blog.hesvh.cn/Article/details/gjniqergz.sHtML

[U74] PHP：读取环境变量
来源：http://m.share.fehbvm.com/Article/details/gsjkusyty.sHtML

getenv("APP_ENV") ?: "production"
来源：http://baike.zdbjq.cn/Article/details/gdsigmqoc.sHtML

[U75] PHP：依赖注入
来源：http://baike.zdbjq.cn/Article/details/ghnuvqxiq.sHtML

composer require psr/container
来源：http://baike.fehbvm.com/Article/details/gyookkvrx.sHtML

[U76] PHP：简单路由
来源：http://blog.hesvh.cn/Article/details/gfukpwniz.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wap.fehbvm.com/Article/details/gfwneunof.sHtML

[U77] PHP：模板渲染
来源：http://www.m.share.hesvh.cn/Article/details/gaoodroww.sHtML

composer require twig/twig
来源：http://mobile.zdbjq.cn/Article/details/galtgvane.sHtML

[U78] PHP：单元测试
来源：http://m.share.fehbvm.com/Article/details/gzoelehpq.sHtML

composer require --dev phpunit/phpunit
来源：http://3g.hesvh.cn/Article/details/gphhhguhe.sHtML

[U79] PHP：静态分析
来源：http://mobile.zdbjq.cn/Article/details/ghougkmxh.sHtML

composer require --dev phpstan/phpstan
来源：http://m.share.fehbvm.com/Article/details/govxxwjtd.sHtML

[U80] PHP：代码规范修复
来源：http://mobile.fehbvm.com/Article/details/gathltnjc.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://m.share.fehbvm.com/Article/details/gdrxsfaua.sHtML

[U81] JS：初始化项目
来源：http://3g.hesvh.cn/Article/details/ghyziarrc.sHtML

npm init -y;  npm i express
来源：http://www.share.fehbvm.com/Article/details/gpwsyxkxi.sHtML

[U82] JS：package.json 脚本
来源：http://baike.hesvh.cn/Article/details/ggiaxjaom.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mobile.fehbvm.com/Article/details/gecynxtbd.sHtML

[U83] JS：ES Module 导入导出
来源：http://read.share.hesvh.cn/Article/details/gqrjpmmoc.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://3g.hesvh.cn/Article/details/gyjikmchc.sHtML

[U84] JS：CommonJS 写法
来源：http://read.share.hesvh.cn/Article/details/gybflkltt.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://3g.zdbjq.cn/Article/details/guzjvpvqv.sHtML

[U85] JS：可选链
来源：http://www.blog.fehbvm.com/Article/details/gftpoilxd.sHtML

a?.b?.c
来源：http://mobile.fehbvm.com/Article/details/gbpxkkqnt.sHtML

[U86] JS：空值合并
来源：http://www.blog.zdbjq.cn/Article/details/gsofmnldh.sHtML

a ?? b
来源：http://www.blog.hesvh.cn/Article/details/gtawztbmu.sHtML

[U87] JS：解构默认值
来源：http://www.share.zdbjq.cn/Article/details/ghomlebpp.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.hesvh.cn/Article/details/gsbgzvqpc.sHtML

[U88] JS：对象展开合并
来源：http://www.blog.fehbvm.com/Article/details/gfarpgkee.sHtML

{ ...a, ...b }
来源：http://mobile.zdbjq.cn/Article/details/gluncrpgn.sHtML

[U89] JS：数组去重
来源：http://mobile.zdbjq.cn/Article/details/gididgbkg.sHtML

[...new Set(arr)]
来源：http://3g.fehbvm.com/Article/details/gtptnnete.sHtML

[U90] JS：数字数组排序
来源：http://m.share.fehbvm.com/Article/details/gthotytsw.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.m.share.hesvh.cn/Article/details/geyjnkddi.sHtML

[U91] JS：对象键值遍历
来源：http://www.m.share.hesvh.cn/Article/details/gwxsfxoxl.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.blog.zdbjq.cn/Article/details/ggwxhxnue.sHtML

[U92] JS：深拷贝
来源：http://m.share.zdbjq.cn/Article/details/glevkdsef.sHtML

structuredClone(obj)
来源：http://baike.zdbjq.cn/Article/details/gjnotlsuh.sHtML

[U93] JS：模板字符串
来源：http://baike.zdbjq.cn/Article/details/ggyqrqvpq.sHtML

`共 ${n} 条`
来源：http://blog.zdbjq.cn/Article/details/gppedjbta.sHtML

[U94] JS：箭头函数
来源：http://www.m.share.fehbvm.com/Article/details/gxmzynfjm.sHtML

const double = x => x * 2;
来源：http://m.share.hesvh.cn/Article/details/gsqysakwc.sHtML

[U95] JS：Promise 包装
来源：http://baike.zdbjq.cn/Article/details/gdzfnyobv.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.fehbvm.com/Article/details/glnngljdx.sHtML

[U96] JS：async/await 与异常
来源：http://www.m.share.zdbjq.cn/Article/details/giaqfpbaf.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wap.fehbvm.com/Article/details/gersfhrvb.sHtML

[U97] JS：并发请求
来源：http://blog.fehbvm.com/Article/details/ggzndxytu.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.fehbvm.com/Article/details/gpzhbbuos.sHtML

[U98] JS：fetch 带 JSON
来源：http://blog.zdbjq.cn/Article/details/gidksvmxa.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wap.fehbvm.com/Article/details/ghkzhzhho.sHtML

[U99] JS：事件监听
来源：http://m.share.hesvh.cn/Article/details/gnvxyzabq.sHtML

el.addEventListener("click", e => {})
来源：http://baike.fehbvm.com/Article/details/gxshbitxa.sHtML

[U100] JS：DOM 查询
来源：http://m.share.zdbjq.cn/Article/details/gsofsqdgu.sHtML

document.querySelector(".item")
来源：http://mobile.zdbjq.cn/Article/details/gxsawoulz.sHtML

[U101] JS：classList 操作
来源：http://www.share.hesvh.cn/Article/details/gtzxxoibc.sHtML

el.classList.toggle("active")
来源：http://www.m.share.zdbjq.cn/Article/details/gwfkckyvl.sHtML

[U102] JS：本地存储
来源：http://read.share.fehbvm.com/Article/details/giwujcsok.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.blog.zdbjq.cn/Article/details/ghmffhjxr.sHtML

[U103] JS：定时器
来源：http://blog.fehbvm.com/Article/details/gubvuucpi.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://m.share.fehbvm.com/Article/details/gtzttatzy.sHtML

[U104] JS：防抖
来源：http://m.share.hesvh.cn/Article/details/giimdakhu.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fehbvm.com/Article/details/gqmlpolvy.sHtML

[U105] JS：节流
来源：http://www.m.share.zdbjq.cn/Article/details/gydsnwdew.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.share.fehbvm.com/Article/details/gncxognxq.sHtML

[U106] JS：日期格式化
来源：http://www.m.share.fehbvm.com/Article/details/glekjlsti.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.blog.fehbvm.com/Article/details/gadctykih.sHtML

[U107] JS：数字千分位
来源：http://3g.fehbvm.com/Article/details/gduiatvmz.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.blog.zdbjq.cn/Article/details/gajoukqpx.sHtML

[U108] JS：随机整数
来源：http://baike.fehbvm.com/Article/details/gxezcyucu.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://m.share.hesvh.cn/Article/details/gkoutjcef.sHtML

[U109] JS：数组分组
来源：http://read.share.fehbvm.com/Article/details/gkynzudzt.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.fehbvm.com/Article/details/gfkcvyetl.sHtML

[U110] JS：数组分块
来源：http://blog.fehbvm.com/Article/details/gqycslkey.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.share.hesvh.cn/Article/details/gfciforsq.sHtML

[U111] JS：对象转 Map
来源：http://wap.fehbvm.com/Article/details/gulxkqqgl.sHtML

new Map(Object.entries(obj))
来源：http://read.share.fehbvm.com/Article/details/gojydotgk.sHtML

[U112] JS：字符串补位
来源：http://www.m.share.zdbjq.cn/Article/details/gxdyjjgdq.sHtML

"7".padStart(3, "0")
来源：http://www.share.hesvh.cn/Article/details/gxainjxhh.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.hesvh.cn/Article/details/gftzstiik.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gdxnyhgty.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.fehbvm.com/Article/details/gkjjltcdm.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.hesvh.cn/Article/details/gkwsjvltt.sHtML

[U115] JS：生成 UUID
来源：http://mobile.fehbvm.com/Article/details/gzkynkzbu.sHtML

crypto.randomUUID()
来源：http://www.share.hesvh.cn/Article/details/gweoowjdn.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://wap.zdbjq.cn/Article/details/guzywcawj.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.hesvh.cn/Article/details/gvlbzkquc.sHtML

[U117] JS：单元测试
来源：http://baike.fehbvm.com/Article/details/glmveztge.sHtML

npm i -D vitest;  npx vitest
来源：http://wap.fehbvm.com/Article/details/gsanegpnj.sHtML

[U118] JS：开发服务器
来源：http://baike.hesvh.cn/Article/details/ggluleoyu.sHtML

npm i -D vite;  npx vite
来源：http://read.share.zdbjq.cn/Article/details/gfsfntjpu.sHtML

[U119] JS：生产构建
来源：http://read.share.fehbvm.com/Article/details/gheewltth.sHtML

npx vite build
来源：http://www.share.hesvh.cn/Article/details/ghbcsazdb.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.share.hesvh.cn/Article/details/giageqwku.sHtML

import.meta.env.VITE_API_URL
来源：http://read.share.hesvh.cn/Article/details/gocutbrrt.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gcagcysfm.sHtML

统计汇总
来源：http://mobile.hesvh.cn/Article/details/gxlpdaafw.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gkcvcwekm.sHtML

按语言统计（条）：
来源：http://wap.zdbjq.cn/Article/details/gxivqeepf.sHtML

Python ......... 252
来源：http://mobile.hesvh.cn/Article/details/gmrkekdff.sHtML

PHP ............ 252
来源：http://blog.zdbjq.cn/Article/details/gjiihovwl.sHtML

JavaScript ..... 252
来源：http://mobile.hesvh.cn/Article/details/gemtvrhkt.sHtML

TypeScript ..... 212
来源：http://read.share.hesvh.cn/Article/details/gatszepww.sHtML

Java ........... 212
来源：http://m.share.zdbjq.cn/Article/details/gbsyaeton.sHtML

Go ............. 212
来源：http://baike.hesvh.cn/Article/details/gvfychhks.sHtML

Ruby ........... 212
来源：http://www.share.fehbvm.com/Article/details/gwnjiurco.sHtML

C# ............. 212
来源：http://www.m.share.zdbjq.cn/Article/details/gspnykics.sHtML

C .............. 30
来源：http://mobile.zdbjq.cn/Article/details/gztgiqxsp.sHtML

C++ ............ 30
来源：http://www.m.share.hesvh.cn/Article/details/gdsimtcef.sHtML

SQL ............ 90
来源：http://www.m.share.hesvh.cn/Article/details/geimgepcq.sHtML

Bash ........... 80
来源：http://www.m.share.fehbvm.com/Article/details/gfggvrgft.sHtML

Kotlin ......... 15
来源：http://m.share.hesvh.cn/Article/details/gqqgifsvy.sHtML

Swift .......... 15
来源：http://mobile.fehbvm.com/Article/details/gfcejnwxm.sHtML

Lua ............ 10
来源：http://baike.zdbjq.cn/Article/details/glatvjxet.sHtML

Perl ........... 10
来源：http://www.m.share.hesvh.cn/Article/details/gffdlpsbx.sHtML

Scala .......... 10
来源：http://read.share.hesvh.cn/Article/details/gaglvjrrv.sHtML

------------------------------------
来源：http://blog.hesvh.cn/Article/details/geuthexbl.sHtML

合计 ........... 2106 条
来源：http://www.blog.hesvh.cn/Article/details/gorjvuvam.sHtML

按章节统计：
来源：http://mobile.zdbjq.cn/Article/details/gjtbvlxnr.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://baike.hesvh.cn/Article/details/gswvofcrv.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.share.fehbvm.com/Article/details/gjeudubpw.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://3g.fehbvm.com/Article/details/gxnmksgmj.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://m.share.fehbvm.com/Article/details/gtebourtk.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://baike.zdbjq.cn/Article/details/gmdqfcpvd.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://read.share.zdbjq.cn/Article/details/gmkswejpo.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.share.fehbvm.com/Article/details/gyegrbrbf.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mobile.fehbvm.com/Article/details/gxkiwdlqv.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://3g.fehbvm.com/Article/details/goviicbjc.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://m.share.fehbvm.com/Article/details/gmbamipya.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://3g.zdbjq.cn/Article/details/gecllehwx.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.m.share.fehbvm.com/Article/details/gexszuqnc.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.m.share.zdbjq.cn/Article/details/gssgvndko.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.blog.fehbvm.com/Article/details/gkotxocrn.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.share.zdbjq.cn/Article/details/ghlhhwuom.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.m.share.hesvh.cn/Article/details/gzlxaanzc.sHtML

Q SQL 专题                              90
来源：http://blog.hesvh.cn/Article/details/ghqtdvepf.sHtML

R Bash 专题                             80
来源：http://www.share.zdbjq.cn/Article/details/gcaetoqix.sHtML

S C / C++ 专题                          60
来源：http://wap.hesvh.cn/Article/details/gamxcnblp.sHtML

T 其他语言补充                          60
来源：http://www.share.hesvh.cn/Article/details/gzcxmwnla.sHtML

U 高频实用片段                         120
来源：http://3g.zdbjq.cn/Article/details/gyyiwqwus.sHtML

------------------------------------
来源：http://wap.fehbvm.com/Article/details/ghdiayxdh.sHtML

合计                                  2106 条
来源：http://www.m.share.zdbjq.cn/Article/details/gqfifmtsh.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/gpitmspsw.sHtML

使用提醒
来源：http://mobile.hesvh.cn/Article/details/gbdzlwidj.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.zdbjq.cn/Article/details/gjkwjnmhs.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://m.share.zdbjq.cn/Article/details/gwcknrtcm.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mobile.hesvh.cn/Article/details/gsicuumam.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://read.share.hesvh.cn/Article/details/grqzbzklq.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://m.share.fehbvm.com/Article/details/gnfhkcprq.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wap.hesvh.cn/Article/details/gbaqbxvhy.sHtML

—— 文件结束 ——
来源：http://www.m.share.zdbjq.cn/Article/details/gpxrlqlnz.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/geevdgxhk.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://read.share.zdbjq.cn/Article/details/gawnrzqad.sHtML

Common Programming Examples Cheat Book
来源：http://read.share.zdbjq.cn/Article/details/gunvfeept.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/geynkhzlb.sHtML

【收录内容】
来源：http://wap.fehbvm.com/Article/details/gzbtrartb.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.share.hesvh.cn/Article/details/gepxelshi.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://baike.hesvh.cn/Article/details/getvfwzlx.sHtML

SQL · Bash · C · C++
来源：http://read.share.fehbvm.com/Article/details/gyujyyrsf.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://mobile.fehbvm.com/Article/details/gagyqjqei.sHtML

【使用说明】
来源：http://blog.fehbvm.com/Article/details/guoirsadu.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://blog.zdbjq.cn/Article/details/gozrrxbnr.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.blog.hesvh.cn/Article/details/gpwymbsbh.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://blog.zdbjq.cn/Article/details/gjnzwemuq.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.m.share.fehbvm.com/Article/details/gylnpmppm.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://read.share.zdbjq.cn/Article/details/gwoknkjxd.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wap.zdbjq.cn/Article/details/gfeajarpi.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wap.fehbvm.com/Article/details/gfsyhrxxl.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://baike.hesvh.cn/Article/details/gjiadxfjc.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.m.share.hesvh.cn/Article/details/guxcjhnpu.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://wap.zdbjq.cn/Article/details/gaglxubdf.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://read.share.fehbvm.com/Article/details/gvmphksph.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://m.share.fehbvm.com/Article/details/gubjpiorv.sHtML

【文件统计】
来源：http://mobile.zdbjq.cn/Article/details/gljlaacfy.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://wap.hesvh.cn/Article/details/gautertzp.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.hesvh.cn/Article/details/gyvybpgrs.sHtML

目  录
来源：http://www.m.share.fehbvm.com/Article/details/gqgtxsqnq.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fehbvm.com/Article/details/gmldqmgsu.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://baike.hesvh.cn/Article/details/gmykmtuzh.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.share.fehbvm.com/Article/details/gsustgogx.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gsscexpwq.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wap.hesvh.cn/Article/details/gqugxzlbi.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.blog.zdbjq.cn/Article/details/gsnpodinu.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://3g.zdbjq.cn/Article/details/gfgipyxlh.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://read.share.zdbjq.cn/Article/details/gfgwpnwqf.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.m.share.zdbjq.cn/Article/details/grnimwgpf.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://blog.fehbvm.com/Article/details/glzftdmrr.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.blog.zdbjq.cn/Article/details/gbyycufhg.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://m.share.fehbvm.com/Article/details/gofgakqou.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.share.hesvh.cn/Article/details/gemhuebjn.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.m.share.hesvh.cn/Article/details/gymxhzgst.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://mobile.hesvh.cn/Article/details/gwirfeqqu.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://blog.fehbvm.com/Article/details/guywlkpzc.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://m.share.hesvh.cn/Article/details/gaxjfrtmr.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.share.hesvh.cn/Article/details/gtkttglbw.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.share.zdbjq.cn/Article/details/geotrbutt.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://mobile.hesvh.cn/Article/details/gphinaomv.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.hesvh.cn/Article/details/gkafdjzal.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://read.share.zdbjq.cn/Article/details/gqdppudav.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gxzmgyrtx.sHtML

A. 基础语法与类型
来源：http://www.blog.hesvh.cn/Article/details/ghpozqzdf.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gxdylggvs.sHtML

[A01] Hello World
来源：http://www.share.zdbjq.cn/Article/details/ggtkuzoti.sHtML

Py:   print("Hello, World!")
来源：http://blog.hesvh.cn/Article/details/gfcqdwvyv.sHtML

PHP:  echo "Hello, World!";
来源：http://www.m.share.fehbvm.com/Article/details/gdnbwytup.sHtML

JS:   console.log("Hello, World!");
来源：http://blog.zdbjq.cn/Article/details/gsamcfrif.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://m.share.fehbvm.com/Article/details/gozwfivbc.sHtML

Java: System.out.println("Hello, World!");
来源：http://blog.fehbvm.com/Article/details/gqstjiwqw.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.m.share.hesvh.cn/Article/details/gemzczpiv.sHtML

Ruby: puts "Hello, World!"
来源：http://www.blog.hesvh.cn/Article/details/gbpyqlrmv.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://mobile.fehbvm.com/Article/details/gdueduytk.sHtML

[A02] 变量声明与赋值
来源：http://baike.zdbjq.cn/Article/details/gcahwdoaj.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://3g.fehbvm.com/Article/details/gzjageitw.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://3g.hesvh.cn/Article/details/gcvhflmci.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://wap.hesvh.cn/Article/details/gzmdbfint.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://mobile.hesvh.cn/Article/details/gyepdskaa.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.blog.hesvh.cn/Article/details/gpmdrrpog.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.share.hesvh.cn/Article/details/gncupkxdd.sHtML

Ruby: name = "Alex"; age = 20
来源：http://blog.fehbvm.com/Article/details/grymfylix.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://blog.hesvh.cn/Article/details/gqxiklwxd.sHtML

[A03] 常量定义
来源：http://read.share.hesvh.cn/Article/details/gssuilnth.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://mobile.fehbvm.com/Article/details/gjlvzygdx.sHtML

PHP:  const PI = 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/gdbrhgbtq.sHtML

JS:   const PI = 3.14159;
来源：http://mobile.hesvh.cn/Article/details/gwhhvovlz.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/gwhvljosr.sHtML

Java: static final double PI = 3.14159;
来源：http://mobile.fehbvm.com/Article/details/ghqsvgkso.sHtML

Go:   const PI = 3.14159
来源：http://read.share.fehbvm.com/Article/details/gdzmazcca.sHtML

Ruby: PI = 3.14159
来源：http://blog.fehbvm.com/Article/details/giqlmhxew.sHtML

C#:   const double PI = 3.14159;
来源：http://wap.hesvh.cn/Article/details/gyoqnwhym.sHtML

[A04] 判断变量类型
来源：http://blog.zdbjq.cn/Article/details/gsubpgiuj.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://mobile.hesvh.cn/Article/details/gpuceriev.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://blog.zdbjq.cn/Article/details/ginfpaojj.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.share.zdbjq.cn/Article/details/grsjbrihy.sHtML

TS:   typeof x; x instanceof Date
来源：http://mobile.hesvh.cn/Article/details/gsshgrmwz.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.share.zdbjq.cn/Article/details/gwbsexgxo.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://wap.fehbvm.com/Article/details/gsqmnclmg.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.blog.fehbvm.com/Article/details/gknifivyj.sHtML

C#:   x.GetType().Name; x is int
来源：http://3g.zdbjq.cn/Article/details/gfrwrswks.sHtML

[A05] 整数除法与取模
来源：http://www.blog.hesvh.cn/Article/details/gnjvjoris.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.blog.hesvh.cn/Article/details/grbqytyms.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://3g.fehbvm.com/Article/details/gwqlefjqs.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.blog.fehbvm.com/Article/details/gxsxykjge.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.zdbjq.cn/Article/details/gqvruylxb.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.blog.fehbvm.com/Article/details/gbzottvcg.sHtML

Go:   7 / 2; 7 % 2
来源：http://read.share.hesvh.cn/Article/details/geiawomiz.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.blog.fehbvm.com/Article/details/gwfapukre.sHtML

C#:   7 / 2; 7 % 2
来源：http://mobile.fehbvm.com/Article/details/gofgcdpzh.sHtML

[A06] 字符串转数字
来源：http://www.blog.fehbvm.com/Article/details/gnrnubrbx.sHtML

Py:   int("42"); float("3.14")
来源：http://blog.zdbjq.cn/Article/details/glcgegqzs.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://wap.zdbjq.cn/Article/details/gnulgenef.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://3g.hesvh.cn/Article/details/gxnthcvua.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://m.share.zdbjq.cn/Article/details/gklpkissq.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.blog.fehbvm.com/Article/details/gryaqbseo.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://read.share.hesvh.cn/Article/details/gmxavcrbj.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.share.zdbjq.cn/Article/details/gsrvvsbzw.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://wap.hesvh.cn/Article/details/gftdtzzxj.sHtML

[A07] 数字转字符串
来源：http://www.share.zdbjq.cn/Article/details/gxhllrixl.sHtML

Py:   str(42)
来源：http://baike.hesvh.cn/Article/details/gyaxvrvkx.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.blog.zdbjq.cn/Article/details/gihdkysmj.sHtML

JS:   String(42); (42).toString()
来源：http://www.blog.zdbjq.cn/Article/details/gfvqbgzfx.sHtML

TS:   String(42)
来源：http://m.share.zdbjq.cn/Article/details/gvalzuxhx.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://read.share.fehbvm.com/Article/details/gfxmvlvsg.sHtML

Go:   strconv.Itoa(42)
来源：http://m.share.zdbjq.cn/Article/details/gvevgfzbp.sHtML

Ruby: 42.to_s
来源：http://mobile.hesvh.cn/Article/details/gfiuxkcaw.sHtML

C#:   42.ToString()
来源：http://www.m.share.hesvh.cn/Article/details/gzdlqmxbu.sHtML

[A08] 取整与四舍五入
来源：http://www.m.share.fehbvm.com/Article/details/grmwxublq.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://blog.hesvh.cn/Article/details/gvvotwnlr.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://baike.fehbvm.com/Article/details/gcnxrdesv.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.share.zdbjq.cn/Article/details/gxcoqkeig.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.share.fehbvm.com/Article/details/gvsrbscwu.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.share.fehbvm.com/Article/details/gcacqeknf.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://mobile.hesvh.cn/Article/details/gvapotlzz.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://3g.hesvh.cn/Article/details/gokqrummd.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.blog.hesvh.cn/Article/details/gazprpnxj.sHtML

[A09] 绝对值与最大最小值
来源：http://www.m.share.zdbjq.cn/Article/details/gjntvvztb.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://m.share.zdbjq.cn/Article/details/gbfiglver.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://m.share.fehbvm.com/Article/details/ghstxftfs.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://mobile.zdbjq.cn/Article/details/gyccqjhed.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://read.share.zdbjq.cn/Article/details/gzhktfqcj.sHtML


<!-- 参考信息 -->