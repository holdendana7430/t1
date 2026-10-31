代发 wailian999

[U57] PHP：字符串插值
来源：http://yd.bookmarksfly.cn

"值: {$a}"
来源：http://fk.shtwfgs.cn

[U58] PHP：数组三件套
来源：http://cq.chemitech.net.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://zd.haigaiapp.cn

[U59] PHP：自定义排序
来源：http://wk.shxzukj.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mv.muxihuayi.cn

[U60] PHP：JSON 编解码
来源：http://gf.szsharing.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://dq.nszjky.cn

[U61] PHP：正则
来源：http://qf.nicolike.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wb.hahajie.cn

[U62] PHP：日期对象
来源：http://qd.shxzskj.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ud.yuntaijiaju.cn

[U63] PHP：文件读写
来源：http://qo.yuexingan06.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ps.gzmigu.cn

[U64] PHP：目录遍历
来源：http://le.huixiangedu.cn

glob("dir/*.php");  scandir("dir");
来源：http://ax.lnxyls.cn

[U65] PHP：会话
来源：http://wv.huixiangedu.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://mf.521024.cn

[U66] PHP：设置 Cookie
来源：http://jb.wgjwhj.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ck.haigaiapp.cn

[U67] PHP：处理文件上传
来源：http://wp.9csxet.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://vf.colortex.cn

[U68] PHP：PDO 连接
来源：http://hf.newstarts.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://iq.szxytkj.cn

[U69] PHP：PDO 预处理
来源：http://fj.huanxung.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mm.bjjhwx.cn

[U70] PHP：PDO 事务
来源：http://ke.jianghongdianzi.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://sa.hnjuh.cn

[U71] PHP：抛出异常
来源：http://vp.bjjhwx.cn

throw new RuntimeException("失败", 500);
来源：http://gy.bjjhwx.cn

[U72] PHP：写错误日志
来源：http://jm.bookmarksfly.cn

error_log("失败: " . $e->getMessage());
来源：http://kv.yuexingan06.cn

[U73] PHP：读取 ini 配置
来源：http://ps.muxihuayi.cn

parse_ini_file("config.ini", true)
来源：http://is.gzmigu.cn

[U74] PHP：读取环境变量
来源：http://ap.huanxung.cn

getenv("APP_ENV") ?: "production"
来源：http://zm.gzmigu.cn

[U75] PHP：依赖注入
来源：http://mh.chemitech.net.cn

composer require psr/container
来源：http://rr.yuexingan06.cn

[U76] PHP：简单路由
来源：http://aq.hahajie.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.huixiangedu.cn

[U77] PHP：模板渲染
来源：http://ua.jctech888.com.cn

composer require twig/twig
来源：http://qu.yuexingan06.cn

[U78] PHP：单元测试
来源：http://mz.hnjuh.cn

composer require --dev phpunit/phpunit
来源：http://jb.jctech888.com.cn

[U79] PHP：静态分析
来源：http://pc.shxzskj.cn

composer require --dev phpstan/phpstan
来源：http://jr.521024.cn

[U80] PHP：代码规范修复
来源：http://ye.yuexingan06.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://hd.wgjwhj.cn

[U81] JS：初始化项目
来源：http://jv.521024.cn

npm init -y;  npm i express
来源：http://vd.lnxyls.cn

[U82] JS：package.json 脚本
来源：http://hd.szxytkj.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://fs.shxzukj.cn

[U83] JS：ES Module 导入导出
来源：http://qg.nicolike.cn

export const a = 1;  import { a } from "./m.js";
来源：http://ud.szxytkj.cn

[U84] JS：CommonJS 写法
来源：http://qt.gzmigu.cn

module.exports = { a };  const { a } = require("./m");
来源：http://nf.shtwfgs.cn

[U85] JS：可选链
来源：http://tp.wgjwhj.cn

a?.b?.c
来源：http://us.shxzukj.cn

[U86] JS：空值合并
来源：http://vw.huanxung.cn

a ?? b
来源：http://rx.hahajie.cn

[U87] JS：解构默认值
来源：http://ny.haigaiapp.cn

const { a = 1, b = 2 } = obj;
来源：http://qy.muxihuayi.cn

[U88] JS：对象展开合并
来源：http://vl.yuexingan06.cn

{ ...a, ...b }
来源：http://gg.yuntaijiaju.cn

[U89] JS：数组去重
来源：http://hn.muxihuayi.cn

[...new Set(arr)]
来源：http://ru.panjiajie.cn

[U90] JS：数字数组排序
来源：http://cx.shxzukj.cn

[...arr].sort((a, b) => a - b)
来源：http://es.9csxet.cn

[U91] JS：对象键值遍历
来源：http://kz.shxzskj.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ye.jctech888.com.cn

[U92] JS：深拷贝
来源：http://bq.hahajie.cn

structuredClone(obj)
来源：http://bv.asd995.cn

[U93] JS：模板字符串
来源：http://hf.yuexingan06.cn

`共 ${n} 条`
来源：http://af.newstarts.cn

[U94] JS：箭头函数
来源：http://nh.shxzskj.cn

const double = x => x * 2;
来源：http://un.huixiangedu.cn

[U95] JS：Promise 包装
来源：http://hq.shtwfgs.cn

new Promise((resolve, reject) => {})
来源：http://gi.9csxet.cn

[U96] JS：async/await 与异常
来源：http://ya.jctech888.com.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://kh.yuntaijiaju.cn

[U97] JS：并发请求
来源：http://kl.haigaiapp.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://ot.gzmigu.cn

[U98] JS：fetch 带 JSON
来源：http://ag.shxzskj.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://nx.muxihuayi.cn

[U99] JS：事件监听
来源：http://yz.asd995.cn

el.addEventListener("click", e => {})
来源：http://hg.chemitech.net.cn

[U100] JS：DOM 查询
来源：http://in.bookmarksfly.cn

document.querySelector(".item")
来源：http://iu.huanxung.cn

[U101] JS：classList 操作
来源：http://mh.shxzskj.cn

el.classList.toggle("active")
来源：http://hq.wgjwhj.cn

[U102] JS：本地存储
来源：http://ha.huanxung.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://qz.szxytkj.cn

[U103] JS：定时器
来源：http://xg.szsharing.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://nm.muxihuayi.cn

[U104] JS：防抖
来源：http://ms.521024.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://aa.asd995.cn

[U105] JS：节流
来源：http://mz.wgjwhj.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://qv.huixinmuqiang.cn

[U106] JS：日期格式化
来源：http://ej.huanxung.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://rk.newstarts.cn

[U107] JS：数字千分位
来源：http://fx.chemitech.net.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://fk.szxytkj.cn

[U108] JS：随机整数
来源：http://qq.muxihuayi.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://cg.nicolike.cn

[U109] JS：数组分组
来源：http://vi.jctech888.com.cn

Object.groupBy(arr, x => x.type)
来源：http://st.yuexingan06.cn

[U110] JS：数组分块
来源：http://lv.hnjuh.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://dt.haigaiapp.cn

[U111] JS：对象转 Map
来源：http://ee.lnxyls.cn

new Map(Object.entries(obj))
来源：http://ye.yuexingan06.cn

[U112] JS：字符串补位
来源：http://bp.hahajie.cn

"7".padStart(3, "0")
来源：http://tx.shxzskj.cn

[U113] JS：正则替换全部
来源：http://zt.nszjky.cn

s.replaceAll("a", "b")
来源：http://po.yuntaijiaju.cn

[U114] JS：JSON 深比较
来源：http://yn.shtwfgs.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://jj.haigaiapp.cn

[U115] JS：生成 UUID
来源：http://ha.newstarts.cn

crypto.randomUUID()
来源：http://ky.panjiajie.cn

[U116] JS：类型检查（JSDoc）
来源：http://ze.bjjhwx.cn

/** @param {string} name */ function f(name) {}
来源：http://lw.haigaiapp.cn

[U117] JS：单元测试
来源：http://ba.hahajie.cn

npm i -D vitest;  npx vitest
来源：http://qz.huixiangedu.cn

[U118] JS：开发服务器
来源：http://nk.yuexingan06.cn

npm i -D vite;  npx vite
来源：http://zh.szxytkj.cn

[U119] JS：生产构建
来源：http://gz.panjiajie.cn

npx vite build
来源：http://lr.lnxyls.cn

[U120] JS：读取环境变量（Vite）
来源：http://bx.huixiangedu.cn

import.meta.env.VITE_API_URL
来源：http://qd.lnxyls.cn

================================================================================
来源：http://wf.yuntaijiaju.cn

统计汇总
来源：http://sr.jctech888.com.cn

================================================================================
来源：http://vb.nszjky.cn

按语言统计（条）：
来源：http://fa.panjiajie.cn

Python ......... 252
来源：http://br.bookmarksfly.cn

PHP ............ 252
来源：http://un.haigaiapp.cn

JavaScript ..... 252
来源：http://ba.shtwfgs.cn

TypeScript ..... 212
来源：http://cr.hahajie.cn

Java ........... 212
来源：http://ps.jianghongdianzi.cn

Go ............. 212
来源：http://ed.muxihuayi.cn

Ruby ........... 212
来源：http://wj.huixinmuqiang.cn

C# ............. 212
来源：http://af.yuntaijiaju.cn

C .............. 30
来源：http://rx.newstarts.cn

C++ ............ 30
来源：http://hc.bookmarksfly.cn

SQL ............ 90
来源：http://zu.gzmigu.cn

Bash ........... 80
来源：http://yl.521024.cn

Kotlin ......... 15
来源：http://iz.szxytkj.cn

Swift .......... 15
来源：http://qs.hahajie.cn

Lua ............ 10
来源：http://et.colortex.cn

Perl ........... 10
来源：http://un.szxytkj.cn

Scala .......... 10
来源：http://jk.haigaiapp.cn

------------------------------------
来源：http://zz.yuntaijiaju.cn

合计 ........... 2106 条
来源：http://ew.huixinmuqiang.cn

按章节统计：
来源：http://fj.jctech888.com.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://tk.yuexingan06.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ob.yuexingan06.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://vy.wgjwhj.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://iv.gzmigu.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://dy.wgjwhj.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://vv.chemitech.net.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://dw.wgjwhj.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://lr.chemitech.net.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://on.shxzskj.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://bn.nszjky.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://vx.muxihuayi.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://dq.hahajie.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://bs.521024.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://al.gzmigu.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://sr.huanxung.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://yn.chemitech.net.cn

Q SQL 专题                              90
来源：http://od.521024.cn

R Bash 专题                             80
来源：http://qp.huixiangedu.cn

S C / C++ 专题                          60
来源：http://on.yuexingan06.cn

T 其他语言补充                          60
来源：http://lz.jianghongdianzi.cn

U 高频实用片段                         120
来源：http://fl.huixinmuqiang.cn

------------------------------------
来源：http://ww.lnxyls.cn

合计                                  2106 条
来源：http://wu.bjjhwx.cn

--------------------------------------------------------------------------------
来源：http://at.yuntaijiaju.cn

使用提醒
来源：http://fx.hnjuh.cn

--------------------------------------------------------------------------------
来源：http://ud.chemitech.net.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ev.shtwfgs.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wt.newstarts.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hl.haigaiapp.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://uo.chemitech.net.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://qr.hnjuh.cn

—— 文件结束 ——
来源：http://zm.shtwfgs.cn

================================================================================
来源：http://qe.lnxyls.cn

程序语言常见例子速查手册（2024 版）
来源：http://cu.hnjuh.cn

Common Programming Examples Cheat Book
来源：http://dt.chemitech.net.cn

================================================================================
来源：http://zu.yuntaijiaju.cn

【收录内容】
来源：http://qr.521024.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://cw.jianghongdianzi.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://md.nszjky.cn

SQL · Bash · C · C++
来源：http://io.hnjuh.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://mn.jctech888.com.cn

【使用说明】
来源：http://ln.gzmigu.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://pd.colortex.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://cl.yuexingan06.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ta.huixinmuqiang.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://yv.haigaiapp.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://tb.shtwfgs.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://xp.muxihuayi.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://uv.chemitech.net.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ic.haigaiapp.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://tf.lnxyls.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ip.gzmigu.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://dd.muxihuayi.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ez.chemitech.net.cn

【文件统计】
来源：http://hg.shtwfgs.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ds.panjiajie.cn

--------------------------------------------------------------------------------
来源：http://ob.huixinmuqiang.cn

目  录
来源：http://wl.hnjuh.cn

--------------------------------------------------------------------------------
来源：http://ha.colortex.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://it.jctech888.com.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://sf.panjiajie.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://ui.shxzskj.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ed.muxihuayi.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://dm.colortex.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://rl.nszjky.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://ty.szxytkj.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://vl.hahajie.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ae.hnjuh.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://cb.huixinmuqiang.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://si.huanxung.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://uv.szxytkj.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://pt.colortex.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://zh.bookmarksfly.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://zp.yuexingan06.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://vc.lnxyls.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ny.bookmarksfly.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://fb.nszjky.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://lx.nszjky.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://rv.521024.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mo.shxzskj.cn

================================================================================
来源：http://ij.muxihuayi.cn

A. 基础语法与类型
来源：http://yb.haigaiapp.cn

================================================================================
来源：http://rf.wgjwhj.cn

[A01] Hello World
来源：http://gf.szxytkj.cn

Py:   print("Hello, World!")
来源：http://bt.szsharing.cn

PHP:  echo "Hello, World!";
来源：http://pm.jianghongdianzi.cn

JS:   console.log("Hello, World!");
来源：http://gs.huixiangedu.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://mi.jctech888.com.cn

Java: System.out.println("Hello, World!");
来源：http://rh.huixiangedu.cn

Go:   fmt.Println("Hello, World!")
来源：http://ah.muxihuayi.cn

Ruby: puts "Hello, World!"
来源：http://ct.huixiangedu.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://ml.jctech888.com.cn

[A02] 变量声明与赋值
来源：http://ty.gzmigu.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://oy.lnxyls.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://ag.shxzukj.cn

JS:   let name = "Alex"; const age = 20;
来源：http://ll.shxzukj.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://dp.haigaiapp.cn

Java: String name = "Alex"; int age = 20;
来源：http://zz.shxzskj.cn

Go:   name := "Alex"; age := 20
来源：http://it.gzmigu.cn

Ruby: name = "Alex"; age = 20
来源：http://hx.szxytkj.cn

C#:   string name = "Alex"; int age = 20;
来源：http://ah.szxytkj.cn

[A03] 常量定义
来源：http://ue.yuntaijiaju.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://bk.jianghongdianzi.cn

PHP:  const PI = 3.14159;
来源：http://eo.haigaiapp.cn

JS:   const PI = 3.14159;
来源：http://ut.huixiangedu.cn

TS:   const PI: number = 3.14159;
来源：http://wt.lnxyls.cn

Java: static final double PI = 3.14159;
来源：http://nw.huixiangedu.cn

Go:   const PI = 3.14159
来源：http://jb.shtwfgs.cn

Ruby: PI = 3.14159
来源：http://vp.shtwfgs.cn

C#:   const double PI = 3.14159;
来源：http://cn.shxzskj.cn

[A04] 判断变量类型
来源：http://kp.huixiangedu.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://ur.nicolike.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://sc.9csxet.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://yt.colortex.cn

TS:   typeof x; x instanceof Date
来源：http://kt.wgjwhj.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://tj.colortex.cn

Go:   reflect.TypeOf(x).Name()
来源：http://bu.newstarts.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://gw.yuntaijiaju.cn

C#:   x.GetType().Name; x is int
来源：http://kj.521024.cn

[A05] 整数除法与取模
来源：http://mr.hahajie.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ax.yuntaijiaju.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://hy.panjiajie.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://cb.bjjhwx.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://pz.nicolike.cn

Java: 7 / 2; 7 % 2
来源：http://ad.lnxyls.cn

Go:   7 / 2; 7 % 2
来源：http://ck.hahajie.cn

Ruby: 7 / 2; 7 % 2
来源：http://wr.shtwfgs.cn

C#:   7 / 2; 7 % 2
来源：http://lz.wgjwhj.cn

[A06] 字符串转数字
来源：http://oe.bookmarksfly.cn

Py:   int("42"); float("3.14")
来源：http://hg.hnjuh.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ua.colortex.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://tf.shxzukj.cn

TS:   parseInt("42", 10); Number("42")
来源：http://ws.lnxyls.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://md.szxytkj.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ph.colortex.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://eq.bookmarksfly.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://dq.521024.cn

[A07] 数字转字符串
来源：http://da.gzmigu.cn

Py:   str(42)
来源：http://dc.jctech888.com.cn

PHP:  (string) 42; strval(42)
来源：http://ml.colortex.cn

JS:   String(42); (42).toString()
来源：http://dp.hnjuh.cn

TS:   String(42)
来源：http://ne.panjiajie.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://mn.shxzukj.cn

Go:   strconv.Itoa(42)
来源：http://ld.bjjhwx.cn

Ruby: 42.to_s
来源：http://hz.asd995.cn

C#:   42.ToString()
来源：http://nj.9csxet.cn

[A08] 取整与四舍五入
来源：http://nk.nicolike.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hc.szxytkj.cn


<!-- 参考信息 -->