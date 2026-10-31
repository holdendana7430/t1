代发 wailian999

[U59] PHP：自定义排序
来源：http://df.yuexingan06.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://jq.shxzskj.cn

[U60] PHP：JSON 编解码
来源：http://va.colortex.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://km.szxytkj.cn

[U61] PHP：正则
来源：http://pq.hahajie.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://eg.yuexingan06.cn

[U62] PHP：日期对象
来源：http://su.bookmarksfly.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://nz.newstarts.cn

[U63] PHP：文件读写
来源：http://tm.yuntaijiaju.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ls.yuexingan06.cn

[U64] PHP：目录遍历
来源：http://ij.nszjky.cn

glob("dir/*.php");  scandir("dir");
来源：http://uc.szxytkj.cn

[U65] PHP：会话
来源：http://vs.shxzukj.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://pr.yuexingan06.cn

[U66] PHP：设置 Cookie
来源：http://ja.nszjky.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mi.yuexingan06.cn

[U67] PHP：处理文件上传
来源：http://fn.jctech888.com.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://yn.szxytkj.cn

[U68] PHP：PDO 连接
来源：http://ih.yuntaijiaju.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ae.asd995.cn

[U69] PHP：PDO 预处理
来源：http://ff.shxzskj.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://de.hnjuh.cn

[U70] PHP：PDO 事务
来源：http://it.shxzskj.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://bp.szxytkj.cn

[U71] PHP：抛出异常
来源：http://ak.yuexingan06.cn

throw new RuntimeException("失败", 500);
来源：http://pj.shxzukj.cn

[U72] PHP：写错误日志
来源：http://un.shtwfgs.cn

error_log("失败: " . $e->getMessage());
来源：http://hy.bjjhwx.cn

[U73] PHP：读取 ini 配置
来源：http://jw.chemitech.net.cn

parse_ini_file("config.ini", true)
来源：http://kr.nicolike.cn

[U74] PHP：读取环境变量
来源：http://of.panjiajie.cn

getenv("APP_ENV") ?: "production"
来源：http://vh.szxytkj.cn

[U75] PHP：依赖注入
来源：http://zv.shxzskj.cn

composer require psr/container
来源：http://rd.panjiajie.cn

[U76] PHP：简单路由
来源：http://ji.shtwfgs.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ig.521024.cn

[U77] PHP：模板渲染
来源：http://md.bjjhwx.cn

composer require twig/twig
来源：http://fd.wgjwhj.cn

[U78] PHP：单元测试
来源：http://zi.panjiajie.cn

composer require --dev phpunit/phpunit
来源：http://oi.muxihuayi.cn

[U79] PHP：静态分析
来源：http://yu.521024.cn

composer require --dev phpstan/phpstan
来源：http://es.yuexingan06.cn

[U80] PHP：代码规范修复
来源：http://us.lnxyls.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://so.lnxyls.cn

[U81] JS：初始化项目
来源：http://he.asd995.cn

npm init -y;  npm i express
来源：http://wh.gzmigu.cn

[U82] JS：package.json 脚本
来源：http://pp.huanxung.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://oo.szsharing.cn

[U83] JS：ES Module 导入导出
来源：http://ti.9csxet.cn

export const a = 1;  import { a } from "./m.js";
来源：http://pa.hahajie.cn

[U84] JS：CommonJS 写法
来源：http://er.shtwfgs.cn

module.exports = { a };  const { a } = require("./m");
来源：http://bp.hnjuh.cn

[U85] JS：可选链
来源：http://ps.jctech888.com.cn

a?.b?.c
来源：http://dm.hahajie.cn

[U86] JS：空值合并
来源：http://yn.bookmarksfly.cn

a ?? b
来源：http://iz.bjjhwx.cn

[U87] JS：解构默认值
来源：http://ny.shtwfgs.cn

const { a = 1, b = 2 } = obj;
来源：http://bl.panjiajie.cn

[U88] JS：对象展开合并
来源：http://if.9csxet.cn

{ ...a, ...b }
来源：http://rq.yuexingan06.cn

[U89] JS：数组去重
来源：http://vc.huanxung.cn

[...new Set(arr)]
来源：http://ba.hahajie.cn

[U90] JS：数字数组排序
来源：http://mr.huixiangedu.cn

[...arr].sort((a, b) => a - b)
来源：http://og.colortex.cn

[U91] JS：对象键值遍历
来源：http://oc.jianghongdianzi.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://yl.colortex.cn

[U92] JS：深拷贝
来源：http://dn.hnjuh.cn

structuredClone(obj)
来源：http://zv.jianghongdianzi.cn

[U93] JS：模板字符串
来源：http://uy.nicolike.cn

`共 ${n} 条`
来源：http://zn.panjiajie.cn

[U94] JS：箭头函数
来源：http://ur.nicolike.cn

const double = x => x * 2;
来源：http://kq.gzmigu.cn

[U95] JS：Promise 包装
来源：http://of.colortex.cn

new Promise((resolve, reject) => {})
来源：http://kq.wgjwhj.cn

[U96] JS：async/await 与异常
来源：http://ev.panjiajie.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://uc.asd995.cn

[U97] JS：并发请求
来源：http://ed.yuntaijiaju.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://ct.szsharing.cn

[U98] JS：fetch 带 JSON
来源：http://np.newstarts.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mc.colortex.cn

[U99] JS：事件监听
来源：http://qx.shtwfgs.cn

el.addEventListener("click", e => {})
来源：http://go.jianghongdianzi.cn

[U100] JS：DOM 查询
来源：http://oo.shxzukj.cn

document.querySelector(".item")
来源：http://in.wgjwhj.cn

[U101] JS：classList 操作
来源：http://ql.gzmigu.cn

el.classList.toggle("active")
来源：http://jd.yuexingan06.cn

[U102] JS：本地存储
来源：http://sr.nszjky.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://fr.shtwfgs.cn

[U103] JS：定时器
来源：http://lr.nicolike.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://fw.yuexingan06.cn

[U104] JS：防抖
来源：http://kx.newstarts.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ny.szsharing.cn

[U105] JS：节流
来源：http://xi.bjjhwx.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ph.521024.cn

[U106] JS：日期格式化
来源：http://du.hahajie.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://cu.jianghongdianzi.cn

[U107] JS：数字千分位
来源：http://kx.chemitech.net.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hs.szsharing.cn

[U108] JS：随机整数
来源：http://cf.chemitech.net.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://qv.hahajie.cn

[U109] JS：数组分组
来源：http://nu.9csxet.cn

Object.groupBy(arr, x => x.type)
来源：http://ui.jctech888.com.cn

[U110] JS：数组分块
来源：http://ur.jctech888.com.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://bh.jianghongdianzi.cn

[U111] JS：对象转 Map
来源：http://zz.521024.cn

new Map(Object.entries(obj))
来源：http://zl.521024.cn

[U112] JS：字符串补位
来源：http://vr.9csxet.cn

"7".padStart(3, "0")
来源：http://op.nicolike.cn

[U113] JS：正则替换全部
来源：http://ym.haigaiapp.cn

s.replaceAll("a", "b")
来源：http://ze.gzmigu.cn

[U114] JS：JSON 深比较
来源：http://ps.hnjuh.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://iw.chemitech.net.cn

[U115] JS：生成 UUID
来源：http://ey.panjiajie.cn

crypto.randomUUID()
来源：http://ez.gzmigu.cn

[U116] JS：类型检查（JSDoc）
来源：http://mj.hahajie.cn

/** @param {string} name */ function f(name) {}
来源：http://nz.shxzskj.cn

[U117] JS：单元测试
来源：http://nv.huixinmuqiang.cn

npm i -D vitest;  npx vitest
来源：http://oq.huixiangedu.cn

[U118] JS：开发服务器
来源：http://ep.wgjwhj.cn

npm i -D vite;  npx vite
来源：http://hv.hahajie.cn

[U119] JS：生产构建
来源：http://wl.nszjky.cn

npx vite build
来源：http://tg.hnjuh.cn

[U120] JS：读取环境变量（Vite）
来源：http://lm.nszjky.cn

import.meta.env.VITE_API_URL
来源：http://fh.asd995.cn

================================================================================
来源：http://nf.jianghongdianzi.cn

统计汇总
来源：http://gb.panjiajie.cn

================================================================================
来源：http://wm.9csxet.cn

按语言统计（条）：
来源：http://yq.yuntaijiaju.cn

Python ......... 252
来源：http://av.521024.cn

PHP ............ 252
来源：http://eb.nszjky.cn

JavaScript ..... 252
来源：http://ku.huixiangedu.cn

TypeScript ..... 212
来源：http://gl.haigaiapp.cn

Java ........... 212
来源：http://nx.huanxung.cn

Go ............. 212
来源：http://wv.521024.cn

Ruby ........... 212
来源：http://au.jctech888.com.cn

C# ............. 212
来源：http://zp.nszjky.cn

C .............. 30
来源：http://js.huanxung.cn

C++ ............ 30
来源：http://je.muxihuayi.cn

SQL ............ 90
来源：http://jz.huixinmuqiang.cn

Bash ........... 80
来源：http://ql.yuntaijiaju.cn

Kotlin ......... 15
来源：http://jc.hahajie.cn

Swift .......... 15
来源：http://pu.colortex.cn

Lua ............ 10
来源：http://ws.huixiangedu.cn

Perl ........... 10
来源：http://tb.bookmarksfly.cn

Scala .......... 10
来源：http://ed.huanxung.cn

------------------------------------
来源：http://ks.nicolike.cn

合计 ........... 2106 条
来源：http://dw.hnjuh.cn

按章节统计：
来源：http://ll.shxzskj.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://tk.huixinmuqiang.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://rx.huixinmuqiang.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://fg.asd995.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wj.521024.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ve.shxzskj.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ly.szxytkj.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://zu.wgjwhj.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://gf.shxzskj.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://za.szsharing.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://re.muxihuayi.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://bw.asd995.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ff.shxzukj.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://xt.huixinmuqiang.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://qk.hahajie.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://pd.nszjky.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://bt.9csxet.cn

Q SQL 专题                              90
来源：http://ks.newstarts.cn

R Bash 专题                             80
来源：http://kp.haigaiapp.cn

S C / C++ 专题                          60
来源：http://er.9csxet.cn

T 其他语言补充                          60
来源：http://fa.haigaiapp.cn

U 高频实用片段                         120
来源：http://tj.shxzukj.cn

------------------------------------
来源：http://je.bookmarksfly.cn

合计                                  2106 条
来源：http://im.shxzukj.cn

--------------------------------------------------------------------------------
来源：http://rb.hnjuh.cn

使用提醒
来源：http://ws.jianghongdianzi.cn

--------------------------------------------------------------------------------
来源：http://vg.szxytkj.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ij.newstarts.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://lw.bjjhwx.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://fw.hahajie.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://lc.huixiangedu.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://nq.haigaiapp.cn

—— 文件结束 ——
来源：http://it.colortex.cn

================================================================================
来源：http://xk.bjjhwx.cn

程序语言常见例子速查手册（2024 版）
来源：http://go.shtwfgs.cn

Common Programming Examples Cheat Book
来源：http://rd.wgjwhj.cn

================================================================================
来源：http://nt.colortex.cn

【收录内容】
来源：http://mr.shtwfgs.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://rs.huixinmuqiang.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://oz.huixinmuqiang.cn

SQL · Bash · C · C++
来源：http://ar.gzmigu.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://dv.yuexingan06.cn

【使用说明】
来源：http://md.colortex.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ez.hahajie.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://jr.lnxyls.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://io.9csxet.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://wz.gzmigu.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://lb.panjiajie.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://rr.lnxyls.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://oc.yuexingan06.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ak.huanxung.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ac.panjiajie.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hp.yuntaijiaju.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://wm.muxihuayi.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://oq.asd995.cn

【文件统计】
来源：http://cd.chemitech.net.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://sl.nicolike.cn

--------------------------------------------------------------------------------
来源：http://dt.9csxet.cn

目  录
来源：http://jo.colortex.cn

--------------------------------------------------------------------------------
来源：http://yj.muxihuayi.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ai.asd995.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://mk.shxzskj.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://tc.gzmigu.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://yb.lnxyls.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://so.haigaiapp.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://ha.haigaiapp.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://bq.shxzukj.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ev.colortex.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://nl.nszjky.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://vn.shxzukj.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://og.panjiajie.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://dz.huanxung.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://is.jianghongdianzi.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://lf.huixinmuqiang.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://wi.asd995.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://jv.newstarts.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://uf.haigaiapp.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://ph.hahajie.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://vd.szxytkj.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://vd.haigaiapp.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://ab.yuntaijiaju.cn

================================================================================
来源：http://jg.bjjhwx.cn

A. 基础语法与类型
来源：http://tb.muxihuayi.cn

================================================================================
来源：http://nb.muxihuayi.cn

[A01] Hello World
来源：http://gw.jianghongdianzi.cn

Py:   print("Hello, World!")
来源：http://zv.bookmarksfly.cn

PHP:  echo "Hello, World!";
来源：http://ub.asd995.cn

JS:   console.log("Hello, World!");
来源：http://dy.colortex.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://pv.jianghongdianzi.cn

Java: System.out.println("Hello, World!");
来源：http://bg.shxzskj.cn

Go:   fmt.Println("Hello, World!")
来源：http://xn.shxzskj.cn

Ruby: puts "Hello, World!"
来源：http://yt.gzmigu.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://nt.lnxyls.cn

[A02] 变量声明与赋值
来源：http://mw.lnxyls.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://jb.nszjky.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://uo.shxzskj.cn

JS:   let name = "Alex"; const age = 20;
来源：http://ws.hnjuh.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://wz.9csxet.cn

Java: String name = "Alex"; int age = 20;
来源：http://ly.nicolike.cn

Go:   name := "Alex"; age := 20
来源：http://ci.9csxet.cn

Ruby: name = "Alex"; age = 20
来源：http://or.colortex.cn

C#:   string name = "Alex"; int age = 20;
来源：http://nj.szxytkj.cn

[A03] 常量定义
来源：http://zp.asd995.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://wq.jianghongdianzi.cn

PHP:  const PI = 3.14159;
来源：http://pz.szsharing.cn

JS:   const PI = 3.14159;
来源：http://mt.shtwfgs.cn

TS:   const PI: number = 3.14159;
来源：http://td.panjiajie.cn

Java: static final double PI = 3.14159;
来源：http://mm.wgjwhj.cn

Go:   const PI = 3.14159
来源：http://gv.szxytkj.cn

Ruby: PI = 3.14159
来源：http://zm.yuntaijiaju.cn

C#:   const double PI = 3.14159;
来源：http://ma.yuexingan06.cn

[A04] 判断变量类型
来源：http://ca.yuntaijiaju.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://od.panjiajie.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hf.yuexingan06.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://mf.muxihuayi.cn

TS:   typeof x; x instanceof Date
来源：http://yr.shxzukj.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ro.chemitech.net.cn

Go:   reflect.TypeOf(x).Name()
来源：http://dj.panjiajie.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://yr.hnjuh.cn

C#:   x.GetType().Name; x is int
来源：http://ig.muxihuayi.cn

[A05] 整数除法与取模
来源：http://rn.yuntaijiaju.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://dl.bookmarksfly.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://vf.yuexingan06.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://do.shtwfgs.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hp.yuntaijiaju.cn

Java: 7 / 2; 7 % 2
来源：http://ht.yuntaijiaju.cn

Go:   7 / 2; 7 % 2
来源：http://wc.shxzskj.cn

Ruby: 7 / 2; 7 % 2
来源：http://ny.panjiajie.cn

C#:   7 / 2; 7 % 2
来源：http://ty.yuexingan06.cn

[A06] 字符串转数字
来源：http://oj.shtwfgs.cn

Py:   int("42"); float("3.14")
来源：http://ie.gzmigu.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://rg.hnjuh.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://uj.chemitech.net.cn

TS:   parseInt("42", 10); Number("42")
来源：http://za.jianghongdianzi.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://vv.haigaiapp.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://cc.bjjhwx.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://rh.wgjwhj.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://ur.huanxung.cn

[A07] 数字转字符串
来源：http://ba.yuexingan06.cn

Py:   str(42)
来源：http://ij.huanxung.cn

PHP:  (string) 42; strval(42)
来源：http://wg.hnjuh.cn

JS:   String(42); (42).toString()
来源：http://ut.gzmigu.cn

TS:   String(42)
来源：http://qx.muxihuayi.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://ac.bjjhwx.cn

Go:   strconv.Itoa(42)
来源：http://pf.shxzskj.cn

Ruby: 42.to_s
来源：http://bo.bookmarksfly.cn

C#:   42.ToString()
来源：http://ne.haigaiapp.cn

[A08] 取整与四舍五入
来源：http://se.muxihuayi.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://bb.jianghongdianzi.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://an.jctech888.com.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hp.nicolike.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ks.szxytkj.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://vq.lnxyls.cn


<!-- 参考信息 -->