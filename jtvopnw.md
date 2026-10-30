代发 wailian999

[U63] PHP：文件读写
来源：http://www.blog.fehbvm.com/Article/details/ghetgsjqh.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.zdbjq.cn/Article/details/gvkdpvhjr.sHtML

[U64] PHP：目录遍历
来源：http://read.share.fehbvm.com/Article/details/gtpkimomp.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.share.zdbjq.cn/Article/details/gibmdonhr.sHtML

[U65] PHP：会话
来源：http://read.share.fehbvm.com/Article/details/gfgiqsowk.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.zdbjq.cn/Article/details/gyzwgyxpz.sHtML

[U66] PHP：设置 Cookie
来源：http://wap.zdbjq.cn/Article/details/gvdznjgtl.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.fehbvm.com/Article/details/ggqynxqtx.sHtML

[U67] PHP：处理文件上传
来源：http://www.share.fehbvm.com/Article/details/ghbimnpiq.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://blog.hesvh.cn/Article/details/gdpbreoui.sHtML

[U68] PHP：PDO 连接
来源：http://baike.hesvh.cn/Article/details/gigitwips.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://blog.hesvh.cn/Article/details/gjicftyrj.sHtML

[U69] PHP：PDO 预处理
来源：http://blog.zdbjq.cn/Article/details/gbttivjcr.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.m.share.zdbjq.cn/Article/details/gpmqjoxlp.sHtML

[U70] PHP：PDO 事务
来源：http://baike.fehbvm.com/Article/details/gvxafhjfs.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.hesvh.cn/Article/details/gabrewhhl.sHtML

[U71] PHP：抛出异常
来源：http://www.m.share.hesvh.cn/Article/details/gmlcfshro.sHtML

throw new RuntimeException("失败", 500);
来源：http://wap.hesvh.cn/Article/details/gzymkyawl.sHtML

[U72] PHP：写错误日志
来源：http://wap.hesvh.cn/Article/details/gkcshyehi.sHtML

error_log("失败: " . $e->getMessage());
来源：http://mobile.fehbvm.com/Article/details/ggelgtpek.sHtML

[U73] PHP：读取 ini 配置
来源：http://m.share.zdbjq.cn/Article/details/gviyqhrgh.sHtML

parse_ini_file("config.ini", true)
来源：http://wap.zdbjq.cn/Article/details/giasukijl.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.hesvh.cn/Article/details/gfuebhavw.sHtML

getenv("APP_ENV") ?: "production"
来源：http://mobile.zdbjq.cn/Article/details/gpajzxmys.sHtML

[U75] PHP：依赖注入
来源：http://blog.fehbvm.com/Article/details/gcyzrftos.sHtML

composer require psr/container
来源：http://blog.fehbvm.com/Article/details/gyapymlmn.sHtML

[U76] PHP：简单路由
来源：http://www.blog.fehbvm.com/Article/details/gfwxlibso.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://blog.hesvh.cn/Article/details/gimlvrgti.sHtML

[U77] PHP：模板渲染
来源：http://read.share.fehbvm.com/Article/details/gxgqgcevi.sHtML

composer require twig/twig
来源：http://www.m.share.fehbvm.com/Article/details/gltqxqfal.sHtML

[U78] PHP：单元测试
来源：http://mobile.zdbjq.cn/Article/details/gchslzftz.sHtML

composer require --dev phpunit/phpunit
来源：http://www.share.fehbvm.com/Article/details/gadfdqysp.sHtML

[U79] PHP：静态分析
来源：http://3g.fehbvm.com/Article/details/gubucpswu.sHtML

composer require --dev phpstan/phpstan
来源：http://baike.hesvh.cn/Article/details/gpmlibevl.sHtML

[U80] PHP：代码规范修复
来源：http://www.m.share.hesvh.cn/Article/details/ghrfhljgt.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://mobile.fehbvm.com/Article/details/ghztarkfn.sHtML

[U81] JS：初始化项目
来源：http://blog.hesvh.cn/Article/details/grvxcqhgw.sHtML

npm init -y;  npm i express
来源：http://blog.fehbvm.com/Article/details/gdywrefpe.sHtML

[U82] JS：package.json 脚本
来源：http://m.share.fehbvm.com/Article/details/ggnchvnsi.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.m.share.hesvh.cn/Article/details/gtadoriaf.sHtML

[U83] JS：ES Module 导入导出
来源：http://3g.zdbjq.cn/Article/details/glnarhzsu.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://baike.hesvh.cn/Article/details/gkvybpzwv.sHtML

[U84] JS：CommonJS 写法
来源：http://wap.zdbjq.cn/Article/details/gevfiwyxm.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.blog.fehbvm.com/Article/details/gzstcoyiq.sHtML

[U85] JS：可选链
来源：http://wap.fehbvm.com/Article/details/gplnpdgzf.sHtML

a?.b?.c
来源：http://www.m.share.hesvh.cn/Article/details/gfvluczdy.sHtML

[U86] JS：空值合并
来源：http://blog.fehbvm.com/Article/details/gzwjmzdyp.sHtML

a ?? b
来源：http://www.share.fehbvm.com/Article/details/gkcpohdob.sHtML

[U87] JS：解构默认值
来源：http://www.m.share.hesvh.cn/Article/details/gtfatllhp.sHtML

const { a = 1, b = 2 } = obj;
来源：http://wap.zdbjq.cn/Article/details/gvrcqnbrz.sHtML

[U88] JS：对象展开合并
来源：http://m.share.hesvh.cn/Article/details/gsluatmlk.sHtML

{ ...a, ...b }
来源：http://blog.zdbjq.cn/Article/details/gyblgdxnz.sHtML

[U89] JS：数组去重
来源：http://mobile.hesvh.cn/Article/details/gclbbeiot.sHtML

[...new Set(arr)]
来源：http://mobile.fehbvm.com/Article/details/gigwylvuz.sHtML

[U90] JS：数字数组排序
来源：http://wap.fehbvm.com/Article/details/gylqrgsxe.sHtML

[...arr].sort((a, b) => a - b)
来源：http://baike.hesvh.cn/Article/details/gdwmketym.sHtML

[U91] JS：对象键值遍历
来源：http://read.share.zdbjq.cn/Article/details/gbvmxhvtf.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://baike.hesvh.cn/Article/details/gorxqhndw.sHtML

[U92] JS：深拷贝
来源：http://www.m.share.fehbvm.com/Article/details/gnbykizmr.sHtML

structuredClone(obj)
来源：http://www.share.hesvh.cn/Article/details/gnprhitzl.sHtML

[U93] JS：模板字符串
来源：http://www.m.share.hesvh.cn/Article/details/grpdxmiom.sHtML

`共 ${n} 条`
来源：http://m.share.hesvh.cn/Article/details/gqvjnjqrj.sHtML

[U94] JS：箭头函数
来源：http://3g.fehbvm.com/Article/details/ghymltyhn.sHtML

const double = x => x * 2;
来源：http://www.blog.fehbvm.com/Article/details/glvnmaiaz.sHtML

[U95] JS：Promise 包装
来源：http://baike.hesvh.cn/Article/details/ghwkubcli.sHtML

new Promise((resolve, reject) => {})
来源：http://blog.zdbjq.cn/Article/details/gdqnuqjto.sHtML

[U96] JS：async/await 与异常
来源：http://3g.hesvh.cn/Article/details/gdyggpgli.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://baike.zdbjq.cn/Article/details/gdssgeuwg.sHtML

[U97] JS：并发请求
来源：http://blog.fehbvm.com/Article/details/gidjvanji.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.hesvh.cn/Article/details/grigvxzee.sHtML

[U98] JS：fetch 带 JSON
来源：http://baike.hesvh.cn/Article/details/gltdchzyu.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wap.hesvh.cn/Article/details/gcmvqbmni.sHtML

[U99] JS：事件监听
来源：http://blog.fehbvm.com/Article/details/gdqzokegx.sHtML

el.addEventListener("click", e => {})
来源：http://wap.zdbjq.cn/Article/details/gjvvopwbs.sHtML

[U100] JS：DOM 查询
来源：http://baike.hesvh.cn/Article/details/gwwezvlcr.sHtML

document.querySelector(".item")
来源：http://m.share.zdbjq.cn/Article/details/gmrxliijj.sHtML

[U101] JS：classList 操作
来源：http://m.share.hesvh.cn/Article/details/gvlhvxsws.sHtML

el.classList.toggle("active")
来源：http://baike.zdbjq.cn/Article/details/glzffxwtt.sHtML

[U102] JS：本地存储
来源：http://www.blog.fehbvm.com/Article/details/gypwrjfbj.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://mobile.fehbvm.com/Article/details/gldutunnn.sHtML

[U103] JS：定时器
来源：http://wap.hesvh.cn/Article/details/gqyqgioyo.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://baike.hesvh.cn/Article/details/grufhmlvx.sHtML

[U104] JS：防抖
来源：http://www.m.share.hesvh.cn/Article/details/gcexbhslr.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.zdbjq.cn/Article/details/gdcpvdbdx.sHtML

[U105] JS：节流
来源：http://www.blog.fehbvm.com/Article/details/gyblsmzup.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.zdbjq.cn/Article/details/ggprludya.sHtML

[U106] JS：日期格式化
来源：http://wap.hesvh.cn/Article/details/ggqdmthfk.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.blog.hesvh.cn/Article/details/gqkbzhsek.sHtML

[U107] JS：数字千分位
来源：http://baike.zdbjq.cn/Article/details/gtccmgpcz.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.hesvh.cn/Article/details/glvplsskc.sHtML

[U108] JS：随机整数
来源：http://m.share.zdbjq.cn/Article/details/gcbmtiapq.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.m.share.fehbvm.com/Article/details/gmhroxmuf.sHtML

[U109] JS：数组分组
来源：http://baike.fehbvm.com/Article/details/ggietwmro.sHtML

Object.groupBy(arr, x => x.type)
来源：http://read.share.fehbvm.com/Article/details/gjnpdutkr.sHtML

[U110] JS：数组分块
来源：http://wap.fehbvm.com/Article/details/gvucmogpm.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://m.share.hesvh.cn/Article/details/glttezddf.sHtML

[U111] JS：对象转 Map
来源：http://mobile.zdbjq.cn/Article/details/gjjqkigrr.sHtML

new Map(Object.entries(obj))
来源：http://www.m.share.zdbjq.cn/Article/details/glgjnggej.sHtML

[U112] JS：字符串补位
来源：http://www.m.share.fehbvm.com/Article/details/ggfgstrrs.sHtML

"7".padStart(3, "0")
来源：http://blog.zdbjq.cn/Article/details/gapacwokj.sHtML

[U113] JS：正则替换全部
来源：http://mobile.fehbvm.com/Article/details/gjwncyznx.sHtML

s.replaceAll("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gqkptsavg.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.hesvh.cn/Article/details/gugoigmrf.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.hesvh.cn/Article/details/ggrtrjheb.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.zdbjq.cn/Article/details/gspqsmjta.sHtML

crypto.randomUUID()
来源：http://3g.fehbvm.com/Article/details/gkmevyyax.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.zdbjq.cn/Article/details/ghbfkovdq.sHtML

/** @param {string} name */ function f(name) {}
来源：http://baike.fehbvm.com/Article/details/ggftlxfau.sHtML

[U117] JS：单元测试
来源：http://www.m.share.zdbjq.cn/Article/details/giwvjzuhp.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.zdbjq.cn/Article/details/gvagxscql.sHtML

[U118] JS：开发服务器
来源：http://www.share.zdbjq.cn/Article/details/gjsvzviag.sHtML

npm i -D vite;  npx vite
来源：http://www.share.fehbvm.com/Article/details/glhphcxbb.sHtML

[U119] JS：生产构建
来源：http://blog.hesvh.cn/Article/details/gxtkcddhn.sHtML

npx vite build
来源：http://mobile.hesvh.cn/Article/details/gazobwjqy.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.hesvh.cn/Article/details/ggnortwbr.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.zdbjq.cn/Article/details/gtepwwpmo.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/glpnqyljs.sHtML

统计汇总
来源：http://baike.fehbvm.com/Article/details/gxlyqimoo.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gqrbseoss.sHtML

按语言统计（条）：
来源：http://blog.zdbjq.cn/Article/details/gsthsrtsg.sHtML

Python ......... 252
来源：http://wap.hesvh.cn/Article/details/goxyyuitl.sHtML

PHP ............ 252
来源：http://3g.zdbjq.cn/Article/details/gvflvdszj.sHtML

JavaScript ..... 252
来源：http://m.share.fehbvm.com/Article/details/ghvhnjbgt.sHtML

TypeScript ..... 212
来源：http://wap.zdbjq.cn/Article/details/gymxsmqdk.sHtML

Java ........... 212
来源：http://mobile.zdbjq.cn/Article/details/gfruvehwy.sHtML

Go ............. 212
来源：http://baike.zdbjq.cn/Article/details/grbxwfywp.sHtML

Ruby ........... 212
来源：http://www.blog.zdbjq.cn/Article/details/gmgccsjlf.sHtML

C# ............. 212
来源：http://m.share.hesvh.cn/Article/details/gxwkviepl.sHtML

C .............. 30
来源：http://blog.hesvh.cn/Article/details/gantyzmdn.sHtML

C++ ............ 30
来源：http://mobile.zdbjq.cn/Article/details/gqkurocrx.sHtML

SQL ............ 90
来源：http://read.share.fehbvm.com/Article/details/gxzrklbjr.sHtML

Bash ........... 80
来源：http://www.share.zdbjq.cn/Article/details/gpqhfrrab.sHtML

Kotlin ......... 15
来源：http://wap.zdbjq.cn/Article/details/gbcvrglqb.sHtML

Swift .......... 15
来源：http://blog.zdbjq.cn/Article/details/ggjdnbsqv.sHtML

Lua ............ 10
来源：http://3g.fehbvm.com/Article/details/gcklbfexn.sHtML

Perl ........... 10
来源：http://blog.zdbjq.cn/Article/details/gnghsbwyh.sHtML

Scala .......... 10
来源：http://m.share.hesvh.cn/Article/details/gbjlskicf.sHtML

------------------------------------
来源：http://www.blog.zdbjq.cn/Article/details/gqflnqizk.sHtML

合计 ........... 2106 条
来源：http://www.share.zdbjq.cn/Article/details/guuneadxx.sHtML

按章节统计：
来源：http://m.share.fehbvm.com/Article/details/gmgzdwbga.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://3g.zdbjq.cn/Article/details/glafljbkk.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://m.share.zdbjq.cn/Article/details/gzmxxbmct.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://blog.hesvh.cn/Article/details/grsbrqisl.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://m.share.fehbvm.com/Article/details/gglmzhgai.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.blog.hesvh.cn/Article/details/ggrjjuthm.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wap.zdbjq.cn/Article/details/gicfkxixe.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://read.share.fehbvm.com/Article/details/gcpaqigvc.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.m.share.hesvh.cn/Article/details/gyryrjcsw.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://blog.hesvh.cn/Article/details/goabzezra.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://read.share.hesvh.cn/Article/details/ghusxbwyj.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.blog.zdbjq.cn/Article/details/glhgjmdtz.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://m.share.zdbjq.cn/Article/details/giqhebgcz.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mobile.zdbjq.cn/Article/details/gmpzzdqgn.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://blog.fehbvm.com/Article/details/grkdbcgxn.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wap.zdbjq.cn/Article/details/ghslcbefj.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.m.share.zdbjq.cn/Article/details/ggflggupd.sHtML

Q SQL 专题                              90
来源：http://baike.zdbjq.cn/Article/details/gguajcphb.sHtML

R Bash 专题                             80
来源：http://blog.hesvh.cn/Article/details/gzxdjjhpa.sHtML

S C / C++ 专题                          60
来源：http://wap.fehbvm.com/Article/details/gukmqdcxc.sHtML

T 其他语言补充                          60
来源：http://baike.fehbvm.com/Article/details/gsreibqtt.sHtML

U 高频实用片段                         120
来源：http://wap.zdbjq.cn/Article/details/gowhiijdm.sHtML

------------------------------------
来源：http://baike.zdbjq.cn/Article/details/gybbygcet.sHtML

合计                                  2106 条
来源：http://3g.zdbjq.cn/Article/details/ggtevroie.sHtML

--------------------------------------------------------------------------------
来源：http://baike.hesvh.cn/Article/details/gfgegljqf.sHtML

使用提醒
来源：http://www.m.share.zdbjq.cn/Article/details/ggdeqygbj.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fehbvm.com/Article/details/gcwtyrwha.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://m.share.zdbjq.cn/Article/details/gyjscrvhs.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://read.share.fehbvm.com/Article/details/gdidmyjrt.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://blog.fehbvm.com/Article/details/gkfjvaxgo.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://read.share.fehbvm.com/Article/details/gosrbrtck.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.share.hesvh.cn/Article/details/genuxkovh.sHtML

—— 文件结束 ——
来源：http://www.m.share.hesvh.cn/Article/details/gqqoiqbna.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gamqfjufa.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.blog.fehbvm.com/Article/details/glolvqxfr.sHtML

Common Programming Examples Cheat Book
来源：http://www.blog.hesvh.cn/Article/details/gtuajftjs.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gvtffhgox.sHtML

【收录内容】
来源：http://3g.zdbjq.cn/Article/details/ggkzodegp.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://wap.zdbjq.cn/Article/details/gdieonscp.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://blog.fehbvm.com/Article/details/gulawgrvd.sHtML

SQL · Bash · C · C++
来源：http://wap.hesvh.cn/Article/details/grzcfqkub.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://m.share.hesvh.cn/Article/details/gybtkfbyr.sHtML

【使用说明】
来源：http://www.m.share.hesvh.cn/Article/details/gdvewbwwx.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://read.share.fehbvm.com/Article/details/gjtkdjybp.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.m.share.hesvh.cn/Article/details/gflnfetma.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.share.fehbvm.com/Article/details/gngjgbfhy.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://mobile.zdbjq.cn/Article/details/gqmobcujh.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.m.share.zdbjq.cn/Article/details/gpvzpsqeo.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://blog.fehbvm.com/Article/details/gocefakww.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.blog.zdbjq.cn/Article/details/gnybouqwg.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://baike.zdbjq.cn/Article/details/gldvcsxpj.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://blog.fehbvm.com/Article/details/gphkpcvbu.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://wap.fehbvm.com/Article/details/ghtcimcnr.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://m.share.zdbjq.cn/Article/details/gkwcukqea.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://read.share.zdbjq.cn/Article/details/gzkvlwunf.sHtML

【文件统计】
来源：http://wap.fehbvm.com/Article/details/grgfjunte.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.m.share.fehbvm.com/Article/details/gxrlgstex.sHtML

--------------------------------------------------------------------------------
来源：http://3g.zdbjq.cn/Article/details/gqcjhjxzw.sHtML

目  录
来源：http://mobile.hesvh.cn/Article/details/gcguvpexj.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fehbvm.com/Article/details/gyximfyeh.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://m.share.fehbvm.com/Article/details/gbpzrwgpo.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.m.share.fehbvm.com/Article/details/ghctftaxv.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://3g.fehbvm.com/Article/details/ggjmceody.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.share.hesvh.cn/Article/details/gsppbqacl.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://read.share.hesvh.cn/Article/details/gqtvnlptq.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://3g.zdbjq.cn/Article/details/giinbpewc.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://baike.hesvh.cn/Article/details/gmmpospwh.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.m.share.fehbvm.com/Article/details/gofxgnkcz.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://3g.hesvh.cn/Article/details/grrrsroqg.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://mobile.zdbjq.cn/Article/details/ghpizgxno.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://wap.fehbvm.com/Article/details/gcivnrtcq.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://mobile.fehbvm.com/Article/details/gakofkise.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.blog.fehbvm.com/Article/details/gfkdcxshe.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://3g.zdbjq.cn/Article/details/gygfhpleq.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.blog.fehbvm.com/Article/details/gtzranbdl.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.share.fehbvm.com/Article/details/gxipnvmjb.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://blog.hesvh.cn/Article/details/gkzuvfumw.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.blog.fehbvm.com/Article/details/gpoxoyvfv.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://wap.zdbjq.cn/Article/details/gisdwnlkf.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.zdbjq.cn/Article/details/gnqldmfjf.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.hesvh.cn/Article/details/gonxziovh.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gumbtdjxq.sHtML

A. 基础语法与类型
来源：http://read.share.zdbjq.cn/Article/details/gljkzycjt.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/glbtvbxgm.sHtML

[A01] Hello World
来源：http://blog.fehbvm.com/Article/details/gybnlugnh.sHtML

Py:   print("Hello, World!")
来源：http://www.blog.hesvh.cn/Article/details/gmdaxzxks.sHtML

PHP:  echo "Hello, World!";
来源：http://3g.hesvh.cn/Article/details/gerrrrzns.sHtML

JS:   console.log("Hello, World!");
来源：http://mobile.hesvh.cn/Article/details/gemdzxdos.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.share.hesvh.cn/Article/details/gswstvbbq.sHtML

Java: System.out.println("Hello, World!");
来源：http://blog.hesvh.cn/Article/details/gdcomgclq.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://read.share.fehbvm.com/Article/details/gfbhcnmkf.sHtML

Ruby: puts "Hello, World!"
来源：http://mobile.fehbvm.com/Article/details/gpwhviyya.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.blog.hesvh.cn/Article/details/gcemkcsba.sHtML

[A02] 变量声明与赋值
来源：http://mobile.zdbjq.cn/Article/details/gsksyyjmk.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://baike.fehbvm.com/Article/details/gotkvvlqb.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://3g.fehbvm.com/Article/details/gpxaiiyjc.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.blog.fehbvm.com/Article/details/gjhusnnze.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://wap.hesvh.cn/Article/details/gmsljwfyr.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://wap.fehbvm.com/Article/details/gtkcjlvma.sHtML

Go:   name := "Alex"; age := 20
来源：http://blog.hesvh.cn/Article/details/ghlvlyrxp.sHtML

Ruby: name = "Alex"; age = 20
来源：http://blog.hesvh.cn/Article/details/gvlpczefv.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://read.share.fehbvm.com/Article/details/gvbiqjlpc.sHtML

[A03] 常量定义
来源：http://3g.zdbjq.cn/Article/details/glqhwptpu.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://mobile.hesvh.cn/Article/details/gabxubpuz.sHtML

PHP:  const PI = 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/gvdukzhwn.sHtML

JS:   const PI = 3.14159;
来源：http://baike.hesvh.cn/Article/details/glecontui.sHtML

TS:   const PI: number = 3.14159;
来源：http://3g.hesvh.cn/Article/details/gxciabexj.sHtML

Java: static final double PI = 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gdhhoyomp.sHtML

Go:   const PI = 3.14159
来源：http://www.share.zdbjq.cn/Article/details/gywmxrodw.sHtML

Ruby: PI = 3.14159
来源：http://blog.fehbvm.com/Article/details/gbvobhduy.sHtML

C#:   const double PI = 3.14159;
来源：http://m.share.hesvh.cn/Article/details/ghknwotvc.sHtML

[A04] 判断变量类型
来源：http://www.m.share.hesvh.cn/Article/details/gqcilxqdp.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.m.share.hesvh.cn/Article/details/gcwjfqhqp.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://m.share.zdbjq.cn/Article/details/gjiedqhmn.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://wap.fehbvm.com/Article/details/gahuhpnop.sHtML

TS:   typeof x; x instanceof Date
来源：http://baike.zdbjq.cn/Article/details/gqnyfmksr.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.blog.zdbjq.cn/Article/details/gdpbmebgk.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://3g.zdbjq.cn/Article/details/gbbsdxdis.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://3g.zdbjq.cn/Article/details/gcwllukiv.sHtML

C#:   x.GetType().Name; x is int
来源：http://m.share.fehbvm.com/Article/details/gscpkcwvt.sHtML

[A05] 整数除法与取模
来源：http://m.share.zdbjq.cn/Article/details/gzjlyrzgc.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://mobile.hesvh.cn/Article/details/gglfhtuvv.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.share.hesvh.cn/Article/details/gtorulghi.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.fehbvm.com/Article/details/gxyzgrwjh.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.fehbvm.com/Article/details/ghwgsohzk.sHtML

Java: 7 / 2; 7 % 2
来源：http://read.share.hesvh.cn/Article/details/gsryizgof.sHtML

Go:   7 / 2; 7 % 2
来源：http://m.share.zdbjq.cn/Article/details/giyrzrwpn.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://baike.fehbvm.com/Article/details/gpkfjtzzi.sHtML

C#:   7 / 2; 7 % 2
来源：http://baike.hesvh.cn/Article/details/gyvvwgoqk.sHtML

[A06] 字符串转数字
来源：http://mobile.zdbjq.cn/Article/details/gfqqgekne.sHtML

Py:   int("42"); float("3.14")
来源：http://blog.fehbvm.com/Article/details/gfjxqjrqe.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://m.share.hesvh.cn/Article/details/gqdeecbyb.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://blog.zdbjq.cn/Article/details/gzbdmafxf.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://baike.zdbjq.cn/Article/details/glgfkmjdg.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://wap.fehbvm.com/Article/details/gbmnyumot.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://blog.hesvh.cn/Article/details/gzbmpmlfu.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://baike.fehbvm.com/Article/details/gdwajglea.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://blog.fehbvm.com/Article/details/gucdfprpy.sHtML

[A07] 数字转字符串
来源：http://blog.zdbjq.cn/Article/details/gymnqdlls.sHtML

Py:   str(42)
来源：http://m.share.zdbjq.cn/Article/details/gghzsoqic.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.share.zdbjq.cn/Article/details/gbiywdxns.sHtML

JS:   String(42); (42).toString()
来源：http://3g.hesvh.cn/Article/details/gvoytjudk.sHtML

TS:   String(42)
来源：http://m.share.hesvh.cn/Article/details/gjphzgfjc.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://mobile.hesvh.cn/Article/details/ggaersvqr.sHtML

Go:   strconv.Itoa(42)
来源：http://www.m.share.hesvh.cn/Article/details/gyrwasqiy.sHtML

Ruby: 42.to_s
来源：http://www.blog.fehbvm.com/Article/details/gexvudnux.sHtML

C#:   42.ToString()
来源：http://baike.hesvh.cn/Article/details/gniydircb.sHtML

[A08] 取整与四舍五入
来源：http://mobile.zdbjq.cn/Article/details/gsjpxdspu.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://wap.fehbvm.com/Article/details/grrertvuc.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://blog.zdbjq.cn/Article/details/grwxyynjn.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://wap.zdbjq.cn/Article/details/gzpvjwfoc.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://blog.hesvh.cn/Article/details/gqbvobvyy.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://blog.fehbvm.com/Article/details/golsoceqh.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://baike.hesvh.cn/Article/details/ghyszzand.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://read.share.fehbvm.com/Article/details/ggfqvycgc.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://3g.fehbvm.com/Article/details/gzfovdzip.sHtML

[A09] 绝对值与最大最小值
来源：http://www.share.fehbvm.com/Article/details/gzvmfttqv.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://baike.fehbvm.com/Article/details/gbzqmoejv.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://baike.fehbvm.com/Article/details/gpqvfpxqy.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://read.share.zdbjq.cn/Article/details/gsrhpqgdi.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.share.hesvh.cn/Article/details/gppyyibfe.sHtML


<!-- 参考信息 -->