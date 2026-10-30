代发 wailian999

[U65] PHP：会话
来源：http://www.share.fanxiaobao.xyz/Article/details/gviucdyqk.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/garvuiedc.sHtML

[U66] PHP：设置 Cookie
来源：http://3g.fanxiaobao.xyz/Article/details/ggmwhpvxu.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gltvoztcq.sHtML

[U67] PHP：处理文件上传
来源：http://3g.fanxiaobao.xyz/Article/details/gjjrrcfkm.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://baike.fanxiaobao.xyz/Article/details/gizifxxxy.sHtML

[U68] PHP：PDO 连接
来源：http://wap.fanxiaobao.xyz/Article/details/grapyhkls.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mobile.fanxiaobao.xyz/Article/details/gmuxbyldz.sHtML

[U69] PHP：PDO 预处理
来源：http://3g.fanxiaobao.xyz/Article/details/ghldldltb.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.fanxiaobao.xyz/Article/details/gpgckkaln.sHtML

[U70] PHP：PDO 事务
来源：http://blog.fanxiaobao.xyz/Article/details/gxafdqnmt.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmrbnweej.sHtML

[U71] PHP：抛出异常
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwpgzcead.sHtML

throw new RuntimeException("失败", 500);
来源：http://mobile.fanxiaobao.xyz/Article/details/gbmzmjrkg.sHtML

[U72] PHP：写错误日志
来源：http://www.share.fanxiaobao.xyz/Article/details/gmccjzdrg.sHtML

error_log("失败: " . $e->getMessage());
来源：http://3g.fanxiaobao.xyz/Article/details/gfvigquzt.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.share.fanxiaobao.xyz/Article/details/gvjhdyckd.sHtML

parse_ini_file("config.ini", true)
来源：http://m.share.fanxiaobao.xyz/Article/details/gvxmhgkll.sHtML

[U74] PHP：读取环境变量
来源：http://wap.fanxiaobao.xyz/Article/details/gcwxwymtp.sHtML

getenv("APP_ENV") ?: "production"
来源：http://mobile.fanxiaobao.xyz/Article/details/gdfconzhr.sHtML

[U75] PHP：依赖注入
来源：http://www.share.fanxiaobao.xyz/Article/details/gciansbsx.sHtML

composer require psr/container
来源：http://m.share.fanxiaobao.xyz/Article/details/gwovusgrj.sHtML

[U76] PHP：简单路由
来源：http://read.share.fanxiaobao.xyz/Article/details/gwvauagnc.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://m.share.fanxiaobao.xyz/Article/details/glpnyqaom.sHtML

[U77] PHP：模板渲染
来源：http://read.share.fanxiaobao.xyz/Article/details/gfvamnazp.sHtML

composer require twig/twig
来源：http://m.share.fanxiaobao.xyz/Article/details/gkypcoytg.sHtML

[U78] PHP：单元测试
来源：http://blog.fanxiaobao.xyz/Article/details/gjpgdhbmc.sHtML

composer require --dev phpunit/phpunit
来源：http://3g.fanxiaobao.xyz/Article/details/ghlowhcqm.sHtML

[U79] PHP：静态分析
来源：http://www.share.fanxiaobao.xyz/Article/details/gelpvqlsk.sHtML

composer require --dev phpstan/phpstan
来源：http://read.share.fanxiaobao.xyz/Article/details/gscwpwjnp.sHtML

[U80] PHP：代码规范修复
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxwbluxgn.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://read.share.fanxiaobao.xyz/Article/details/graijnhab.sHtML

[U81] JS：初始化项目
来源：http://www.share.fanxiaobao.xyz/Article/details/gqxbapbvk.sHtML

npm init -y;  npm i express
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtmbyrkjh.sHtML

[U82] JS：package.json 脚本
来源：http://baike.fanxiaobao.xyz/Article/details/gboxoohjh.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mobile.fanxiaobao.xyz/Article/details/gbnzkvifu.sHtML

[U83] JS：ES Module 导入导出
来源：http://blog.fanxiaobao.xyz/Article/details/ghapcgnmy.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.share.fanxiaobao.xyz/Article/details/gtfebqzgk.sHtML

[U84] JS：CommonJS 写法
来源：http://www.blog.fanxiaobao.xyz/Article/details/guvvwywzt.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://m.share.fanxiaobao.xyz/Article/details/gvavuceki.sHtML

[U85] JS：可选链
来源：http://www.blog.fanxiaobao.xyz/Article/details/gebuksinf.sHtML

a?.b?.c
来源：http://m.share.fanxiaobao.xyz/Article/details/ghtumtyzq.sHtML

[U86] JS：空值合并
来源：http://m.share.fanxiaobao.xyz/Article/details/gpyncostj.sHtML

a ?? b
来源：http://3g.fanxiaobao.xyz/Article/details/gspgylohg.sHtML

[U87] JS：解构默认值
来源：http://www.share.fanxiaobao.xyz/Article/details/gmrqnjoki.sHtML

const { a = 1, b = 2 } = obj;
来源：http://3g.fanxiaobao.xyz/Article/details/gwrnaxmfy.sHtML

[U88] JS：对象展开合并
来源：http://mobile.fanxiaobao.xyz/Article/details/gwlwflnlr.sHtML

{ ...a, ...b }
来源：http://wap.fanxiaobao.xyz/Article/details/gvlfhqfyj.sHtML

[U89] JS：数组去重
来源：http://m.share.fanxiaobao.xyz/Article/details/gyuzpvrlv.sHtML

[...new Set(arr)]
来源：http://baike.fanxiaobao.xyz/Article/details/gawjqtlzh.sHtML

[U90] JS：数字数组排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gttgooshx.sHtML

[...arr].sort((a, b) => a - b)
来源：http://blog.fanxiaobao.xyz/Article/details/gnuymhrck.sHtML

[U91] JS：对象键值遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/geueqgttu.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzzwbzxik.sHtML

[U92] JS：深拷贝
来源：http://mobile.fanxiaobao.xyz/Article/details/gpynbwopx.sHtML

structuredClone(obj)
来源：http://mobile.fanxiaobao.xyz/Article/details/gqvvjadpj.sHtML

[U93] JS：模板字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcslxbprm.sHtML

`共 ${n} 条`
来源：http://3g.fanxiaobao.xyz/Article/details/gtwwfgxgs.sHtML

[U94] JS：箭头函数
来源：http://baike.fanxiaobao.xyz/Article/details/gmiuvffkr.sHtML

const double = x => x * 2;
来源：http://www.share.fanxiaobao.xyz/Article/details/gyiqupeit.sHtML

[U95] JS：Promise 包装
来源：http://blog.fanxiaobao.xyz/Article/details/gpmfadiwy.sHtML

new Promise((resolve, reject) => {})
来源：http://3g.fanxiaobao.xyz/Article/details/gwacbymng.sHtML

[U96] JS：async/await 与异常
来源：http://mobile.fanxiaobao.xyz/Article/details/guhenwogn.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mobile.fanxiaobao.xyz/Article/details/ghcenehnf.sHtML

[U97] JS：并发请求
来源：http://wap.fanxiaobao.xyz/Article/details/gkryyoqyy.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.fanxiaobao.xyz/Article/details/gasamyodj.sHtML

[U98] JS：fetch 带 JSON
来源：http://3g.fanxiaobao.xyz/Article/details/glvdkcieu.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.share.fanxiaobao.xyz/Article/details/gzeyfklof.sHtML

[U99] JS：事件监听
来源：http://baike.fanxiaobao.xyz/Article/details/gaszwfode.sHtML

el.addEventListener("click", e => {})
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfhefwsyb.sHtML

[U100] JS：DOM 查询
来源：http://www.blog.fanxiaobao.xyz/Article/details/glvgvdqqr.sHtML

document.querySelector(".item")
来源：http://www.share.fanxiaobao.xyz/Article/details/gjfzhmtou.sHtML

[U101] JS：classList 操作
来源：http://www.share.fanxiaobao.xyz/Article/details/gllrkgqre.sHtML

el.classList.toggle("active")
来源：http://mobile.fanxiaobao.xyz/Article/details/gzdbpeyto.sHtML

[U102] JS：本地存储
来源：http://mobile.fanxiaobao.xyz/Article/details/gyuxoousm.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxbpmgrcl.sHtML

[U103] JS：定时器
来源：http://blog.fanxiaobao.xyz/Article/details/gtbntgvjs.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blog.fanxiaobao.xyz/Article/details/gzvjfwigz.sHtML

[U104] JS：防抖
来源：http://baike.fanxiaobao.xyz/Article/details/gvxhxarbi.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fanxiaobao.xyz/Article/details/guepprymz.sHtML

[U105] JS：节流
来源：http://baike.fanxiaobao.xyz/Article/details/gvtjesfvy.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmofcodlr.sHtML

[U106] JS：日期格式化
来源：http://3g.fanxiaobao.xyz/Article/details/gmtqpuuft.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.fanxiaobao.xyz/Article/details/gewvlzebt.sHtML

[U107] JS：数字千分位
来源：http://blog.fanxiaobao.xyz/Article/details/gwtekadcs.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.fanxiaobao.xyz/Article/details/gsfwgriwk.sHtML

[U108] JS：随机整数
来源：http://m.share.fanxiaobao.xyz/Article/details/gmkccqohs.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://blog.fanxiaobao.xyz/Article/details/gfsewvirs.sHtML

[U109] JS：数组分组
来源：http://mobile.fanxiaobao.xyz/Article/details/gtdqxxlrv.sHtML

Object.groupBy(arr, x => x.type)
来源：http://read.share.fanxiaobao.xyz/Article/details/guurmjfnl.sHtML

[U110] JS：数组分块
来源：http://read.share.fanxiaobao.xyz/Article/details/gpptomyxe.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.share.fanxiaobao.xyz/Article/details/guhmkncyj.sHtML

[U111] JS：对象转 Map
来源：http://wap.fanxiaobao.xyz/Article/details/gaktckvkn.sHtML

new Map(Object.entries(obj))
来源：http://baike.fanxiaobao.xyz/Article/details/gpdephlbm.sHtML

[U112] JS：字符串补位
来源：http://mobile.fanxiaobao.xyz/Article/details/gmnzngmpa.sHtML

"7".padStart(3, "0")
来源：http://m.share.fanxiaobao.xyz/Article/details/gnzitvpms.sHtML

[U113] JS：正则替换全部
来源：http://mobile.fanxiaobao.xyz/Article/details/gsibyesux.sHtML

s.replaceAll("a", "b")
来源：http://3g.fanxiaobao.xyz/Article/details/gwcvxcceu.sHtML

[U114] JS：JSON 深比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grsmllaey.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.fanxiaobao.xyz/Article/details/gvozseafa.sHtML

[U115] JS：生成 UUID
来源：http://blog.fanxiaobao.xyz/Article/details/gqgaxgqtx.sHtML

crypto.randomUUID()
来源：http://m.share.fanxiaobao.xyz/Article/details/ghpmyouwv.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.fanxiaobao.xyz/Article/details/gguyebxps.sHtML

/** @param {string} name */ function f(name) {}
来源：http://wap.fanxiaobao.xyz/Article/details/gtenmmvqi.sHtML

[U117] JS：单元测试
来源：http://www.share.fanxiaobao.xyz/Article/details/gadodhvpm.sHtML

npm i -D vitest;  npx vitest
来源：http://www.blog.fanxiaobao.xyz/Article/details/gihqfixeq.sHtML

[U118] JS：开发服务器
来源：http://www.share.fanxiaobao.xyz/Article/details/gxisanewc.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkarvgoqa.sHtML

[U119] JS：生产构建
来源：http://baike.fanxiaobao.xyz/Article/details/gzxuyczqm.sHtML

npx vite build
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gutbalour.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkbceiuyf.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.fanxiaobao.xyz/Article/details/gjxfxgsdr.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gnsmzedos.sHtML

统计汇总
来源：http://baike.fanxiaobao.xyz/Article/details/gszhcalha.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gaenwxney.sHtML

按语言统计（条）：
来源：http://blog.fanxiaobao.xyz/Article/details/gpvxcanvs.sHtML

Python ......... 252
来源：http://3g.fanxiaobao.xyz/Article/details/guonjuyna.sHtML

PHP ............ 252
来源：http://3g.fanxiaobao.xyz/Article/details/gluzyrfeb.sHtML

JavaScript ..... 252
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqvagjmit.sHtML

TypeScript ..... 212
来源：http://read.share.fanxiaobao.xyz/Article/details/gsivzsray.sHtML

Java ........... 212
来源：http://www.share.fanxiaobao.xyz/Article/details/gcwefyuur.sHtML

Go ............. 212
来源：http://blog.fanxiaobao.xyz/Article/details/gobzfvcdk.sHtML

Ruby ........... 212
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gisbjkfvo.sHtML

C# ............. 212
来源：http://m.share.fanxiaobao.xyz/Article/details/grzzwnwgr.sHtML

C .............. 30
来源：http://wap.fanxiaobao.xyz/Article/details/gcpqbodrg.sHtML

C++ ............ 30
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvswkfmgi.sHtML

SQL ............ 90
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbxjyqnno.sHtML

Bash ........... 80
来源：http://mobile.fanxiaobao.xyz/Article/details/glnlxxfjn.sHtML

Kotlin ......... 15
来源：http://read.share.fanxiaobao.xyz/Article/details/gbuggmywc.sHtML

Swift .......... 15
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwipnpuio.sHtML

Lua ............ 10
来源：http://blog.fanxiaobao.xyz/Article/details/gdzaejwpj.sHtML

Perl ........... 10
来源：http://wap.fanxiaobao.xyz/Article/details/gxchphnyk.sHtML

Scala .......... 10
来源：http://3g.fanxiaobao.xyz/Article/details/gpcohxsyl.sHtML

------------------------------------
来源：http://3g.fanxiaobao.xyz/Article/details/ghsgvusqw.sHtML

合计 ........... 2106 条
来源：http://m.share.fanxiaobao.xyz/Article/details/ggfgjsdfm.sHtML

按章节统计：
来源：http://mobile.fanxiaobao.xyz/Article/details/gtwcuymwd.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://blog.fanxiaobao.xyz/Article/details/gtmfwgiqf.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://blog.fanxiaobao.xyz/Article/details/grhehuixm.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gthejlnaj.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mobile.fanxiaobao.xyz/Article/details/gjgdgnmxv.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://blog.fanxiaobao.xyz/Article/details/gzxljoqfk.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://blog.fanxiaobao.xyz/Article/details/grckmonzs.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.share.fanxiaobao.xyz/Article/details/gmozaffgu.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://read.share.fanxiaobao.xyz/Article/details/gkqgangjf.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://blog.fanxiaobao.xyz/Article/details/gwnqkypgy.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://3g.fanxiaobao.xyz/Article/details/gtzqwnugt.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfmdarcwm.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://read.share.fanxiaobao.xyz/Article/details/gjbnnhrio.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://3g.fanxiaobao.xyz/Article/details/gkgjuginc.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://m.share.fanxiaobao.xyz/Article/details/glyebgjrk.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://blog.fanxiaobao.xyz/Article/details/gbmsqcypn.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkaswhcfi.sHtML

Q SQL 专题                              90
来源：http://wap.fanxiaobao.xyz/Article/details/gsryblpat.sHtML

R Bash 专题                             80
来源：http://3g.fanxiaobao.xyz/Article/details/grtabaeon.sHtML

S C / C++ 专题                          60
来源：http://mobile.fanxiaobao.xyz/Article/details/goygllzts.sHtML

T 其他语言补充                          60
来源：http://mobile.fanxiaobao.xyz/Article/details/gwwrawnyn.sHtML

U 高频实用片段                         120
来源：http://3g.fanxiaobao.xyz/Article/details/gnkmnyrbd.sHtML

------------------------------------
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqijlmbus.sHtML

合计                                  2106 条
来源：http://www.share.fanxiaobao.xyz/Article/details/gzaecubxc.sHtML

--------------------------------------------------------------------------------
来源：http://blog.fanxiaobao.xyz/Article/details/gudcmnmjh.sHtML

使用提醒
来源：http://m.share.fanxiaobao.xyz/Article/details/gvjiltndg.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fanxiaobao.xyz/Article/details/gkckfywvs.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://3g.fanxiaobao.xyz/Article/details/grwzkwppj.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://m.share.fanxiaobao.xyz/Article/details/ghqhqmjcr.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mobile.fanxiaobao.xyz/Article/details/gaonfordi.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://read.share.fanxiaobao.xyz/Article/details/gbtqaunou.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://read.share.fanxiaobao.xyz/Article/details/gzoiwhnjn.sHtML

—— 文件结束 ——
来源：http://baike.fanxiaobao.xyz/Article/details/gbfodpoin.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gbfhexjds.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://baike.fanxiaobao.xyz/Article/details/galrriula.sHtML

Common Programming Examples Cheat Book
来源：http://wap.fanxiaobao.xyz/Article/details/gavaaojmu.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gitngglbx.sHtML

【收录内容】
来源：http://blog.fanxiaobao.xyz/Article/details/gtopmllfs.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://baike.fanxiaobao.xyz/Article/details/ggtsbyiyd.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://3g.fanxiaobao.xyz/Article/details/glfqiddzs.sHtML

SQL · Bash · C · C++
来源：http://3g.fanxiaobao.xyz/Article/details/ggyphsufy.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://blog.fanxiaobao.xyz/Article/details/gekscuwiy.sHtML

【使用说明】
来源：http://read.share.fanxiaobao.xyz/Article/details/gbckgljrz.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://blog.fanxiaobao.xyz/Article/details/golojimng.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gudrgvuml.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwygftiak.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://mobile.fanxiaobao.xyz/Article/details/gumgknlyw.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggzorqokq.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://read.share.fanxiaobao.xyz/Article/details/gygsoinri.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://m.share.fanxiaobao.xyz/Article/details/glgyaxvya.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://mobile.fanxiaobao.xyz/Article/details/gkhupnnfr.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://m.share.fanxiaobao.xyz/Article/details/gicqyxagf.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://mobile.fanxiaobao.xyz/Article/details/gfbssoxke.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbakflysa.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://blog.fanxiaobao.xyz/Article/details/gdqnvpkhl.sHtML

【文件统计】
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpxptaodn.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://mobile.fanxiaobao.xyz/Article/details/gotebbzwn.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnrqrizoj.sHtML

目  录
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpmotjoar.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fanxiaobao.xyz/Article/details/gcnowjtnd.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gahupgrib.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gupvqghqo.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gztzhmtwa.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gsrloguno.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/grdvxoivj.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gdkakdqrl.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gcsloebqp.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gasahykas.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://baike.fanxiaobao.xyz/Article/details/grzvtcapl.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/ggijkzyge.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gkxfpydlm.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gsaqjnxom.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gmtyourga.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gcyuspwzg.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gsdoosdvi.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/grpnksqkx.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvvwbeiwj.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gwiaywqol.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://3g.fanxiaobao.xyz/Article/details/glsekculi.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.fanxiaobao.xyz/Article/details/guwiuonwm.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/ghzrjtgbi.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gcpbmrzxl.sHtML

A. 基础语法与类型
来源：http://blog.fanxiaobao.xyz/Article/details/gyntrejkg.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gwwmejnka.sHtML

[A01] Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gldahlomt.sHtML

Py:   print("Hello, World!")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glrfpukhi.sHtML

PHP:  echo "Hello, World!";
来源：http://m.share.fanxiaobao.xyz/Article/details/gpccgcmny.sHtML

JS:   console.log("Hello, World!");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpytmhvif.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://baike.fanxiaobao.xyz/Article/details/gtnuszzoj.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzdyscoek.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://wap.fanxiaobao.xyz/Article/details/gxtlvxcxz.sHtML

Ruby: puts "Hello, World!"
来源：http://m.share.fanxiaobao.xyz/Article/details/gegmcpxem.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.share.fanxiaobao.xyz/Article/details/grfbmhfxl.sHtML

[A02] 变量声明与赋值
来源：http://wap.fanxiaobao.xyz/Article/details/gkbjtvhut.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://read.share.fanxiaobao.xyz/Article/details/gpumvsjpz.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.share.fanxiaobao.xyz/Article/details/gcrygngcf.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://wap.fanxiaobao.xyz/Article/details/ggkgoupbl.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyndihsxn.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://3g.fanxiaobao.xyz/Article/details/grqfiensy.sHtML

Go:   name := "Alex"; age := 20
来源：http://wap.fanxiaobao.xyz/Article/details/gsfgixzvs.sHtML

Ruby: name = "Alex"; age = 20
来源：http://mobile.fanxiaobao.xyz/Article/details/ghcscvzsn.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://3g.fanxiaobao.xyz/Article/details/gaulkworx.sHtML

[A03] 常量定义
来源：http://mobile.fanxiaobao.xyz/Article/details/gqorsrprc.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://3g.fanxiaobao.xyz/Article/details/gengawqlr.sHtML

PHP:  const PI = 3.14159;
来源：http://3g.fanxiaobao.xyz/Article/details/gzikycbwk.sHtML

JS:   const PI = 3.14159;
来源：http://read.share.fanxiaobao.xyz/Article/details/gbszfipkf.sHtML

TS:   const PI: number = 3.14159;
来源：http://baike.fanxiaobao.xyz/Article/details/gwarguzoh.sHtML

Java: static final double PI = 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnvladyej.sHtML

Go:   const PI = 3.14159
来源：http://read.share.fanxiaobao.xyz/Article/details/gnbihvzfi.sHtML

Ruby: PI = 3.14159
来源：http://blog.fanxiaobao.xyz/Article/details/gsabukcea.sHtML

C#:   const double PI = 3.14159;
来源：http://www.share.fanxiaobao.xyz/Article/details/gacbefqie.sHtML

[A04] 判断变量类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqwhjygre.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.blog.fanxiaobao.xyz/Article/details/geclkskvn.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://blog.fanxiaobao.xyz/Article/details/gkgqeybru.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://m.share.fanxiaobao.xyz/Article/details/gsfkusvto.sHtML

TS:   typeof x; x instanceof Date
来源：http://blog.fanxiaobao.xyz/Article/details/gxxlklxid.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://blog.fanxiaobao.xyz/Article/details/gqgcbxugr.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://baike.fanxiaobao.xyz/Article/details/gnbieoewb.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://wap.fanxiaobao.xyz/Article/details/gajcitiwb.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gthkshxxs.sHtML

[A05] 整数除法与取模
来源：http://m.share.fanxiaobao.xyz/Article/details/gyhazuyli.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://mobile.fanxiaobao.xyz/Article/details/gjvspyvfb.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://wap.fanxiaobao.xyz/Article/details/gugdhlfps.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjeohskrr.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gejfzhbyh.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcapulkqa.sHtML

Go:   7 / 2; 7 % 2
来源：http://mobile.fanxiaobao.xyz/Article/details/grnpczytn.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://baike.fanxiaobao.xyz/Article/details/ggfmenjrk.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gjqlviqbx.sHtML

[A06] 字符串转数字
来源：http://mobile.fanxiaobao.xyz/Article/details/gfhetcfqc.sHtML

Py:   int("42"); float("3.14")
来源：http://www.share.fanxiaobao.xyz/Article/details/ghjevgegh.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://read.share.fanxiaobao.xyz/Article/details/gtrmcgjsv.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://mobile.fanxiaobao.xyz/Article/details/gustwgxst.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.share.fanxiaobao.xyz/Article/details/gahqrgwgz.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://m.share.fanxiaobao.xyz/Article/details/gvzexyyey.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://read.share.fanxiaobao.xyz/Article/details/gbuhzopkq.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.share.fanxiaobao.xyz/Article/details/gakwloofx.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://blog.fanxiaobao.xyz/Article/details/gnsqzcooe.sHtML

[A07] 数字转字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gkizellya.sHtML

Py:   str(42)
来源：http://m.share.fanxiaobao.xyz/Article/details/gpkgalpjj.sHtML

PHP:  (string) 42; strval(42)
来源：http://m.share.fanxiaobao.xyz/Article/details/ghteplqsq.sHtML

JS:   String(42); (42).toString()
来源：http://3g.fanxiaobao.xyz/Article/details/geszjqynl.sHtML

TS:   String(42)
来源：http://m.share.fanxiaobao.xyz/Article/details/gyfwafamc.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://wap.fanxiaobao.xyz/Article/details/gxtbxziqv.sHtML

Go:   strconv.Itoa(42)
来源：http://3g.fanxiaobao.xyz/Article/details/gevwgmkjh.sHtML

Ruby: 42.to_s
来源：http://baike.fanxiaobao.xyz/Article/details/gftwxlzvv.sHtML

C#:   42.ToString()
来源：http://read.share.fanxiaobao.xyz/Article/details/giclugtyw.sHtML

[A08] 取整与四舍五入
来源：http://wap.fanxiaobao.xyz/Article/details/gdjgqzhde.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giaubeqyn.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjgjsejdp.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://mobile.fanxiaobao.xyz/Article/details/ganckgwhc.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://m.share.fanxiaobao.xyz/Article/details/gpzpgivce.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.share.fanxiaobao.xyz/Article/details/gcbqrzmaq.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://mobile.fanxiaobao.xyz/Article/details/guugyvkyn.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdkjedhle.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://mobile.fanxiaobao.xyz/Article/details/gqbjbyfaq.sHtML

[A09] 绝对值与最大最小值
来源：http://wap.fanxiaobao.xyz/Article/details/glgwbhuim.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gvaackrju.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gtuhgksjc.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gezitovnm.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://blog.fanxiaobao.xyz/Article/details/gicxirkdc.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://3g.fanxiaobao.xyz/Article/details/guzfepbox.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.blog.fanxiaobao.xyz/Article/details/giekolcfw.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://read.share.fanxiaobao.xyz/Article/details/gtmyujxut.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/glcosqpke.sHtML


<!-- 参考信息 -->