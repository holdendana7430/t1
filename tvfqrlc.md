代发 wailian999

[U61] PHP：正则
来源：http://ku.szxytkj.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://uy.newstarts.cn

[U62] PHP：日期对象
来源：http://dt.yuntaijiaju.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://os.szxytkj.cn

[U63] PHP：文件读写
来源：http://ra.lnxyls.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://dm.huixinmuqiang.cn

[U64] PHP：目录遍历
来源：http://fw.jianghongdianzi.cn

glob("dir/*.php");  scandir("dir");
来源：http://yx.huanxung.cn

[U65] PHP：会话
来源：http://rr.521024.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://qs.shxzskj.cn

[U66] PHP：设置 Cookie
来源：http://hj.wgjwhj.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ez.asd995.cn

[U67] PHP：处理文件上传
来源：http://fe.bjjhwx.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ii.yuexingan06.cn

[U68] PHP：PDO 连接
来源：http://yk.jianghongdianzi.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://rx.colortex.cn

[U69] PHP：PDO 预处理
来源：http://dz.nicolike.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://xr.huixinmuqiang.cn

[U70] PHP：PDO 事务
来源：http://oq.shxzukj.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://gj.shxzskj.cn

[U71] PHP：抛出异常
来源：http://nw.bookmarksfly.cn

throw new RuntimeException("失败", 500);
来源：http://fh.szxytkj.cn

[U72] PHP：写错误日志
来源：http://xt.jianghongdianzi.cn

error_log("失败: " . $e->getMessage());
来源：http://dq.9csxet.cn

[U73] PHP：读取 ini 配置
来源：http://np.nszjky.cn

parse_ini_file("config.ini", true)
来源：http://qa.gzmigu.cn

[U74] PHP：读取环境变量
来源：http://fv.521024.cn

getenv("APP_ENV") ?: "production"
来源：http://ow.yuntaijiaju.cn

[U75] PHP：依赖注入
来源：http://if.9csxet.cn

composer require psr/container
来源：http://wo.huixinmuqiang.cn

[U76] PHP：简单路由
来源：http://hy.wgjwhj.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://oe.9csxet.cn

[U77] PHP：模板渲染
来源：http://pm.bjjhwx.cn

composer require twig/twig
来源：http://uz.9csxet.cn

[U78] PHP：单元测试
来源：http://av.bjjhwx.cn

composer require --dev phpunit/phpunit
来源：http://kt.wgjwhj.cn

[U79] PHP：静态分析
来源：http://nv.wgjwhj.cn

composer require --dev phpstan/phpstan
来源：http://iu.wgjwhj.cn

[U80] PHP：代码规范修复
来源：http://xl.panjiajie.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://az.panjiajie.cn

[U81] JS：初始化项目
来源：http://lc.shxzukj.cn

npm init -y;  npm i express
来源：http://wh.lnxyls.cn

[U82] JS：package.json 脚本
来源：http://kt.yuexingan06.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://pi.hnjuh.cn

[U83] JS：ES Module 导入导出
来源：http://ce.lnxyls.cn

export const a = 1;  import { a } from "./m.js";
来源：http://ee.newstarts.cn

[U84] JS：CommonJS 写法
来源：http://ax.9csxet.cn

module.exports = { a };  const { a } = require("./m");
来源：http://ce.shtwfgs.cn

[U85] JS：可选链
来源：http://ge.colortex.cn

a?.b?.c
来源：http://ee.nszjky.cn

[U86] JS：空值合并
来源：http://al.huixiangedu.cn

a ?? b
来源：http://qa.yuexingan06.cn

[U87] JS：解构默认值
来源：http://gh.chemitech.net.cn

const { a = 1, b = 2 } = obj;
来源：http://vn.colortex.cn

[U88] JS：对象展开合并
来源：http://in.huanxung.cn

{ ...a, ...b }
来源：http://yk.jianghongdianzi.cn

[U89] JS：数组去重
来源：http://vq.yuexingan06.cn

[...new Set(arr)]
来源：http://vk.panjiajie.cn

[U90] JS：数字数组排序
来源：http://pl.colortex.cn

[...arr].sort((a, b) => a - b)
来源：http://wr.huanxung.cn

[U91] JS：对象键值遍历
来源：http://uq.huanxung.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://fm.muxihuayi.cn

[U92] JS：深拷贝
来源：http://va.gzmigu.cn

structuredClone(obj)
来源：http://pp.bookmarksfly.cn

[U93] JS：模板字符串
来源：http://ab.huanxung.cn

`共 ${n} 条`
来源：http://zc.521024.cn

[U94] JS：箭头函数
来源：http://wa.bjjhwx.cn

const double = x => x * 2;
来源：http://mc.huixiangedu.cn

[U95] JS：Promise 包装
来源：http://ln.lnxyls.cn

new Promise((resolve, reject) => {})
来源：http://fr.yuntaijiaju.cn

[U96] JS：async/await 与异常
来源：http://uk.panjiajie.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://kd.asd995.cn

[U97] JS：并发请求
来源：http://bi.jctech888.com.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://la.bookmarksfly.cn

[U98] JS：fetch 带 JSON
来源：http://fz.huanxung.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mr.shxzukj.cn

[U99] JS：事件监听
来源：http://sk.hnjuh.cn

el.addEventListener("click", e => {})
来源：http://ku.asd995.cn

[U100] JS：DOM 查询
来源：http://oy.bookmarksfly.cn

document.querySelector(".item")
来源：http://ge.9csxet.cn

[U101] JS：classList 操作
来源：http://ca.colortex.cn

el.classList.toggle("active")
来源：http://hk.newstarts.cn

[U102] JS：本地存储
来源：http://vw.9csxet.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://wz.huixiangedu.cn

[U103] JS：定时器
来源：http://ch.9csxet.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://us.yuntaijiaju.cn

[U104] JS：防抖
来源：http://zw.newstarts.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bf.newstarts.cn

[U105] JS：节流
来源：http://pk.szsharing.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ny.hahajie.cn

[U106] JS：日期格式化
来源：http://lt.huixiangedu.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://bt.haigaiapp.cn

[U107] JS：数字千分位
来源：http://sn.yuntaijiaju.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hf.asd995.cn

[U108] JS：随机整数
来源：http://fj.shxzskj.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://vs.hahajie.cn

[U109] JS：数组分组
来源：http://kw.bjjhwx.cn

Object.groupBy(arr, x => x.type)
来源：http://lv.yuexingan06.cn

[U110] JS：数组分块
来源：http://ku.521024.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://da.gzmigu.cn

[U111] JS：对象转 Map
来源：http://yk.hahajie.cn

new Map(Object.entries(obj))
来源：http://xk.jctech888.com.cn

[U112] JS：字符串补位
来源：http://st.yuexingan06.cn

"7".padStart(3, "0")
来源：http://yu.huixiangedu.cn

[U113] JS：正则替换全部
来源：http://bd.521024.cn

s.replaceAll("a", "b")
来源：http://xy.asd995.cn

[U114] JS：JSON 深比较
来源：http://um.yuexingan06.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://wj.shxzukj.cn

[U115] JS：生成 UUID
来源：http://ed.9csxet.cn

crypto.randomUUID()
来源：http://cp.chemitech.net.cn

[U116] JS：类型检查（JSDoc）
来源：http://fx.newstarts.cn

/** @param {string} name */ function f(name) {}
来源：http://kr.lnxyls.cn

[U117] JS：单元测试
来源：http://xv.muxihuayi.cn

npm i -D vitest;  npx vitest
来源：http://vo.lnxyls.cn

[U118] JS：开发服务器
来源：http://rr.bookmarksfly.cn

npm i -D vite;  npx vite
来源：http://ox.nicolike.cn

[U119] JS：生产构建
来源：http://re.nicolike.cn

npx vite build
来源：http://ai.chemitech.net.cn

[U120] JS：读取环境变量（Vite）
来源：http://qe.bjjhwx.cn

import.meta.env.VITE_API_URL
来源：http://yc.9csxet.cn

================================================================================
来源：http://ue.chemitech.net.cn

统计汇总
来源：http://fe.szxytkj.cn

================================================================================
来源：http://de.shxzskj.cn

按语言统计（条）：
来源：http://hc.shxzskj.cn

Python ......... 252
来源：http://zc.hahajie.cn

PHP ............ 252
来源：http://ez.nszjky.cn

JavaScript ..... 252
来源：http://vh.chemitech.net.cn

TypeScript ..... 212
来源：http://rw.hahajie.cn

Java ........... 212
来源：http://dc.panjiajie.cn

Go ............. 212
来源：http://yd.muxihuayi.cn

Ruby ........... 212
来源：http://wn.asd995.cn

C# ............. 212
来源：http://fs.jianghongdianzi.cn

C .............. 30
来源：http://xf.yuntaijiaju.cn

C++ ............ 30
来源：http://oh.nicolike.cn

SQL ............ 90
来源：http://jd.9csxet.cn

Bash ........... 80
来源：http://vt.9csxet.cn

Kotlin ......... 15
来源：http://cm.szxytkj.cn

Swift .......... 15
来源：http://he.yuntaijiaju.cn

Lua ............ 10
来源：http://mz.521024.cn

Perl ........... 10
来源：http://wy.bookmarksfly.cn

Scala .......... 10
来源：http://bx.lnxyls.cn

------------------------------------
来源：http://mo.bookmarksfly.cn

合计 ........... 2106 条
来源：http://py.9csxet.cn

按章节统计：
来源：http://dq.yuexingan06.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://oc.szxytkj.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://rc.nszjky.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://oz.bookmarksfly.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ow.lnxyls.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://iz.haigaiapp.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://or.nicolike.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ni.yuntaijiaju.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ri.colortex.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://tu.asd995.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://yx.szxytkj.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://im.yuexingan06.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://vz.huanxung.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://sz.huanxung.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://pq.bookmarksfly.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hd.huixinmuqiang.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://lg.shxzukj.cn

Q SQL 专题                              90
来源：http://lh.huanxung.cn

R Bash 专题                             80
来源：http://gx.nszjky.cn

S C / C++ 专题                          60
来源：http://av.huixiangedu.cn

T 其他语言补充                          60
来源：http://yi.shxzukj.cn

U 高频实用片段                         120
来源：http://vq.newstarts.cn

------------------------------------
来源：http://gg.colortex.cn

合计                                  2106 条
来源：http://vg.9csxet.cn

--------------------------------------------------------------------------------
来源：http://dd.huixiangedu.cn

使用提醒
来源：http://xe.colortex.cn

--------------------------------------------------------------------------------
来源：http://cc.szxytkj.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://vb.panjiajie.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://be.chemitech.net.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://tr.jianghongdianzi.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://es.szxytkj.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ur.jctech888.com.cn

—— 文件结束 ——
来源：http://dg.hnjuh.cn

================================================================================
来源：http://hj.jianghongdianzi.cn

程序语言常见例子速查手册（2024 版）
来源：http://bm.colortex.cn

Common Programming Examples Cheat Book
来源：http://pn.shxzskj.cn

================================================================================
来源：http://rx.colortex.cn

【收录内容】
来源：http://oi.muxihuayi.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://lt.9csxet.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://nl.nicolike.cn

SQL · Bash · C · C++
来源：http://eu.lnxyls.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hl.szsharing.cn

【使用说明】
来源：http://qw.panjiajie.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://cr.521024.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://io.yuexingan06.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://qc.newstarts.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://fo.gzmigu.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://pi.521024.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://jf.colortex.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ai.nszjky.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://zh.newstarts.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://kk.hnjuh.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hh.newstarts.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://tw.muxihuayi.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://uh.newstarts.cn

【文件统计】
来源：http://aq.yuexingan06.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ek.huixiangedu.cn

--------------------------------------------------------------------------------
来源：http://rd.asd995.cn

目  录
来源：http://kq.wgjwhj.cn

--------------------------------------------------------------------------------
来源：http://mr.nicolike.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://as.nicolike.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://gq.haigaiapp.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://ot.lnxyls.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ey.shtwfgs.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://cn.jianghongdianzi.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://yj.jctech888.com.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://nk.szxytkj.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://vt.huanxung.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ed.gzmigu.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://om.newstarts.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://zq.bookmarksfly.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://tt.colortex.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://tr.chemitech.net.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ge.hnjuh.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.hahajie.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://ab.jctech888.com.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://mq.wgjwhj.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://uf.hahajie.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://jc.panjiajie.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://xo.gzmigu.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://lo.asd995.cn

================================================================================
来源：http://zm.nicolike.cn

A. 基础语法与类型
来源：http://gm.wgjwhj.cn

================================================================================
来源：http://ts.yuexingan06.cn

[A01] Hello World
来源：http://aj.yuntaijiaju.cn

Py:   print("Hello, World!")
来源：http://im.panjiajie.cn

PHP:  echo "Hello, World!";
来源：http://la.bjjhwx.cn

JS:   console.log("Hello, World!");
来源：http://iq.haigaiapp.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ha.jianghongdianzi.cn

Java: System.out.println("Hello, World!");
来源：http://pg.gzmigu.cn

Go:   fmt.Println("Hello, World!")
来源：http://ix.gzmigu.cn

Ruby: puts "Hello, World!"
来源：http://fy.nicolike.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://lh.shtwfgs.cn

[A02] 变量声明与赋值
来源：http://qs.asd995.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://gi.panjiajie.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://cs.jctech888.com.cn

JS:   let name = "Alex"; const age = 20;
来源：http://ww.huixiangedu.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ft.haigaiapp.cn

Java: String name = "Alex"; int age = 20;
来源：http://ps.jctech888.com.cn

Go:   name := "Alex"; age := 20
来源：http://vp.bjjhwx.cn

Ruby: name = "Alex"; age = 20
来源：http://xy.colortex.cn

C#:   string name = "Alex"; int age = 20;
来源：http://jo.yuexingan06.cn

[A03] 常量定义
来源：http://ie.huixiangedu.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://pu.hahajie.cn

PHP:  const PI = 3.14159;
来源：http://yw.asd995.cn

JS:   const PI = 3.14159;
来源：http://cg.521024.cn

TS:   const PI: number = 3.14159;
来源：http://wd.szsharing.cn

Java: static final double PI = 3.14159;
来源：http://hf.jctech888.com.cn

Go:   const PI = 3.14159
来源：http://ns.jctech888.com.cn

Ruby: PI = 3.14159
来源：http://sw.shtwfgs.cn

C#:   const double PI = 3.14159;
来源：http://ks.muxihuayi.cn

[A04] 判断变量类型
来源：http://oh.chemitech.net.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://hi.bookmarksfly.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://rq.asd995.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://cd.nszjky.cn

TS:   typeof x; x instanceof Date
来源：http://pf.jianghongdianzi.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://gn.nicolike.cn

Go:   reflect.TypeOf(x).Name()
来源：http://yo.wgjwhj.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://gz.szxytkj.cn

C#:   x.GetType().Name; x is int
来源：http://zw.hnjuh.cn

[A05] 整数除法与取模
来源：http://vc.nicolike.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ev.asd995.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://ms.yuntaijiaju.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://yh.jianghongdianzi.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://eq.panjiajie.cn

Java: 7 / 2; 7 % 2
来源：http://hu.chemitech.net.cn

Go:   7 / 2; 7 % 2
来源：http://sw.newstarts.cn

Ruby: 7 / 2; 7 % 2
来源：http://wl.bjjhwx.cn

C#:   7 / 2; 7 % 2
来源：http://lz.asd995.cn

[A06] 字符串转数字
来源：http://xn.yuntaijiaju.cn

Py:   int("42"); float("3.14")
来源：http://nu.huixinmuqiang.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://fw.hnjuh.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://tk.bjjhwx.cn

TS:   parseInt("42", 10); Number("42")
来源：http://nm.yuntaijiaju.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://il.chemitech.net.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hu.jianghongdianzi.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://ex.shxzukj.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://fb.lnxyls.cn

[A07] 数字转字符串
来源：http://hl.huanxung.cn

Py:   str(42)
来源：http://kg.panjiajie.cn

PHP:  (string) 42; strval(42)
来源：http://nb.haigaiapp.cn

JS:   String(42); (42).toString()
来源：http://it.521024.cn

TS:   String(42)
来源：http://nl.panjiajie.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://ok.szsharing.cn

Go:   strconv.Itoa(42)
来源：http://wc.shtwfgs.cn

Ruby: 42.to_s
来源：http://vv.newstarts.cn

C#:   42.ToString()
来源：http://kp.nszjky.cn

[A08] 取整与四舍五入
来源：http://an.shxzskj.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://mv.wgjwhj.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://eh.yuexingan06.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hc.muxihuayi.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://va.yuexingan06.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://ri.szxytkj.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://wa.bjjhwx.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://po.9csxet.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://pq.bookmarksfly.cn

[A09] 绝对值与最大最小值
来源：http://qh.nszjky.cn


<!-- 参考信息 -->