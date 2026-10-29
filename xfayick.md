代发 wailian999

[U63] PHP：文件读写
来源：http://www.blog.hesvh.cn/Article/details/gkjhjereu.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.hesvh.cn/Article/details/giqqldwlv.sHtML

[U64] PHP：目录遍历
来源：http://3g.zdbjq.cn/Article/details/glvpdwovu.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://read.share.fehbvm.com/Article/details/gesuahnrh.sHtML

[U65] PHP：会话
来源：http://mobile.hesvh.cn/Article/details/gegbcjeez.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://read.share.hesvh.cn/Article/details/gmcyqpknc.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.fehbvm.com/Article/details/gzqkcmeao.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://read.share.hesvh.cn/Article/details/gqtllxymi.sHtML

[U67] PHP：处理文件上传
来源：http://www.blog.hesvh.cn/Article/details/gwrntqkel.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mobile.zdbjq.cn/Article/details/geuqbunkc.sHtML

[U68] PHP：PDO 连接
来源：http://m.share.zdbjq.cn/Article/details/ggmpnrfdh.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://read.share.hesvh.cn/Article/details/gccpbsbrd.sHtML

[U69] PHP：PDO 预处理
来源：http://www.m.share.zdbjq.cn/Article/details/gejvvfubu.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mobile.zdbjq.cn/Article/details/guisqawjh.sHtML

[U70] PHP：PDO 事务
来源：http://m.share.hesvh.cn/Article/details/gggelrbww.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.fehbvm.com/Article/details/grrdvqizz.sHtML

[U71] PHP：抛出异常
来源：http://www.m.share.hesvh.cn/Article/details/goqlzgvjq.sHtML

throw new RuntimeException("失败", 500);
来源：http://read.share.fehbvm.com/Article/details/gsddpnhlp.sHtML

[U72] PHP：写错误日志
来源：http://3g.fehbvm.com/Article/details/gfmdofuvh.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.share.hesvh.cn/Article/details/gshliwmsr.sHtML

[U73] PHP：读取 ini 配置
来源：http://mobile.fehbvm.com/Article/details/gjkwgyqcj.sHtML

parse_ini_file("config.ini", true)
来源：http://m.share.zdbjq.cn/Article/details/gzzczlanx.sHtML

[U74] PHP：读取环境变量
来源：http://m.share.zdbjq.cn/Article/details/gyawobcpd.sHtML

getenv("APP_ENV") ?: "production"
来源：http://m.share.zdbjq.cn/Article/details/gptuwccgo.sHtML

[U75] PHP：依赖注入
来源：http://mobile.fehbvm.com/Article/details/gelccomed.sHtML

composer require psr/container
来源：http://read.share.hesvh.cn/Article/details/goqfusftg.sHtML

[U76] PHP：简单路由
来源：http://m.share.fehbvm.com/Article/details/gvthfcwcr.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://blog.hesvh.cn/Article/details/gbijmhzil.sHtML

[U77] PHP：模板渲染
来源：http://www.blog.zdbjq.cn/Article/details/gjwilclaa.sHtML

composer require twig/twig
来源：http://www.share.zdbjq.cn/Article/details/gglgoqgpg.sHtML

[U78] PHP：单元测试
来源：http://www.blog.hesvh.cn/Article/details/ggvakkktj.sHtML

composer require --dev phpunit/phpunit
来源：http://www.blog.fehbvm.com/Article/details/ggoqwvtjv.sHtML

[U79] PHP：静态分析
来源：http://read.share.fehbvm.com/Article/details/guqknpfyu.sHtML

composer require --dev phpstan/phpstan
来源：http://mobile.zdbjq.cn/Article/details/gjqaepyfs.sHtML

[U80] PHP：代码规范修复
来源：http://read.share.zdbjq.cn/Article/details/gycpllhmv.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://3g.fehbvm.com/Article/details/glmtavlbm.sHtML

[U81] JS：初始化项目
来源：http://wap.zdbjq.cn/Article/details/gvqegveng.sHtML

npm init -y;  npm i express
来源：http://www.share.zdbjq.cn/Article/details/gfdfdjlbc.sHtML

[U82] JS：package.json 脚本
来源：http://wap.zdbjq.cn/Article/details/gucuoxrck.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.m.share.fehbvm.com/Article/details/gwrlnluym.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.share.zdbjq.cn/Article/details/gfovtdwjc.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://blog.fehbvm.com/Article/details/ghmvptvoq.sHtML

[U84] JS：CommonJS 写法
来源：http://mobile.fehbvm.com/Article/details/ggyzkanya.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.zdbjq.cn/Article/details/gdodhrodc.sHtML

[U85] JS：可选链
来源：http://www.share.fehbvm.com/Article/details/gyhwcbozq.sHtML

a?.b?.c
来源：http://www.m.share.hesvh.cn/Article/details/gjfjupfkx.sHtML

[U86] JS：空值合并
来源：http://wap.fehbvm.com/Article/details/grftlgian.sHtML

a ?? b
来源：http://baike.hesvh.cn/Article/details/gdyglzpyo.sHtML

[U87] JS：解构默认值
来源：http://baike.hesvh.cn/Article/details/gscjedbor.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.hesvh.cn/Article/details/gtvlcshtl.sHtML

[U88] JS：对象展开合并
来源：http://baike.hesvh.cn/Article/details/gimphyfit.sHtML

{ ...a, ...b }
来源：http://mobile.fehbvm.com/Article/details/gptdkutvb.sHtML

[U89] JS：数组去重
来源：http://mobile.fehbvm.com/Article/details/gchwegdrv.sHtML

[...new Set(arr)]
来源：http://read.share.fehbvm.com/Article/details/giqbmuffp.sHtML

[U90] JS：数字数组排序
来源：http://read.share.fehbvm.com/Article/details/gwywudihf.sHtML

[...arr].sort((a, b) => a - b)
来源：http://blog.fehbvm.com/Article/details/gqyxkroxs.sHtML

[U91] JS：对象键值遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gldleqqxi.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://baike.hesvh.cn/Article/details/gbqxqarsv.sHtML

[U92] JS：深拷贝
来源：http://3g.fehbvm.com/Article/details/gbxqcsmct.sHtML

structuredClone(obj)
来源：http://www.share.zdbjq.cn/Article/details/gelgtknfd.sHtML

[U93] JS：模板字符串
来源：http://read.share.zdbjq.cn/Article/details/guhndntjd.sHtML

`共 ${n} 条`
来源：http://3g.hesvh.cn/Article/details/gltfwbhrw.sHtML

[U94] JS：箭头函数
来源：http://mobile.fehbvm.com/Article/details/glicduqia.sHtML

const double = x => x * 2;
来源：http://www.share.zdbjq.cn/Article/details/gvahqvbut.sHtML

[U95] JS：Promise 包装
来源：http://read.share.zdbjq.cn/Article/details/grlrpwojg.sHtML

new Promise((resolve, reject) => {})
来源：http://3g.hesvh.cn/Article/details/gcyzzxcgl.sHtML

[U96] JS：async/await 与异常
来源：http://www.m.share.zdbjq.cn/Article/details/gbxglovtw.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://blog.hesvh.cn/Article/details/gsjrzekma.sHtML

[U97] JS：并发请求
来源：http://m.share.hesvh.cn/Article/details/gztiryuew.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.fehbvm.com/Article/details/gzsygpyva.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.share.zdbjq.cn/Article/details/gprgxguyh.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mobile.hesvh.cn/Article/details/geumhxzxj.sHtML

[U99] JS：事件监听
来源：http://baike.fehbvm.com/Article/details/gowhlabod.sHtML

el.addEventListener("click", e => {})
来源：http://blog.zdbjq.cn/Article/details/ghkxvihgo.sHtML

[U100] JS：DOM 查询
来源：http://m.share.zdbjq.cn/Article/details/gcsqyedrp.sHtML

document.querySelector(".item")
来源：http://www.blog.hesvh.cn/Article/details/gljwgrghd.sHtML

[U101] JS：classList 操作
来源：http://wap.hesvh.cn/Article/details/godsjteyy.sHtML

el.classList.toggle("active")
来源：http://m.share.fehbvm.com/Article/details/gnwfromyi.sHtML

[U102] JS：本地存储
来源：http://blog.fehbvm.com/Article/details/gelnvtxdj.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://read.share.fehbvm.com/Article/details/gngswrses.sHtML

[U103] JS：定时器
来源：http://mobile.zdbjq.cn/Article/details/gafbagbfe.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.m.share.zdbjq.cn/Article/details/gdogsjoco.sHtML

[U104] JS：防抖
来源：http://read.share.hesvh.cn/Article/details/gdcxbqcsq.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.zdbjq.cn/Article/details/gqllyxpal.sHtML

[U105] JS：节流
来源：http://mobile.hesvh.cn/Article/details/guiuwzkyd.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://blog.hesvh.cn/Article/details/gkouwqscy.sHtML

[U106] JS：日期格式化
来源：http://wap.zdbjq.cn/Article/details/grucadnyi.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.m.share.hesvh.cn/Article/details/gpbwznbxp.sHtML

[U107] JS：数字千分位
来源：http://3g.hesvh.cn/Article/details/gbadfnodm.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wap.hesvh.cn/Article/details/gtksnxwue.sHtML

[U108] JS：随机整数
来源：http://read.share.zdbjq.cn/Article/details/gijoqkehj.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.fehbvm.com/Article/details/gqthheqrb.sHtML

[U109] JS：数组分组
来源：http://3g.hesvh.cn/Article/details/gdwquqefr.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.hesvh.cn/Article/details/gzgkcqane.sHtML

[U110] JS：数组分块
来源：http://blog.fehbvm.com/Article/details/gqiyrayij.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.m.share.fehbvm.com/Article/details/guyrcysfa.sHtML

[U111] JS：对象转 Map
来源：http://read.share.hesvh.cn/Article/details/ghcxsbydd.sHtML

new Map(Object.entries(obj))
来源：http://m.share.fehbvm.com/Article/details/gddoyhtut.sHtML

[U112] JS：字符串补位
来源：http://www.m.share.zdbjq.cn/Article/details/gkpzfpagq.sHtML

"7".padStart(3, "0")
来源：http://blog.hesvh.cn/Article/details/gbgtbcwlv.sHtML

[U113] JS：正则替换全部
来源：http://mobile.zdbjq.cn/Article/details/gnimrablo.sHtML

s.replaceAll("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gavezbmdp.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.fehbvm.com/Article/details/gkkhafyvw.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.hesvh.cn/Article/details/gzxyxpzsm.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.hesvh.cn/Article/details/gxfxvwsah.sHtML

crypto.randomUUID()
来源：http://blog.zdbjq.cn/Article/details/gvuebovvh.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://m.share.hesvh.cn/Article/details/graqrwljd.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.hesvh.cn/Article/details/grjwlhvbn.sHtML

[U117] JS：单元测试
来源：http://www.blog.hesvh.cn/Article/details/grbofuktj.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.zdbjq.cn/Article/details/gzebpinrc.sHtML

[U118] JS：开发服务器
来源：http://read.share.hesvh.cn/Article/details/gyzotffqh.sHtML

npm i -D vite;  npx vite
来源：http://www.share.fehbvm.com/Article/details/gftqvteft.sHtML

[U119] JS：生产构建
来源：http://m.share.fehbvm.com/Article/details/ggyunxefw.sHtML

npx vite build
来源：http://mobile.zdbjq.cn/Article/details/glzwmjrqr.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://3g.fehbvm.com/Article/details/gnmrqqgyv.sHtML

import.meta.env.VITE_API_URL
来源：http://www.m.share.fehbvm.com/Article/details/gwrrezxua.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/groisoaaw.sHtML

统计汇总
来源：http://3g.hesvh.cn/Article/details/gavvybqvi.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gaqgwulhh.sHtML

按语言统计（条）：
来源：http://www.share.fehbvm.com/Article/details/gvbvhfzhg.sHtML

Python ......... 252
来源：http://m.share.zdbjq.cn/Article/details/grhfaqgfi.sHtML

PHP ............ 252
来源：http://www.share.hesvh.cn/Article/details/grphcehni.sHtML

JavaScript ..... 252
来源：http://mobile.fehbvm.com/Article/details/gztljnuft.sHtML

TypeScript ..... 212
来源：http://baike.fehbvm.com/Article/details/guxxiklle.sHtML

Java ........... 212
来源：http://wap.fehbvm.com/Article/details/gleumkxjh.sHtML

Go ............. 212
来源：http://mobile.fehbvm.com/Article/details/gwyiijsyp.sHtML

Ruby ........... 212
来源：http://www.share.fehbvm.com/Article/details/gmqsuufra.sHtML

C# ............. 212
来源：http://m.share.zdbjq.cn/Article/details/gzkycqsbo.sHtML

C .............. 30
来源：http://mobile.zdbjq.cn/Article/details/gjnwasflm.sHtML

C++ ............ 30
来源：http://www.m.share.zdbjq.cn/Article/details/gzxdpqxnu.sHtML

SQL ............ 90
来源：http://www.blog.hesvh.cn/Article/details/gohluhjet.sHtML

Bash ........... 80
来源：http://www.share.hesvh.cn/Article/details/gduzzjuzn.sHtML

Kotlin ......... 15
来源：http://www.share.zdbjq.cn/Article/details/gfbvfukrg.sHtML

Swift .......... 15
来源：http://read.share.zdbjq.cn/Article/details/gfrnyxnds.sHtML

Lua ............ 10
来源：http://wap.zdbjq.cn/Article/details/gnencuvph.sHtML

Perl ........... 10
来源：http://blog.zdbjq.cn/Article/details/gmydybltf.sHtML

Scala .......... 10
来源：http://www.share.zdbjq.cn/Article/details/gnvnooayv.sHtML

------------------------------------
来源：http://mobile.hesvh.cn/Article/details/gbzjwgskn.sHtML

合计 ........... 2106 条
来源：http://blog.fehbvm.com/Article/details/gcfhpqpka.sHtML

按章节统计：
来源：http://mobile.zdbjq.cn/Article/details/gsoqvrvpc.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://read.share.hesvh.cn/Article/details/gzsfjlihn.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://read.share.fehbvm.com/Article/details/gfjnjvmyi.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://blog.zdbjq.cn/Article/details/ghhajykts.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://3g.fehbvm.com/Article/details/gvcaxqsmt.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://baike.zdbjq.cn/Article/details/gbkhzbqdm.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.blog.fehbvm.com/Article/details/gjdrnbrut.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.blog.fehbvm.com/Article/details/gtpelpdsh.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mobile.hesvh.cn/Article/details/gcrbqgkii.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://3g.hesvh.cn/Article/details/gqqqunygk.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wap.fehbvm.com/Article/details/gqktybypp.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.m.share.hesvh.cn/Article/details/gwpdkniys.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.share.hesvh.cn/Article/details/geailvbiu.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://read.share.hesvh.cn/Article/details/gcarimxeu.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://blog.zdbjq.cn/Article/details/ghimoavdy.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wap.zdbjq.cn/Article/details/gjeqtdvqd.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.m.share.fehbvm.com/Article/details/grosclrzh.sHtML

Q SQL 专题                              90
来源：http://blog.zdbjq.cn/Article/details/gqhnwirlu.sHtML

R Bash 专题                             80
来源：http://read.share.zdbjq.cn/Article/details/gdifwlgfc.sHtML

S C / C++ 专题                          60
来源：http://www.blog.hesvh.cn/Article/details/gqocdjuqu.sHtML

T 其他语言补充                          60
来源：http://read.share.zdbjq.cn/Article/details/gkfnbbddc.sHtML

U 高频实用片段                         120
来源：http://m.share.hesvh.cn/Article/details/gjhrdsnhk.sHtML

------------------------------------
来源：http://3g.hesvh.cn/Article/details/golbldnfq.sHtML

合计                                  2106 条
来源：http://www.blog.fehbvm.com/Article/details/glqwsyzck.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.hesvh.cn/Article/details/gjavgeojr.sHtML

使用提醒
来源：http://www.blog.fehbvm.com/Article/details/ggahuveoc.sHtML

--------------------------------------------------------------------------------
来源：http://baike.zdbjq.cn/Article/details/gogcvmdox.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://3g.zdbjq.cn/Article/details/gywgoetob.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://3g.zdbjq.cn/Article/details/gobaggsxx.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.share.zdbjq.cn/Article/details/grgguldlu.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://3g.fehbvm.com/Article/details/gbntstuyz.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wap.zdbjq.cn/Article/details/gwyxjcfxj.sHtML

—— 文件结束 ——
来源：http://3g.fehbvm.com/Article/details/guowdzoqj.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gullrtzzx.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://read.share.hesvh.cn/Article/details/gedbeennj.sHtML

Common Programming Examples Cheat Book
来源：http://baike.fehbvm.com/Article/details/gbglhjfzs.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/guawxbegu.sHtML

【收录内容】
来源：http://read.share.zdbjq.cn/Article/details/gxqutbfnm.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://read.share.fehbvm.com/Article/details/gwwrylgho.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://read.share.hesvh.cn/Article/details/gihmbqbxp.sHtML

SQL · Bash · C · C++
来源：http://mobile.zdbjq.cn/Article/details/gcmkgmwgy.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://m.share.zdbjq.cn/Article/details/gwzsrrnaf.sHtML

【使用说明】
来源：http://www.blog.hesvh.cn/Article/details/gsiqpbvhs.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://3g.fehbvm.com/Article/details/gkyyptfnv.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://m.share.zdbjq.cn/Article/details/glqhxwvmo.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.blog.zdbjq.cn/Article/details/gqsmthlme.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://m.share.hesvh.cn/Article/details/gdjackmok.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://baike.hesvh.cn/Article/details/gzeifhrvm.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wap.zdbjq.cn/Article/details/gbrwmwoot.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://m.share.fehbvm.com/Article/details/gtvdclgct.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://read.share.fehbvm.com/Article/details/gabqhphjt.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://mobile.hesvh.cn/Article/details/gmbzrxejl.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://read.share.fehbvm.com/Article/details/gqwehbvlq.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://blog.fehbvm.com/Article/details/gopigwtbv.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://wap.hesvh.cn/Article/details/gxxgupkgf.sHtML

【文件统计】
来源：http://wap.fehbvm.com/Article/details/gmqdotfca.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://blog.fehbvm.com/Article/details/gwitqessq.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fehbvm.com/Article/details/ggckjcqyh.sHtML

目  录
来源：http://read.share.hesvh.cn/Article/details/gswcfacsd.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.fehbvm.com/Article/details/gzxyxmtzx.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://baike.hesvh.cn/Article/details/gmtdjcuib.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://mobile.zdbjq.cn/Article/details/glovyqinx.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://mobile.zdbjq.cn/Article/details/gmkqjjuja.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wap.hesvh.cn/Article/details/gosvpllum.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://blog.zdbjq.cn/Article/details/gjxqnozqn.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.blog.hesvh.cn/Article/details/gackqvyrz.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.blog.hesvh.cn/Article/details/gpknczork.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.m.share.hesvh.cn/Article/details/gfmdxukhg.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://baike.fehbvm.com/Article/details/glwhxnaph.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://baike.fehbvm.com/Article/details/gtezmbhts.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://3g.fehbvm.com/Article/details/gzpctkejg.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://wap.zdbjq.cn/Article/details/gbzlwmwxs.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://mobile.zdbjq.cn/Article/details/gtleozlfo.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://read.share.fehbvm.com/Article/details/gsotkylqk.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://blog.zdbjq.cn/Article/details/gdlmdhbxn.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://wap.fehbvm.com/Article/details/ginrflqcs.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.blog.zdbjq.cn/Article/details/gepkwcice.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.m.share.fehbvm.com/Article/details/gyaigxmvt.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://3g.fehbvm.com/Article/details/gfryoscmu.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.hesvh.cn/Article/details/gvnjufntn.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://read.share.zdbjq.cn/Article/details/ghydgzjhf.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gumhzcpfy.sHtML

A. 基础语法与类型
来源：http://read.share.hesvh.cn/Article/details/gtwmufora.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gwrnuwoky.sHtML

[A01] Hello World
来源：http://baike.hesvh.cn/Article/details/giimviutb.sHtML

Py:   print("Hello, World!")
来源：http://www.blog.fehbvm.com/Article/details/gpogykvjh.sHtML

PHP:  echo "Hello, World!";
来源：http://www.blog.hesvh.cn/Article/details/gukdhrwtp.sHtML

JS:   console.log("Hello, World!");
来源：http://mobile.fehbvm.com/Article/details/gachgamlf.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://3g.zdbjq.cn/Article/details/gpzqfgwdb.sHtML

Java: System.out.println("Hello, World!");
来源：http://baike.zdbjq.cn/Article/details/guwxfqhcl.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://blog.zdbjq.cn/Article/details/gwpjffpcm.sHtML

Ruby: puts "Hello, World!"
来源：http://www.m.share.hesvh.cn/Article/details/gvcasmeke.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://mobile.zdbjq.cn/Article/details/gsxfnvzrs.sHtML

[A02] 变量声明与赋值
来源：http://www.blog.zdbjq.cn/Article/details/gmxplaawa.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://m.share.fehbvm.com/Article/details/gbbtaucda.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.blog.zdbjq.cn/Article/details/gztfuuvdr.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://read.share.fehbvm.com/Article/details/gbdfrkgoi.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.share.hesvh.cn/Article/details/gaebijyxv.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://read.share.zdbjq.cn/Article/details/gdcbmyuko.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.m.share.fehbvm.com/Article/details/gdsuuhhni.sHtML

Ruby: name = "Alex"; age = 20
来源：http://read.share.zdbjq.cn/Article/details/gjmxginfr.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://m.share.hesvh.cn/Article/details/geozctyos.sHtML

[A03] 常量定义
来源：http://blog.zdbjq.cn/Article/details/gmcdeinje.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.blog.fehbvm.com/Article/details/gphijiqxr.sHtML

PHP:  const PI = 3.14159;
来源：http://blog.fehbvm.com/Article/details/gsswhcdla.sHtML

JS:   const PI = 3.14159;
来源：http://blog.hesvh.cn/Article/details/guhahhpif.sHtML

TS:   const PI: number = 3.14159;
来源：http://read.share.hesvh.cn/Article/details/grxycilhc.sHtML

Java: static final double PI = 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/gebfafrmj.sHtML

Go:   const PI = 3.14159
来源：http://blog.fehbvm.com/Article/details/gxbnogstj.sHtML

Ruby: PI = 3.14159
来源：http://mobile.zdbjq.cn/Article/details/gitstlzkd.sHtML

C#:   const double PI = 3.14159;
来源：http://3g.fehbvm.com/Article/details/gfxtpjpsc.sHtML

[A04] 判断变量类型
来源：http://www.blog.zdbjq.cn/Article/details/gvcwhzdcq.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.blog.fehbvm.com/Article/details/gbjqyyrvl.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://wap.fehbvm.com/Article/details/gruprgqix.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://m.share.fehbvm.com/Article/details/grphngetg.sHtML

TS:   typeof x; x instanceof Date
来源：http://baike.hesvh.cn/Article/details/gtuqyrfom.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://3g.zdbjq.cn/Article/details/giuixyytq.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://3g.fehbvm.com/Article/details/gmtcopozk.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.share.zdbjq.cn/Article/details/grrwgayvs.sHtML

C#:   x.GetType().Name; x is int
来源：http://3g.zdbjq.cn/Article/details/ggqpmagio.sHtML

[A05] 整数除法与取模
来源：http://mobile.fehbvm.com/Article/details/gkxqodsvv.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://m.share.zdbjq.cn/Article/details/gdfbihoso.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://baike.zdbjq.cn/Article/details/ggktatdlo.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.hesvh.cn/Article/details/gmdciyhbs.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.fehbvm.com/Article/details/ghvcsaibe.sHtML

Java: 7 / 2; 7 % 2
来源：http://baike.hesvh.cn/Article/details/gcplsdjrz.sHtML

Go:   7 / 2; 7 % 2
来源：http://baike.zdbjq.cn/Article/details/gvmiuzesg.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.share.zdbjq.cn/Article/details/ghapueqrw.sHtML

C#:   7 / 2; 7 % 2
来源：http://wap.hesvh.cn/Article/details/gewyywhng.sHtML

[A06] 字符串转数字
来源：http://www.blog.zdbjq.cn/Article/details/gufzxyubc.sHtML

Py:   int("42"); float("3.14")
来源：http://3g.fehbvm.com/Article/details/ggxcduwus.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.share.fehbvm.com/Article/details/gozamuhko.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.m.share.fehbvm.com/Article/details/gywpinahd.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.m.share.hesvh.cn/Article/details/gmisymdkd.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://wap.fehbvm.com/Article/details/gbkwvhnbv.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://mobile.hesvh.cn/Article/details/gxvhdyzja.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://3g.zdbjq.cn/Article/details/gsmttlwpm.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.share.fehbvm.com/Article/details/gyvsqxnhe.sHtML

[A07] 数字转字符串
来源：http://wap.hesvh.cn/Article/details/gfgtnxifu.sHtML

Py:   str(42)
来源：http://www.blog.fehbvm.com/Article/details/glpuuunhp.sHtML

PHP:  (string) 42; strval(42)
来源：http://mobile.fehbvm.com/Article/details/gincdxgjk.sHtML

JS:   String(42); (42).toString()
来源：http://www.blog.zdbjq.cn/Article/details/gzqrcaemm.sHtML

TS:   String(42)
来源：http://wap.zdbjq.cn/Article/details/gteyeoonz.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://read.share.fehbvm.com/Article/details/gccjjqnjr.sHtML

Go:   strconv.Itoa(42)
来源：http://www.blog.zdbjq.cn/Article/details/grmugsxcv.sHtML

Ruby: 42.to_s
来源：http://wap.fehbvm.com/Article/details/gbqwxxfat.sHtML

C#:   42.ToString()
来源：http://blog.zdbjq.cn/Article/details/gfongqqjy.sHtML

[A08] 取整与四舍五入
来源：http://wap.zdbjq.cn/Article/details/gqczkrkvd.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.m.share.fehbvm.com/Article/details/gctotlbea.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://read.share.fehbvm.com/Article/details/gyymhbrky.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://m.share.fehbvm.com/Article/details/gliuykhxt.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://baike.fehbvm.com/Article/details/gmunzfqmb.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://3g.hesvh.cn/Article/details/gbjxhwxfg.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.share.hesvh.cn/Article/details/gwygkjmst.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://3g.fehbvm.com/Article/details/gbeifklkv.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://m.share.zdbjq.cn/Article/details/gopdhghez.sHtML

[A09] 绝对值与最大最小值
来源：http://baike.zdbjq.cn/Article/details/gjutewpfz.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://3g.hesvh.cn/Article/details/gggrvqqvi.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://read.share.zdbjq.cn/Article/details/glgjtpble.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.m.share.fehbvm.com/Article/details/gqhelocts.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://blog.fehbvm.com/Article/details/gbmfxpnau.sHtML


<!-- 参考信息 -->