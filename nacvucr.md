代发 wailian999

[U71] PHP：抛出异常
来源：http://hf.chemitech.net.cn

throw new RuntimeException("失败", 500);
来源：http://rb.colortex.cn

[U72] PHP：写错误日志
来源：http://xt.jctech888.com.cn

error_log("失败: " . $e->getMessage());
来源：http://jt.nicolike.cn

[U73] PHP：读取 ini 配置
来源：http://rv.lnxyls.cn

parse_ini_file("config.ini", true)
来源：http://ws.newstarts.cn

[U74] PHP：读取环境变量
来源：http://ia.szxytkj.cn

getenv("APP_ENV") ?: "production"
来源：http://ij.nszjky.cn

[U75] PHP：依赖注入
来源：http://jg.colortex.cn

composer require psr/container
来源：http://vk.haigaiapp.cn

[U76] PHP：简单路由
来源：http://ys.muxihuayi.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hk.yuntaijiaju.cn

[U77] PHP：模板渲染
来源：http://eo.521024.cn

composer require twig/twig
来源：http://uv.nszjky.cn

[U78] PHP：单元测试
来源：http://pg.yuntaijiaju.cn

composer require --dev phpunit/phpunit
来源：http://sh.lnxyls.cn

[U79] PHP：静态分析
来源：http://nw.hnjuh.cn

composer require --dev phpstan/phpstan
来源：http://fj.yuexingan06.cn

[U80] PHP：代码规范修复
来源：http://rp.bookmarksfly.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://do.szsharing.cn

[U81] JS：初始化项目
来源：http://yj.shxzukj.cn

npm init -y;  npm i express
来源：http://iq.colortex.cn

[U82] JS：package.json 脚本
来源：http://zu.asd995.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://pd.shxzukj.cn

[U83] JS：ES Module 导入导出
来源：http://jg.bjjhwx.cn

export const a = 1;  import { a } from "./m.js";
来源：http://oa.chemitech.net.cn

[U84] JS：CommonJS 写法
来源：http://ck.yuexingan06.cn

module.exports = { a };  const { a } = require("./m");
来源：http://ng.9csxet.cn

[U85] JS：可选链
来源：http://ur.szsharing.cn

a?.b?.c
来源：http://tq.jianghongdianzi.cn

[U86] JS：空值合并
来源：http://ui.9csxet.cn

a ?? b
来源：http://iw.jctech888.com.cn

[U87] JS：解构默认值
来源：http://pm.huixinmuqiang.cn

const { a = 1, b = 2 } = obj;
来源：http://jy.9csxet.cn

[U88] JS：对象展开合并
来源：http://qo.jianghongdianzi.cn

{ ...a, ...b }
来源：http://bh.bookmarksfly.cn

[U89] JS：数组去重
来源：http://es.hahajie.cn

[...new Set(arr)]
来源：http://oy.jctech888.com.cn

[U90] JS：数字数组排序
来源：http://cn.nicolike.cn

[...arr].sort((a, b) => a - b)
来源：http://ro.nicolike.cn

[U91] JS：对象键值遍历
来源：http://ld.newstarts.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ke.jianghongdianzi.cn

[U92] JS：深拷贝
来源：http://em.newstarts.cn

structuredClone(obj)
来源：http://ib.shxzskj.cn

[U93] JS：模板字符串
来源：http://bc.newstarts.cn

`共 ${n} 条`
来源：http://im.muxihuayi.cn

[U94] JS：箭头函数
来源：http://mf.panjiajie.cn

const double = x => x * 2;
来源：http://fs.shtwfgs.cn

[U95] JS：Promise 包装
来源：http://ge.lnxyls.cn

new Promise((resolve, reject) => {})
来源：http://zq.haigaiapp.cn

[U96] JS：async/await 与异常
来源：http://wd.yuexingan06.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://jl.9csxet.cn

[U97] JS：并发请求
来源：http://da.yuexingan06.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://ne.jctech888.com.cn

[U98] JS：fetch 带 JSON
来源：http://oz.gzmigu.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://fv.hahajie.cn

[U99] JS：事件监听
来源：http://fq.szxytkj.cn

el.addEventListener("click", e => {})
来源：http://tm.yuexingan06.cn

[U100] JS：DOM 查询
来源：http://lh.lnxyls.cn

document.querySelector(".item")
来源：http://qn.asd995.cn

[U101] JS：classList 操作
来源：http://kr.521024.cn

el.classList.toggle("active")
来源：http://hc.gzmigu.cn

[U102] JS：本地存储
来源：http://wd.newstarts.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://cy.521024.cn

[U103] JS：定时器
来源：http://kv.hahajie.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://gs.newstarts.cn

[U104] JS：防抖
来源：http://tf.hahajie.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qp.yuntaijiaju.cn

[U105] JS：节流
来源：http://nm.yuntaijiaju.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://xg.newstarts.cn

[U106] JS：日期格式化
来源：http://rx.shxzskj.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://fa.yuntaijiaju.cn

[U107] JS：数字千分位
来源：http://ww.shxzskj.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ay.muxihuayi.cn

[U108] JS：随机整数
来源：http://ln.chemitech.net.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://aw.hnjuh.cn

[U109] JS：数组分组
来源：http://bk.jianghongdianzi.cn

Object.groupBy(arr, x => x.type)
来源：http://uk.nszjky.cn

[U110] JS：数组分块
来源：http://hr.521024.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ar.shxzukj.cn

[U111] JS：对象转 Map
来源：http://rl.bjjhwx.cn

new Map(Object.entries(obj))
来源：http://mg.hahajie.cn

[U112] JS：字符串补位
来源：http://jy.huixiangedu.cn

"7".padStart(3, "0")
来源：http://ju.huanxung.cn

[U113] JS：正则替换全部
来源：http://nf.panjiajie.cn

s.replaceAll("a", "b")
来源：http://my.shtwfgs.cn

[U114] JS：JSON 深比较
来源：http://fm.nszjky.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://jm.huanxung.cn

[U115] JS：生成 UUID
来源：http://ol.hahajie.cn

crypto.randomUUID()
来源：http://ij.jctech888.com.cn

[U116] JS：类型检查（JSDoc）
来源：http://wj.yuntaijiaju.cn

/** @param {string} name */ function f(name) {}
来源：http://dx.shxzskj.cn

[U117] JS：单元测试
来源：http://va.9csxet.cn

npm i -D vitest;  npx vitest
来源：http://wy.shxzukj.cn

[U118] JS：开发服务器
来源：http://ak.nszjky.cn

npm i -D vite;  npx vite
来源：http://ua.nszjky.cn

[U119] JS：生产构建
来源：http://an.huixiangedu.cn

npx vite build
来源：http://ti.szxytkj.cn

[U120] JS：读取环境变量（Vite）
来源：http://yh.shxzukj.cn

import.meta.env.VITE_API_URL
来源：http://od.yuexingan06.cn

================================================================================
来源：http://vh.shtwfgs.cn

统计汇总
来源：http://xm.521024.cn

================================================================================
来源：http://as.hahajie.cn

按语言统计（条）：
来源：http://po.521024.cn

Python ......... 252
来源：http://be.bookmarksfly.cn

PHP ............ 252
来源：http://wn.bjjhwx.cn

JavaScript ..... 252
来源：http://qr.szsharing.cn

TypeScript ..... 212
来源：http://zb.nicolike.cn

Java ........... 212
来源：http://ny.jctech888.com.cn

Go ............. 212
来源：http://ev.hahajie.cn

Ruby ........... 212
来源：http://xo.hahajie.cn

C# ............. 212
来源：http://li.521024.cn

C .............. 30
来源：http://iy.yuexingan06.cn

C++ ............ 30
来源：http://mk.huanxung.cn

SQL ............ 90
来源：http://rs.panjiajie.cn

Bash ........... 80
来源：http://ye.szsharing.cn

Kotlin ......... 15
来源：http://af.szsharing.cn

Swift .......... 15
来源：http://zm.haigaiapp.cn

Lua ............ 10
来源：http://fd.gzmigu.cn

Perl ........... 10
来源：http://fz.nicolike.cn

Scala .......... 10
来源：http://vj.shxzskj.cn

------------------------------------
来源：http://lx.hahajie.cn

合计 ........... 2106 条
来源：http://iq.haigaiapp.cn

按章节统计：
来源：http://pd.9csxet.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://yq.521024.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://jn.panjiajie.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://sq.shxzukj.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://bm.bookmarksfly.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wi.yuntaijiaju.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ku.szsharing.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://le.shxzukj.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ko.panjiajie.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://bx.gzmigu.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://fd.huanxung.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://vb.bjjhwx.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://fm.bjjhwx.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://dl.hnjuh.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://vo.asd995.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wq.nszjky.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://rr.521024.cn

Q SQL 专题                              90
来源：http://bz.huixiangedu.cn

R Bash 专题                             80
来源：http://ft.szxytkj.cn

S C / C++ 专题                          60
来源：http://zl.colortex.cn

T 其他语言补充                          60
来源：http://zo.521024.cn

U 高频实用片段                         120
来源：http://tz.521024.cn

------------------------------------
来源：http://bh.haigaiapp.cn

合计                                  2106 条
来源：http://jf.muxihuayi.cn

--------------------------------------------------------------------------------
来源：http://my.jianghongdianzi.cn

使用提醒
来源：http://db.colortex.cn

--------------------------------------------------------------------------------
来源：http://vr.colortex.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ge.chemitech.net.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://vm.szxytkj.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ng.colortex.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://cp.asd995.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://bw.szsharing.cn

—— 文件结束 ——
来源：http://rd.nszjky.cn

================================================================================
来源：http://rv.asd995.cn

程序语言常见例子速查手册（2024 版）
来源：http://kt.szxytkj.cn

Common Programming Examples Cheat Book
来源：http://pc.yuntaijiaju.cn

================================================================================
来源：http://ex.gzmigu.cn

【收录内容】
来源：http://rq.shtwfgs.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://nc.huanxung.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://xj.shxzskj.cn

SQL · Bash · C · C++
来源：http://pm.yuntaijiaju.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://dc.hahajie.cn

【使用说明】
来源：http://lu.hahajie.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ey.9csxet.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://lg.asd995.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ge.9csxet.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://nx.colortex.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://fc.huixinmuqiang.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://sy.hnjuh.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://mf.yuntaijiaju.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://fe.szsharing.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ab.newstarts.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://pt.nszjky.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://qa.panjiajie.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://lr.chemitech.net.cn

【文件统计】
来源：http://dz.hnjuh.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://oy.colortex.cn

--------------------------------------------------------------------------------
来源：http://td.wgjwhj.cn

目  录
来源：http://gb.nicolike.cn

--------------------------------------------------------------------------------
来源：http://af.hnjuh.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://zj.huixiangedu.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://vm.lnxyls.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://cf.shxzukj.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://qc.lnxyls.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://wd.nszjky.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://pd.gzmigu.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://jq.haigaiapp.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ka.hahajie.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://rq.szsharing.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://gh.wgjwhj.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://vq.huixiangedu.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://pv.shxzskj.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://zl.huixinmuqiang.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ls.szxytkj.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://jx.chemitech.net.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://pv.nszjky.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://re.bjjhwx.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://iq.haigaiapp.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hr.nszjky.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ww.521024.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://iz.nszjky.cn

================================================================================
来源：http://kl.panjiajie.cn

A. 基础语法与类型
来源：http://dy.nszjky.cn

================================================================================
来源：http://lj.lnxyls.cn

[A01] Hello World
来源：http://fh.newstarts.cn

Py:   print("Hello, World!")
来源：http://gb.jianghongdianzi.cn

PHP:  echo "Hello, World!";
来源：http://vz.521024.cn

JS:   console.log("Hello, World!");
来源：http://nj.huanxung.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://et.bookmarksfly.cn

Java: System.out.println("Hello, World!");
来源：http://pw.yuntaijiaju.cn

Go:   fmt.Println("Hello, World!")
来源：http://sz.szxytkj.cn

Ruby: puts "Hello, World!"
来源：http://pq.haigaiapp.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://qe.hnjuh.cn

[A02] 变量声明与赋值
来源：http://ma.asd995.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://dn.jianghongdianzi.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://od.panjiajie.cn

JS:   let name = "Alex"; const age = 20;
来源：http://kc.shtwfgs.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ac.yuexingan06.cn

Java: String name = "Alex"; int age = 20;
来源：http://zt.asd995.cn

Go:   name := "Alex"; age := 20
来源：http://gw.bjjhwx.cn

Ruby: name = "Alex"; age = 20
来源：http://vs.jianghongdianzi.cn

C#:   string name = "Alex"; int age = 20;
来源：http://lx.jianghongdianzi.cn

[A03] 常量定义
来源：http://bi.szsharing.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ad.521024.cn

PHP:  const PI = 3.14159;
来源：http://ou.nicolike.cn

JS:   const PI = 3.14159;
来源：http://ky.chemitech.net.cn

TS:   const PI: number = 3.14159;
来源：http://fy.huixinmuqiang.cn

Java: static final double PI = 3.14159;
来源：http://vw.jctech888.com.cn

Go:   const PI = 3.14159
来源：http://na.nicolike.cn

Ruby: PI = 3.14159
来源：http://be.asd995.cn

C#:   const double PI = 3.14159;
来源：http://yg.wgjwhj.cn

[A04] 判断变量类型
来源：http://hv.huanxung.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://uy.shxzskj.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://cj.szsharing.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://aw.asd995.cn

TS:   typeof x; x instanceof Date
来源：http://zx.chemitech.net.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://lm.bjjhwx.cn

Go:   reflect.TypeOf(x).Name()
来源：http://rh.huanxung.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://kj.huanxung.cn

C#:   x.GetType().Name; x is int
来源：http://ki.bjjhwx.cn

[A05] 整数除法与取模
来源：http://mg.hahajie.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hc.szxytkj.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://zk.9csxet.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://st.panjiajie.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://us.huanxung.cn

Java: 7 / 2; 7 % 2
来源：http://dx.shxzskj.cn

Go:   7 / 2; 7 % 2
来源：http://zd.shtwfgs.cn

Ruby: 7 / 2; 7 % 2
来源：http://ic.gzmigu.cn

C#:   7 / 2; 7 % 2
来源：http://jx.shtwfgs.cn

[A06] 字符串转数字
来源：http://cj.szxytkj.cn

Py:   int("42"); float("3.14")
来源：http://lo.hahajie.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://pq.newstarts.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://qd.asd995.cn

TS:   parseInt("42", 10); Number("42")
来源：http://us.chemitech.net.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://id.newstarts.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ww.wgjwhj.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://by.szxytkj.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://fq.haigaiapp.cn

[A07] 数字转字符串
来源：http://gd.gzmigu.cn

Py:   str(42)
来源：http://zu.lnxyls.cn

PHP:  (string) 42; strval(42)
来源：http://kn.chemitech.net.cn

JS:   String(42); (42).toString()
来源：http://rg.bjjhwx.cn

TS:   String(42)
来源：http://qy.panjiajie.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://eu.nszjky.cn

Go:   strconv.Itoa(42)
来源：http://nv.newstarts.cn

Ruby: 42.to_s
来源：http://cv.bjjhwx.cn

C#:   42.ToString()
来源：http://uh.shtwfgs.cn

[A08] 取整与四舍五入
来源：http://yz.yuntaijiaju.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://dl.colortex.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://kh.jctech888.com.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://sp.huanxung.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ru.lnxyls.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://cq.yuexingan06.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://qs.huixiangedu.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://ez.szxytkj.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://oy.colortex.cn

[A09] 绝对值与最大最小值
来源：http://zx.muxihuayi.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ya.szxytkj.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ws.bookmarksfly.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://dg.bookmarksfly.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://vb.bookmarksfly.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://pr.asd995.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ol.huixinmuqiang.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://fq.bookmarksfly.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://hs.hnjuh.cn

[A10] 生成随机数
来源：http://ny.muxihuayi.cn

Py:   import random; random.randint(1, 100)
来源：http://zl.huixinmuqiang.cn

PHP:  random_int(1, 100);
来源：http://xj.huixinmuqiang.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://cr.nszjky.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://mo.szxytkj.cn

Java: new Random().nextInt(100) + 1
来源：http://lr.haigaiapp.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://zs.huanxung.cn

Ruby: rand(1..100)
来源：http://bo.hnjuh.cn

C#:   new Random().Next(1, 101)
来源：http://nz.szxytkj.cn

[A11] 条件表达式（三元）
来源：http://nt.colortex.cn

Py:   "yes" if x > 0 else "no"
来源：http://bt.yuexingan06.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://xl.shxzskj.cn


<!-- 参考信息 -->