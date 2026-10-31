代发 wailian999

[U53] PHP：空合并运算符
来源：http://my.9csxet.cn

$v = $a ?? $b ?? "default";
来源：http://yg.yuexingan06.cn

[U54] PHP：空安全调用
来源：http://jo.nicolike.cn

$obj?->method()
来源：http://gi.yuntaijiaju.cn

[U55] PHP：match 表达式
来源：http://gk.hahajie.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://qm.huanxung.cn

[U56] PHP：命名参数
来源：http://gc.hnjuh.cn

f(a: 1, b: 2)
来源：http://sc.gzmigu.cn

[U57] PHP：字符串插值
来源：http://ak.yuntaijiaju.cn

"值: {$a}"
来源：http://fy.chemitech.net.cn

[U58] PHP：数组三件套
来源：http://rr.huixiangedu.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://dq.colortex.cn

[U59] PHP：自定义排序
来源：http://kj.wgjwhj.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hu.huixiangedu.cn

[U60] PHP：JSON 编解码
来源：http://od.yuntaijiaju.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://kp.jctech888.com.cn

[U61] PHP：正则
来源：http://vq.shxzskj.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://bx.9csxet.cn

[U62] PHP：日期对象
来源：http://sv.szxytkj.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ol.haigaiapp.cn

[U63] PHP：文件读写
来源：http://pv.yuntaijiaju.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ku.wgjwhj.cn

[U64] PHP：目录遍历
来源：http://vq.jianghongdianzi.cn

glob("dir/*.php");  scandir("dir");
来源：http://xh.huixinmuqiang.cn

[U65] PHP：会话
来源：http://gk.yuntaijiaju.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://ev.yuexingan06.cn

[U66] PHP：设置 Cookie
来源：http://xj.jianghongdianzi.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://tv.szxytkj.cn

[U67] PHP：处理文件上传
来源：http://hu.nszjky.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://st.hnjuh.cn

[U68] PHP：PDO 连接
来源：http://be.521024.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ws.wgjwhj.cn

[U69] PHP：PDO 预处理
来源：http://ds.gzmigu.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://bb.muxihuayi.cn

[U70] PHP：PDO 事务
来源：http://yd.9csxet.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://vi.hnjuh.cn

[U71] PHP：抛出异常
来源：http://hv.muxihuayi.cn

throw new RuntimeException("失败", 500);
来源：http://ee.szsharing.cn

[U72] PHP：写错误日志
来源：http://cp.huixiangedu.cn

error_log("失败: " . $e->getMessage());
来源：http://mn.huixiangedu.cn

[U73] PHP：读取 ini 配置
来源：http://nn.jctech888.com.cn

parse_ini_file("config.ini", true)
来源：http://nh.nszjky.cn

[U74] PHP：读取环境变量
来源：http://da.lnxyls.cn

getenv("APP_ENV") ?: "production"
来源：http://lt.shxzskj.cn

[U75] PHP：依赖注入
来源：http://on.newstarts.cn

composer require psr/container
来源：http://rg.muxihuayi.cn

[U76] PHP：简单路由
来源：http://tg.newstarts.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://bg.521024.cn

[U77] PHP：模板渲染
来源：http://nu.chemitech.net.cn

composer require twig/twig
来源：http://px.huanxung.cn

[U78] PHP：单元测试
来源：http://dn.huanxung.cn

composer require --dev phpunit/phpunit
来源：http://ds.szsharing.cn

[U79] PHP：静态分析
来源：http://iw.hnjuh.cn

composer require --dev phpstan/phpstan
来源：http://mk.shxzskj.cn

[U80] PHP：代码规范修复
来源：http://au.huanxung.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://ye.panjiajie.cn

[U81] JS：初始化项目
来源：http://hp.newstarts.cn

npm init -y;  npm i express
来源：http://nz.huixinmuqiang.cn

[U82] JS：package.json 脚本
来源：http://an.lnxyls.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://qy.jctech888.com.cn

[U83] JS：ES Module 导入导出
来源：http://og.hnjuh.cn

export const a = 1;  import { a } from "./m.js";
来源：http://jq.shxzukj.cn

[U84] JS：CommonJS 写法
来源：http://tv.521024.cn

module.exports = { a };  const { a } = require("./m");
来源：http://dh.jctech888.com.cn

[U85] JS：可选链
来源：http://jq.gzmigu.cn

a?.b?.c
来源：http://lo.yuntaijiaju.cn

[U86] JS：空值合并
来源：http://ro.shtwfgs.cn

a ?? b
来源：http://mr.521024.cn

[U87] JS：解构默认值
来源：http://nv.muxihuayi.cn

const { a = 1, b = 2 } = obj;
来源：http://ou.huanxung.cn

[U88] JS：对象展开合并
来源：http://hz.huixiangedu.cn

{ ...a, ...b }
来源：http://mj.9csxet.cn

[U89] JS：数组去重
来源：http://ez.muxihuayi.cn

[...new Set(arr)]
来源：http://nb.jctech888.com.cn

[U90] JS：数字数组排序
来源：http://gl.521024.cn

[...arr].sort((a, b) => a - b)
来源：http://nm.huanxung.cn

[U91] JS：对象键值遍历
来源：http://uz.bjjhwx.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://zd.szxytkj.cn

[U92] JS：深拷贝
来源：http://eg.wgjwhj.cn

structuredClone(obj)
来源：http://th.nszjky.cn

[U93] JS：模板字符串
来源：http://bi.szsharing.cn

`共 ${n} 条`
来源：http://gh.yuexingan06.cn

[U94] JS：箭头函数
来源：http://gv.jianghongdianzi.cn

const double = x => x * 2;
来源：http://wn.9csxet.cn

[U95] JS：Promise 包装
来源：http://ce.szsharing.cn

new Promise((resolve, reject) => {})
来源：http://qa.521024.cn

[U96] JS：async/await 与异常
来源：http://xy.panjiajie.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://vt.bookmarksfly.cn

[U97] JS：并发请求
来源：http://gu.shxzukj.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://cp.shtwfgs.cn

[U98] JS：fetch 带 JSON
来源：http://ff.shxzukj.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://yc.bjjhwx.cn

[U99] JS：事件监听
来源：http://jq.panjiajie.cn

el.addEventListener("click", e => {})
来源：http://bh.colortex.cn

[U100] JS：DOM 查询
来源：http://ue.shtwfgs.cn

document.querySelector(".item")
来源：http://ty.jianghongdianzi.cn

[U101] JS：classList 操作
来源：http://ln.hnjuh.cn

el.classList.toggle("active")
来源：http://ds.huixinmuqiang.cn

[U102] JS：本地存储
来源：http://rb.panjiajie.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://hu.jctech888.com.cn

[U103] JS：定时器
来源：http://nf.hahajie.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ws.yuexingan06.cn

[U104] JS：防抖
来源：http://fo.521024.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://yd.asd995.cn

[U105] JS：节流
来源：http://fs.gzmigu.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://bj.panjiajie.cn

[U106] JS：日期格式化
来源：http://mk.bookmarksfly.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://yo.colortex.cn

[U107] JS：数字千分位
来源：http://jp.wgjwhj.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ce.nicolike.cn

[U108] JS：随机整数
来源：http://qx.yuntaijiaju.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ug.nicolike.cn

[U109] JS：数组分组
来源：http://fz.huixinmuqiang.cn

Object.groupBy(arr, x => x.type)
来源：http://xr.newstarts.cn

[U110] JS：数组分块
来源：http://zr.521024.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://fd.gzmigu.cn

[U111] JS：对象转 Map
来源：http://sa.colortex.cn

new Map(Object.entries(obj))
来源：http://gw.bjjhwx.cn

[U112] JS：字符串补位
来源：http://de.yuexingan06.cn

"7".padStart(3, "0")
来源：http://dh.yuexingan06.cn

[U113] JS：正则替换全部
来源：http://su.colortex.cn

s.replaceAll("a", "b")
来源：http://ks.szsharing.cn

[U114] JS：JSON 深比较
来源：http://xt.haigaiapp.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://xq.huixiangedu.cn

[U115] JS：生成 UUID
来源：http://bp.shxzukj.cn

crypto.randomUUID()
来源：http://uk.jctech888.com.cn

[U116] JS：类型检查（JSDoc）
来源：http://nt.huixiangedu.cn

/** @param {string} name */ function f(name) {}
来源：http://hr.yuntaijiaju.cn

[U117] JS：单元测试
来源：http://ci.shxzukj.cn

npm i -D vitest;  npx vitest
来源：http://tc.huanxung.cn

[U118] JS：开发服务器
来源：http://hj.shxzskj.cn

npm i -D vite;  npx vite
来源：http://gk.bookmarksfly.cn

[U119] JS：生产构建
来源：http://bu.colortex.cn

npx vite build
来源：http://hz.gzmigu.cn

[U120] JS：读取环境变量（Vite）
来源：http://yl.hahajie.cn

import.meta.env.VITE_API_URL
来源：http://yw.szxytkj.cn

================================================================================
来源：http://ik.huixiangedu.cn

统计汇总
来源：http://ts.muxihuayi.cn

================================================================================
来源：http://gc.hahajie.cn

按语言统计（条）：
来源：http://ww.gzmigu.cn

Python ......... 252
来源：http://tt.huanxung.cn

PHP ............ 252
来源：http://jx.szsharing.cn

JavaScript ..... 252
来源：http://mx.chemitech.net.cn

TypeScript ..... 212
来源：http://cs.hahajie.cn

Java ........... 212
来源：http://vb.asd995.cn

Go ............. 212
来源：http://nk.shtwfgs.cn

Ruby ........... 212
来源：http://gz.nszjky.cn

C# ............. 212
来源：http://fg.gzmigu.cn

C .............. 30
来源：http://sj.panjiajie.cn

C++ ............ 30
来源：http://xf.jctech888.com.cn

SQL ............ 90
来源：http://ec.9csxet.cn

Bash ........... 80
来源：http://ya.yuexingan06.cn

Kotlin ......... 15
来源：http://pi.9csxet.cn

Swift .......... 15
来源：http://yb.yuntaijiaju.cn

Lua ............ 10
来源：http://xo.hahajie.cn

Perl ........... 10
来源：http://hm.bjjhwx.cn

Scala .......... 10
来源：http://us.szxytkj.cn

------------------------------------
来源：http://na.bookmarksfly.cn

合计 ........... 2106 条
来源：http://js.wgjwhj.cn

按章节统计：
来源：http://pg.colortex.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wc.bjjhwx.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://cb.9csxet.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ot.colortex.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://pg.szsharing.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://bh.gzmigu.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mk.haigaiapp.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ql.szsharing.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://vl.wgjwhj.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://cj.9csxet.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://bz.shxzukj.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://fn.nszjky.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://th.newstarts.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://iv.huixiangedu.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://om.asd995.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://nn.lnxyls.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://fe.shxzukj.cn

Q SQL 专题                              90
来源：http://hn.lnxyls.cn

R Bash 专题                             80
来源：http://jj.lnxyls.cn

S C / C++ 专题                          60
来源：http://su.chemitech.net.cn

T 其他语言补充                          60
来源：http://cj.newstarts.cn

U 高频实用片段                         120
来源：http://gl.shtwfgs.cn

------------------------------------
来源：http://ws.lnxyls.cn

合计                                  2106 条
来源：http://dr.colortex.cn

--------------------------------------------------------------------------------
来源：http://mi.shtwfgs.cn

使用提醒
来源：http://nl.huixinmuqiang.cn

--------------------------------------------------------------------------------
来源：http://so.gzmigu.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://xh.szsharing.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://uv.yuntaijiaju.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://bo.huixinmuqiang.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://vv.asd995.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://bv.gzmigu.cn

—— 文件结束 ——
来源：http://ko.asd995.cn

================================================================================
来源：http://fb.nszjky.cn

程序语言常见例子速查手册（2024 版）
来源：http://iz.jianghongdianzi.cn

Common Programming Examples Cheat Book
来源：http://yu.huixinmuqiang.cn

================================================================================
来源：http://sr.yuntaijiaju.cn

【收录内容】
来源：http://zy.hnjuh.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://pi.jianghongdianzi.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://kf.huanxung.cn

SQL · Bash · C · C++
来源：http://te.szsharing.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ly.jianghongdianzi.cn

【使用说明】
来源：http://xd.shxzukj.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hs.muxihuayi.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ym.asd995.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://rt.bookmarksfly.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://rd.panjiajie.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://vh.haigaiapp.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://dc.shtwfgs.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ia.hnjuh.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://pn.chemitech.net.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ls.yuntaijiaju.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://gy.yuntaijiaju.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://lv.yuntaijiaju.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://kx.huixinmuqiang.cn

【文件统计】
来源：http://zh.jianghongdianzi.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://dj.hnjuh.cn

--------------------------------------------------------------------------------
来源：http://vj.nicolike.cn

目  录
来源：http://hh.muxihuayi.cn

--------------------------------------------------------------------------------
来源：http://yv.bookmarksfly.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ov.521024.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ub.9csxet.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://ne.panjiajie.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://fx.nicolike.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://fz.yuexingan06.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://qr.wgjwhj.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://nh.muxihuayi.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://rn.huixinmuqiang.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://av.hahajie.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://lr.shtwfgs.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://pk.jctech888.com.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://pm.panjiajie.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://ay.bjjhwx.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ef.shxzukj.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://jp.panjiajie.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://kv.gzmigu.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://sz.muxihuayi.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://hp.panjiajie.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://gi.haigaiapp.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://sk.hahajie.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://pz.521024.cn

================================================================================
来源：http://oi.chemitech.net.cn

A. 基础语法与类型
来源：http://ub.nicolike.cn

================================================================================
来源：http://hz.jianghongdianzi.cn

[A01] Hello World
来源：http://ht.huanxung.cn

Py:   print("Hello, World!")
来源：http://gj.bjjhwx.cn

PHP:  echo "Hello, World!";
来源：http://ds.lnxyls.cn

JS:   console.log("Hello, World!");
来源：http://am.shtwfgs.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://tg.521024.cn

Java: System.out.println("Hello, World!");
来源：http://bs.huanxung.cn

Go:   fmt.Println("Hello, World!")
来源：http://yi.jctech888.com.cn

Ruby: puts "Hello, World!"
来源：http://pf.colortex.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://xp.yuntaijiaju.cn

[A02] 变量声明与赋值
来源：http://vr.gzmigu.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://da.hahajie.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://xz.yuexingan06.cn

JS:   let name = "Alex"; const age = 20;
来源：http://sj.shtwfgs.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://um.yuexingan06.cn

Java: String name = "Alex"; int age = 20;
来源：http://wy.hnjuh.cn

Go:   name := "Alex"; age := 20
来源：http://sj.panjiajie.cn

Ruby: name = "Alex"; age = 20
来源：http://dz.newstarts.cn

C#:   string name = "Alex"; int age = 20;
来源：http://mw.521024.cn

[A03] 常量定义
来源：http://qx.shxzukj.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://gf.asd995.cn

PHP:  const PI = 3.14159;
来源：http://mn.bookmarksfly.cn

JS:   const PI = 3.14159;
来源：http://yj.yuexingan06.cn

TS:   const PI: number = 3.14159;
来源：http://rw.szxytkj.cn

Java: static final double PI = 3.14159;
来源：http://fr.nszjky.cn

Go:   const PI = 3.14159
来源：http://qo.chemitech.net.cn

Ruby: PI = 3.14159
来源：http://fn.huixinmuqiang.cn

C#:   const double PI = 3.14159;
来源：http://dt.huanxung.cn

[A04] 判断变量类型
来源：http://fw.9csxet.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://fx.hnjuh.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://zt.jianghongdianzi.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://ia.haigaiapp.cn

TS:   typeof x; x instanceof Date
来源：http://qi.shxzskj.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ug.521024.cn

Go:   reflect.TypeOf(x).Name()
来源：http://od.shtwfgs.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://wq.bjjhwx.cn

C#:   x.GetType().Name; x is int
来源：http://sp.yuntaijiaju.cn

[A05] 整数除法与取模
来源：http://pa.haigaiapp.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://re.haigaiapp.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://cs.shxzukj.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://gy.yuntaijiaju.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://tu.wgjwhj.cn

Java: 7 / 2; 7 % 2
来源：http://yw.nszjky.cn

Go:   7 / 2; 7 % 2
来源：http://so.lnxyls.cn

Ruby: 7 / 2; 7 % 2
来源：http://nx.nicolike.cn

C#:   7 / 2; 7 % 2
来源：http://rm.asd995.cn

[A06] 字符串转数字
来源：http://yo.muxihuayi.cn

Py:   int("42"); float("3.14")
来源：http://bt.gzmigu.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://vx.hahajie.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://of.szxytkj.cn

TS:   parseInt("42", 10); Number("42")
来源：http://cc.jianghongdianzi.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hz.bjjhwx.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://iu.nszjky.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://et.gzmigu.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://sd.muxihuayi.cn

[A07] 数字转字符串
来源：http://tk.wgjwhj.cn

Py:   str(42)
来源：http://ui.chemitech.net.cn

PHP:  (string) 42; strval(42)
来源：http://ar.chemitech.net.cn


<!-- 参考信息 -->