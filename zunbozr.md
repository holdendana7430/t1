代发 wailian999

[U55] PHP：match 表达式
来源：http://ps.shxzskj.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://up.jctech888.com.cn

[U56] PHP：命名参数
来源：http://un.panjiajie.cn

f(a: 1, b: 2)
来源：http://wj.szxytkj.cn

[U57] PHP：字符串插值
来源：http://yv.shxzukj.cn

"值: {$a}"
来源：http://mt.hnjuh.cn

[U58] PHP：数组三件套
来源：http://qq.9csxet.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://fk.shtwfgs.cn

[U59] PHP：自定义排序
来源：http://ck.muxihuayi.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ln.huixinmuqiang.cn

[U60] PHP：JSON 编解码
来源：http://hj.shtwfgs.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://el.asd995.cn

[U61] PHP：正则
来源：http://sy.huixiangedu.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ru.shxzskj.cn

[U62] PHP：日期对象
来源：http://zp.chemitech.net.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://et.muxihuayi.cn

[U63] PHP：文件读写
来源：http://lj.panjiajie.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://tg.bookmarksfly.cn

[U64] PHP：目录遍历
来源：http://eg.haigaiapp.cn

glob("dir/*.php");  scandir("dir");
来源：http://if.bookmarksfly.cn

[U65] PHP：会话
来源：http://xh.hahajie.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://hy.muxihuayi.cn

[U66] PHP：设置 Cookie
来源：http://fi.wgjwhj.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://xa.wgjwhj.cn

[U67] PHP：处理文件上传
来源：http://vy.asd995.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://lf.bjjhwx.cn

[U68] PHP：PDO 连接
来源：http://bg.panjiajie.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://xw.huixinmuqiang.cn

[U69] PHP：PDO 预处理
来源：http://zi.wgjwhj.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://bq.newstarts.cn

[U70] PHP：PDO 事务
来源：http://qx.shtwfgs.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://zx.hahajie.cn

[U71] PHP：抛出异常
来源：http://tw.szxytkj.cn

throw new RuntimeException("失败", 500);
来源：http://sz.huanxung.cn

[U72] PHP：写错误日志
来源：http://qd.shxzukj.cn

error_log("失败: " . $e->getMessage());
来源：http://kf.panjiajie.cn

[U73] PHP：读取 ini 配置
来源：http://om.szxytkj.cn

parse_ini_file("config.ini", true)
来源：http://tf.szxytkj.cn

[U74] PHP：读取环境变量
来源：http://eq.hahajie.cn

getenv("APP_ENV") ?: "production"
来源：http://mp.muxihuayi.cn

[U75] PHP：依赖注入
来源：http://ci.hnjuh.cn

composer require psr/container
来源：http://rd.shxzukj.cn

[U76] PHP：简单路由
来源：http://et.panjiajie.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://rz.yuexingan06.cn

[U77] PHP：模板渲染
来源：http://br.colortex.cn

composer require twig/twig
来源：http://dq.shtwfgs.cn

[U78] PHP：单元测试
来源：http://kb.gzmigu.cn

composer require --dev phpunit/phpunit
来源：http://bb.yuntaijiaju.cn

[U79] PHP：静态分析
来源：http://uj.haigaiapp.cn

composer require --dev phpstan/phpstan
来源：http://jj.newstarts.cn

[U80] PHP：代码规范修复
来源：http://ky.521024.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://qs.9csxet.cn

[U81] JS：初始化项目
来源：http://yc.bookmarksfly.cn

npm init -y;  npm i express
来源：http://nu.gzmigu.cn

[U82] JS：package.json 脚本
来源：http://hn.gzmigu.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://jg.shxzukj.cn

[U83] JS：ES Module 导入导出
来源：http://yi.yuntaijiaju.cn

export const a = 1;  import { a } from "./m.js";
来源：http://yi.chemitech.net.cn

[U84] JS：CommonJS 写法
来源：http://iw.chemitech.net.cn

module.exports = { a };  const { a } = require("./m");
来源：http://il.huanxung.cn

[U85] JS：可选链
来源：http://cf.newstarts.cn

a?.b?.c
来源：http://nc.521024.cn

[U86] JS：空值合并
来源：http://gb.hahajie.cn

a ?? b
来源：http://gi.nicolike.cn

[U87] JS：解构默认值
来源：http://wy.gzmigu.cn

const { a = 1, b = 2 } = obj;
来源：http://je.hnjuh.cn

[U88] JS：对象展开合并
来源：http://ry.gzmigu.cn

{ ...a, ...b }
来源：http://zq.newstarts.cn

[U89] JS：数组去重
来源：http://es.shtwfgs.cn

[...new Set(arr)]
来源：http://nr.asd995.cn

[U90] JS：数字数组排序
来源：http://aa.colortex.cn

[...arr].sort((a, b) => a - b)
来源：http://vw.521024.cn

[U91] JS：对象键值遍历
来源：http://pa.521024.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wn.shtwfgs.cn

[U92] JS：深拷贝
来源：http://cc.chemitech.net.cn

structuredClone(obj)
来源：http://ii.shxzukj.cn

[U93] JS：模板字符串
来源：http://ng.jianghongdianzi.cn

`共 ${n} 条`
来源：http://ef.chemitech.net.cn

[U94] JS：箭头函数
来源：http://xx.jctech888.com.cn

const double = x => x * 2;
来源：http://ch.newstarts.cn

[U95] JS：Promise 包装
来源：http://ch.colortex.cn

new Promise((resolve, reject) => {})
来源：http://mh.asd995.cn

[U96] JS：async/await 与异常
来源：http://oj.gzmigu.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://bv.9csxet.cn

[U97] JS：并发请求
来源：http://iv.lnxyls.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://lz.gzmigu.cn

[U98] JS：fetch 带 JSON
来源：http://ac.panjiajie.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://cu.shxzskj.cn

[U99] JS：事件监听
来源：http://gy.yuexingan06.cn

el.addEventListener("click", e => {})
来源：http://ax.yuntaijiaju.cn

[U100] JS：DOM 查询
来源：http://ec.shtwfgs.cn

document.querySelector(".item")
来源：http://qf.chemitech.net.cn

[U101] JS：classList 操作
来源：http://ja.newstarts.cn

el.classList.toggle("active")
来源：http://zg.gzmigu.cn

[U102] JS：本地存储
来源：http://sv.haigaiapp.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://cn.yuexingan06.cn

[U103] JS：定时器
来源：http://ae.asd995.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wn.nicolike.cn

[U104] JS：防抖
来源：http://qj.shxzskj.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ah.jianghongdianzi.cn

[U105] JS：节流
来源：http://la.huanxung.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hr.hnjuh.cn

[U106] JS：日期格式化
来源：http://uq.wgjwhj.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://om.gzmigu.cn

[U107] JS：数字千分位
来源：http://gd.9csxet.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wn.muxihuayi.cn

[U108] JS：随机整数
来源：http://pi.nicolike.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://vz.huanxung.cn

[U109] JS：数组分组
来源：http://xc.9csxet.cn

Object.groupBy(arr, x => x.type)
来源：http://yr.chemitech.net.cn

[U110] JS：数组分块
来源：http://mz.yuntaijiaju.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://dq.hnjuh.cn

[U111] JS：对象转 Map
来源：http://sk.gzmigu.cn

new Map(Object.entries(obj))
来源：http://ir.hnjuh.cn

[U112] JS：字符串补位
来源：http://je.nszjky.cn

"7".padStart(3, "0")
来源：http://oy.chemitech.net.cn

[U113] JS：正则替换全部
来源：http://gf.haigaiapp.cn

s.replaceAll("a", "b")
来源：http://dp.hahajie.cn

[U114] JS：JSON 深比较
来源：http://ls.chemitech.net.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://ha.lnxyls.cn

[U115] JS：生成 UUID
来源：http://ya.jianghongdianzi.cn

crypto.randomUUID()
来源：http://vy.shxzskj.cn

[U116] JS：类型检查（JSDoc）
来源：http://mw.nicolike.cn

/** @param {string} name */ function f(name) {}
来源：http://pv.yuntaijiaju.cn

[U117] JS：单元测试
来源：http://ir.huixiangedu.cn

npm i -D vitest;  npx vitest
来源：http://qq.huixiangedu.cn

[U118] JS：开发服务器
来源：http://um.huanxung.cn

npm i -D vite;  npx vite
来源：http://al.hahajie.cn

[U119] JS：生产构建
来源：http://na.huixiangedu.cn

npx vite build
来源：http://gk.jctech888.com.cn

[U120] JS：读取环境变量（Vite）
来源：http://pt.yuexingan06.cn

import.meta.env.VITE_API_URL
来源：http://ax.huixiangedu.cn

================================================================================
来源：http://ar.huixiangedu.cn

统计汇总
来源：http://am.lnxyls.cn

================================================================================
来源：http://tu.asd995.cn

按语言统计（条）：
来源：http://jp.huanxung.cn

Python ......... 252
来源：http://ox.colortex.cn

PHP ............ 252
来源：http://uv.nicolike.cn

JavaScript ..... 252
来源：http://eq.yuntaijiaju.cn

TypeScript ..... 212
来源：http://as.shxzukj.cn

Java ........... 212
来源：http://iz.huixiangedu.cn

Go ............. 212
来源：http://vo.bookmarksfly.cn

Ruby ........... 212
来源：http://gc.lnxyls.cn

C# ............. 212
来源：http://wu.nszjky.cn

C .............. 30
来源：http://ak.asd995.cn

C++ ............ 30
来源：http://nk.gzmigu.cn

SQL ............ 90
来源：http://ne.szxytkj.cn

Bash ........... 80
来源：http://bh.colortex.cn

Kotlin ......... 15
来源：http://st.nicolike.cn

Swift .......... 15
来源：http://zw.yuntaijiaju.cn

Lua ............ 10
来源：http://jr.huanxung.cn

Perl ........... 10
来源：http://fh.huixinmuqiang.cn

Scala .......... 10
来源：http://yp.szsharing.cn

------------------------------------
来源：http://yn.wgjwhj.cn

合计 ........... 2106 条
来源：http://fu.huixinmuqiang.cn

按章节统计：
来源：http://nh.newstarts.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hv.shxzskj.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://os.jctech888.com.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hb.haigaiapp.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hf.panjiajie.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://gh.panjiajie.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://nu.shxzskj.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://sw.jctech888.com.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://zx.yuexingan06.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://pw.muxihuayi.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ae.asd995.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://pn.shtwfgs.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://jj.bjjhwx.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://jk.hahajie.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://pg.panjiajie.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://am.newstarts.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://cb.bjjhwx.cn

Q SQL 专题                              90
来源：http://iv.huixinmuqiang.cn

R Bash 专题                             80
来源：http://cu.colortex.cn

S C / C++ 专题                          60
来源：http://le.jianghongdianzi.cn

T 其他语言补充                          60
来源：http://aj.newstarts.cn

U 高频实用片段                         120
来源：http://kb.bjjhwx.cn

------------------------------------
来源：http://gz.haigaiapp.cn

合计                                  2106 条
来源：http://wp.shtwfgs.cn

--------------------------------------------------------------------------------
来源：http://bq.jctech888.com.cn

使用提醒
来源：http://oh.shtwfgs.cn

--------------------------------------------------------------------------------
来源：http://oi.bjjhwx.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://eg.nszjky.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://zp.hnjuh.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://xw.szxytkj.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://rq.shxzukj.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://nz.newstarts.cn

—— 文件结束 ——
来源：http://vj.haigaiapp.cn

================================================================================
来源：http://bx.szsharing.cn

程序语言常见例子速查手册（2024 版）
来源：http://kg.nszjky.cn

Common Programming Examples Cheat Book
来源：http://co.gzmigu.cn

================================================================================
来源：http://pt.huanxung.cn

【收录内容】
来源：http://fj.hahajie.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://te.huanxung.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ee.colortex.cn

SQL · Bash · C · C++
来源：http://qw.jctech888.com.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://bc.hahajie.cn

【使用说明】
来源：http://yq.hahajie.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://vf.szxytkj.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://te.jctech888.com.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://rh.newstarts.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://bk.lnxyls.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://nl.nszjky.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://dg.nicolike.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wz.asd995.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://sr.jctech888.com.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://kk.haigaiapp.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://gu.colortex.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ny.haigaiapp.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://sq.yuntaijiaju.cn

【文件统计】
来源：http://ex.jctech888.com.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://nx.chemitech.net.cn

--------------------------------------------------------------------------------
来源：http://df.lnxyls.cn

目  录
来源：http://we.wgjwhj.cn

--------------------------------------------------------------------------------
来源：http://rc.bjjhwx.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://sf.nszjky.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ek.yuntaijiaju.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://pb.panjiajie.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ac.chemitech.net.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://dd.colortex.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://is.wgjwhj.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://xr.yuexingan06.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://mq.huixinmuqiang.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ja.colortex.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://cz.muxihuayi.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ro.colortex.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://vk.muxihuayi.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://yg.jctech888.com.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://at.jctech888.com.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://wv.shxzukj.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://uh.hnjuh.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://kd.gzmigu.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://bq.wgjwhj.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://xr.hnjuh.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://jb.colortex.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://ig.huixiangedu.cn

================================================================================
来源：http://jn.hahajie.cn

A. 基础语法与类型
来源：http://tt.jctech888.com.cn

================================================================================
来源：http://bz.shxzukj.cn

[A01] Hello World
来源：http://bn.muxihuayi.cn

Py:   print("Hello, World!")
来源：http://au.shxzskj.cn

PHP:  echo "Hello, World!";
来源：http://yk.huanxung.cn

JS:   console.log("Hello, World!");
来源：http://fg.huanxung.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://tu.huixiangedu.cn

Java: System.out.println("Hello, World!");
来源：http://wr.haigaiapp.cn

Go:   fmt.Println("Hello, World!")
来源：http://oc.colortex.cn

Ruby: puts "Hello, World!"
来源：http://xx.jianghongdianzi.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://ah.huixiangedu.cn

[A02] 变量声明与赋值
来源：http://bc.asd995.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://gm.nszjky.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://wz.panjiajie.cn

JS:   let name = "Alex"; const age = 20;
来源：http://ie.bookmarksfly.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://iv.huanxung.cn

Java: String name = "Alex"; int age = 20;
来源：http://cs.jianghongdianzi.cn

Go:   name := "Alex"; age := 20
来源：http://mi.haigaiapp.cn

Ruby: name = "Alex"; age = 20
来源：http://af.nicolike.cn

C#:   string name = "Alex"; int age = 20;
来源：http://gy.hahajie.cn

[A03] 常量定义
来源：http://er.9csxet.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://re.hahajie.cn

PHP:  const PI = 3.14159;
来源：http://xw.nszjky.cn

JS:   const PI = 3.14159;
来源：http://pq.szsharing.cn

TS:   const PI: number = 3.14159;
来源：http://kk.gzmigu.cn

Java: static final double PI = 3.14159;
来源：http://mq.chemitech.net.cn

Go:   const PI = 3.14159
来源：http://pc.huixinmuqiang.cn

Ruby: PI = 3.14159
来源：http://ky.haigaiapp.cn

C#:   const double PI = 3.14159;
来源：http://nf.panjiajie.cn

[A04] 判断变量类型
来源：http://nw.asd995.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://um.yuexingan06.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ad.bookmarksfly.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://jr.panjiajie.cn

TS:   typeof x; x instanceof Date
来源：http://as.shxzukj.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ci.shxzukj.cn

Go:   reflect.TypeOf(x).Name()
来源：http://xb.nszjky.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://gw.huanxung.cn

C#:   x.GetType().Name; x is int
来源：http://vs.asd995.cn

[A05] 整数除法与取模
来源：http://wj.jctech888.com.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://qb.bjjhwx.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://zk.gzmigu.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://gw.yuexingan06.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://td.wgjwhj.cn

Java: 7 / 2; 7 % 2
来源：http://pd.szxytkj.cn

Go:   7 / 2; 7 % 2
来源：http://fd.hnjuh.cn

Ruby: 7 / 2; 7 % 2
来源：http://og.huanxung.cn

C#:   7 / 2; 7 % 2
来源：http://sw.szxytkj.cn

[A06] 字符串转数字
来源：http://xv.521024.cn

Py:   int("42"); float("3.14")
来源：http://jn.hnjuh.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://id.bjjhwx.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hn.shtwfgs.cn

TS:   parseInt("42", 10); Number("42")
来源：http://ib.nszjky.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://cc.panjiajie.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://vi.shxzukj.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://im.colortex.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://ov.yuntaijiaju.cn

[A07] 数字转字符串
来源：http://xp.bjjhwx.cn

Py:   str(42)
来源：http://sa.jianghongdianzi.cn

PHP:  (string) 42; strval(42)
来源：http://xu.huixiangedu.cn

JS:   String(42); (42).toString()
来源：http://fa.jctech888.com.cn

TS:   String(42)
来源：http://dc.huixiangedu.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://xv.shtwfgs.cn

Go:   strconv.Itoa(42)
来源：http://ui.panjiajie.cn


<!-- 参考信息 -->