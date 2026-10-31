代发 wailian999

[U59] PHP：自定义排序
来源：http://wn.huixiangedu.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://qq.huanxung.cn

[U60] PHP：JSON 编解码
来源：http://yb.huixinmuqiang.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://vn.nszjky.cn

[U61] PHP：正则
来源：http://lr.bookmarksfly.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://bv.shxzukj.cn

[U62] PHP：日期对象
来源：http://wr.szsharing.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://on.szsharing.cn

[U63] PHP：文件读写
来源：http://fm.muxihuayi.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://fs.shxzskj.cn

[U64] PHP：目录遍历
来源：http://fh.gzmigu.cn

glob("dir/*.php");  scandir("dir");
来源：http://dc.muxihuayi.cn

[U65] PHP：会话
来源：http://ge.huixiangedu.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://oc.shxzskj.cn

[U66] PHP：设置 Cookie
来源：http://na.newstarts.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://sg.9csxet.cn

[U67] PHP：处理文件上传
来源：http://io.nszjky.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://uv.asd995.cn

[U68] PHP：PDO 连接
来源：http://yb.haigaiapp.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ne.nszjky.cn

[U69] PHP：PDO 预处理
来源：http://fh.bjjhwx.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://nb.szxytkj.cn

[U70] PHP：PDO 事务
来源：http://hi.szxytkj.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://dd.shtwfgs.cn

[U71] PHP：抛出异常
来源：http://mx.wgjwhj.cn

throw new RuntimeException("失败", 500);
来源：http://il.nicolike.cn

[U72] PHP：写错误日志
来源：http://ye.huixiangedu.cn

error_log("失败: " . $e->getMessage());
来源：http://xn.muxihuayi.cn

[U73] PHP：读取 ini 配置
来源：http://ca.shxzskj.cn

parse_ini_file("config.ini", true)
来源：http://ik.gzmigu.cn

[U74] PHP：读取环境变量
来源：http://hb.shxzskj.cn

getenv("APP_ENV") ?: "production"
来源：http://ad.haigaiapp.cn

[U75] PHP：依赖注入
来源：http://wg.9csxet.cn

composer require psr/container
来源：http://gm.yuexingan06.cn

[U76] PHP：简单路由
来源：http://pm.chemitech.net.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hk.wgjwhj.cn

[U77] PHP：模板渲染
来源：http://bi.hahajie.cn

composer require twig/twig
来源：http://xe.jctech888.com.cn

[U78] PHP：单元测试
来源：http://xv.jianghongdianzi.cn

composer require --dev phpunit/phpunit
来源：http://lz.nszjky.cn

[U79] PHP：静态分析
来源：http://jz.jianghongdianzi.cn

composer require --dev phpstan/phpstan
来源：http://jo.asd995.cn

[U80] PHP：代码规范修复
来源：http://zm.lnxyls.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://py.asd995.cn

[U81] JS：初始化项目
来源：http://vl.shxzskj.cn

npm init -y;  npm i express
来源：http://tq.szxytkj.cn

[U82] JS：package.json 脚本
来源：http://ef.521024.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://rm.asd995.cn

[U83] JS：ES Module 导入导出
来源：http://rm.bookmarksfly.cn

export const a = 1;  import { a } from "./m.js";
来源：http://kd.jctech888.com.cn

[U84] JS：CommonJS 写法
来源：http://yr.lnxyls.cn

module.exports = { a };  const { a } = require("./m");
来源：http://yy.hnjuh.cn

[U85] JS：可选链
来源：http://wj.yuexingan06.cn

a?.b?.c
来源：http://kf.szsharing.cn

[U86] JS：空值合并
来源：http://ui.bookmarksfly.cn

a ?? b
来源：http://yg.gzmigu.cn

[U87] JS：解构默认值
来源：http://ko.jctech888.com.cn

const { a = 1, b = 2 } = obj;
来源：http://bu.asd995.cn

[U88] JS：对象展开合并
来源：http://yy.hahajie.cn

{ ...a, ...b }
来源：http://jz.jctech888.com.cn

[U89] JS：数组去重
来源：http://zl.shxzskj.cn

[...new Set(arr)]
来源：http://wi.asd995.cn

[U90] JS：数字数组排序
来源：http://fq.yuexingan06.cn

[...arr].sort((a, b) => a - b)
来源：http://cr.nicolike.cn

[U91] JS：对象键值遍历
来源：http://bq.colortex.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://yo.muxihuayi.cn

[U92] JS：深拷贝
来源：http://ep.shxzukj.cn

structuredClone(obj)
来源：http://zw.jianghongdianzi.cn

[U93] JS：模板字符串
来源：http://wf.szxytkj.cn

`共 ${n} 条`
来源：http://ug.9csxet.cn

[U94] JS：箭头函数
来源：http://hi.yuntaijiaju.cn

const double = x => x * 2;
来源：http://ue.szxytkj.cn

[U95] JS：Promise 包装
来源：http://re.bjjhwx.cn

new Promise((resolve, reject) => {})
来源：http://na.yuexingan06.cn

[U96] JS：async/await 与异常
来源：http://bc.bookmarksfly.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://qn.shxzskj.cn

[U97] JS：并发请求
来源：http://rq.shtwfgs.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://fg.muxihuayi.cn

[U98] JS：fetch 带 JSON
来源：http://la.nszjky.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://zv.yuexingan06.cn

[U99] JS：事件监听
来源：http://cs.huanxung.cn

el.addEventListener("click", e => {})
来源：http://lm.9csxet.cn

[U100] JS：DOM 查询
来源：http://bl.shxzukj.cn

document.querySelector(".item")
来源：http://dv.nicolike.cn

[U101] JS：classList 操作
来源：http://he.wgjwhj.cn

el.classList.toggle("active")
来源：http://kn.newstarts.cn

[U102] JS：本地存储
来源：http://jp.bookmarksfly.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://di.hahajie.cn

[U103] JS：定时器
来源：http://ty.newstarts.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://qr.haigaiapp.cn

[U104] JS：防抖
来源：http://qs.jianghongdianzi.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://si.jctech888.com.cn

[U105] JS：节流
来源：http://mh.shxzskj.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://gt.bookmarksfly.cn

[U106] JS：日期格式化
来源：http://mb.huanxung.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://qx.shtwfgs.cn

[U107] JS：数字千分位
来源：http://wk.nszjky.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://sk.shxzukj.cn

[U108] JS：随机整数
来源：http://vp.bookmarksfly.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://oz.hnjuh.cn

[U109] JS：数组分组
来源：http://dk.nicolike.cn

Object.groupBy(arr, x => x.type)
来源：http://mp.huanxung.cn

[U110] JS：数组分块
来源：http://jw.szsharing.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wu.shtwfgs.cn

[U111] JS：对象转 Map
来源：http://pq.szxytkj.cn

new Map(Object.entries(obj))
来源：http://zl.yuntaijiaju.cn

[U112] JS：字符串补位
来源：http://xx.wgjwhj.cn

"7".padStart(3, "0")
来源：http://fu.asd995.cn

[U113] JS：正则替换全部
来源：http://ba.huixinmuqiang.cn

s.replaceAll("a", "b")
来源：http://lk.9csxet.cn

[U114] JS：JSON 深比较
来源：http://uj.huanxung.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://of.gzmigu.cn

[U115] JS：生成 UUID
来源：http://ly.asd995.cn

crypto.randomUUID()
来源：http://lb.huanxung.cn

[U116] JS：类型检查（JSDoc）
来源：http://sn.szxytkj.cn

/** @param {string} name */ function f(name) {}
来源：http://is.521024.cn

[U117] JS：单元测试
来源：http://fe.szxytkj.cn

npm i -D vitest;  npx vitest
来源：http://rl.shtwfgs.cn

[U118] JS：开发服务器
来源：http://zw.muxihuayi.cn

npm i -D vite;  npx vite
来源：http://xc.huixiangedu.cn

[U119] JS：生产构建
来源：http://li.bookmarksfly.cn

npx vite build
来源：http://xn.chemitech.net.cn

[U120] JS：读取环境变量（Vite）
来源：http://wk.newstarts.cn

import.meta.env.VITE_API_URL
来源：http://ur.jctech888.com.cn

================================================================================
来源：http://ke.panjiajie.cn

统计汇总
来源：http://za.newstarts.cn

================================================================================
来源：http://cw.asd995.cn

按语言统计（条）：
来源：http://pq.huanxung.cn

Python ......... 252
来源：http://kj.521024.cn

PHP ............ 252
来源：http://wx.huixinmuqiang.cn

JavaScript ..... 252
来源：http://zy.panjiajie.cn

TypeScript ..... 212
来源：http://ly.shxzskj.cn

Java ........... 212
来源：http://pm.shxzukj.cn

Go ............. 212
来源：http://ol.hahajie.cn

Ruby ........... 212
来源：http://jc.panjiajie.cn

C# ............. 212
来源：http://cg.yuexingan06.cn

C .............. 30
来源：http://xk.jianghongdianzi.cn

C++ ............ 30
来源：http://ef.nszjky.cn

SQL ............ 90
来源：http://wu.hahajie.cn

Bash ........... 80
来源：http://ta.hnjuh.cn

Kotlin ......... 15
来源：http://pb.haigaiapp.cn

Swift .......... 15
来源：http://tz.colortex.cn

Lua ............ 10
来源：http://uf.bookmarksfly.cn

Perl ........... 10
来源：http://rn.chemitech.net.cn

Scala .......... 10
来源：http://os.huanxung.cn

------------------------------------
来源：http://tm.newstarts.cn

合计 ........... 2106 条
来源：http://qx.chemitech.net.cn

按章节统计：
来源：http://fl.shxzskj.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://qr.chemitech.net.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://br.wgjwhj.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wo.colortex.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://gr.shxzukj.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://er.nicolike.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://km.panjiajie.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://kt.szsharing.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://pc.panjiajie.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://oi.shxzskj.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://yi.yuntaijiaju.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ba.shtwfgs.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://zm.haigaiapp.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://vj.hnjuh.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wf.jctech888.com.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mi.jianghongdianzi.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ys.shtwfgs.cn

Q SQL 专题                              90
来源：http://dz.hnjuh.cn

R Bash 专题                             80
来源：http://hr.haigaiapp.cn

S C / C++ 专题                          60
来源：http://nj.szsharing.cn

T 其他语言补充                          60
来源：http://bx.shtwfgs.cn

U 高频实用片段                         120
来源：http://hb.nszjky.cn

------------------------------------
来源：http://qa.yuntaijiaju.cn

合计                                  2106 条
来源：http://ys.bjjhwx.cn

--------------------------------------------------------------------------------
来源：http://eu.lnxyls.cn

使用提醒
来源：http://oi.9csxet.cn

--------------------------------------------------------------------------------
来源：http://cb.jctech888.com.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://jt.colortex.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://oc.9csxet.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://go.muxihuayi.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://ye.huanxung.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://qz.yuntaijiaju.cn

—— 文件结束 ——
来源：http://dl.hahajie.cn

================================================================================
来源：http://hm.9csxet.cn

程序语言常见例子速查手册（2024 版）
来源：http://ux.shxzskj.cn

Common Programming Examples Cheat Book
来源：http://ia.huixiangedu.cn

================================================================================
来源：http://ph.szsharing.cn

【收录内容】
来源：http://gn.szxytkj.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://vi.shxzskj.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://gj.yuntaijiaju.cn

SQL · Bash · C · C++
来源：http://ls.hahajie.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://oe.huanxung.cn

【使用说明】
来源：http://bq.shxzukj.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://or.nszjky.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://rh.lnxyls.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://re.shxzukj.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://wb.haigaiapp.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://er.jctech888.com.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://io.shtwfgs.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://yc.panjiajie.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ta.yuntaijiaju.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://mu.9csxet.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://vm.521024.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://eo.szsharing.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://cv.lnxyls.cn

【文件统计】
来源：http://uq.shtwfgs.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://is.lnxyls.cn

--------------------------------------------------------------------------------
来源：http://cm.jctech888.com.cn

目  录
来源：http://bz.shxzskj.cn

--------------------------------------------------------------------------------
来源：http://uk.colortex.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ry.muxihuayi.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://xo.yuexingan06.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://nm.muxihuayi.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://xa.panjiajie.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://xw.lnxyls.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://pi.521024.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://ck.wgjwhj.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://aw.yuexingan06.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://uz.9csxet.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://nk.yuexingan06.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://kh.jianghongdianzi.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://ts.nicolike.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://sk.shxzskj.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hn.szxytkj.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ox.nszjky.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://jk.jianghongdianzi.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://qv.szxytkj.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://vh.panjiajie.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://ud.panjiajie.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://bo.colortex.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://ws.huanxung.cn

================================================================================
来源：http://sc.shtwfgs.cn

A. 基础语法与类型
来源：http://kz.muxihuayi.cn

================================================================================
来源：http://vw.shtwfgs.cn

[A01] Hello World
来源：http://mp.shxzukj.cn

Py:   print("Hello, World!")
来源：http://dz.panjiajie.cn

PHP:  echo "Hello, World!";
来源：http://pn.jianghongdianzi.cn

JS:   console.log("Hello, World!");
来源：http://uz.shxzukj.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ky.9csxet.cn

Java: System.out.println("Hello, World!");
来源：http://mx.nszjky.cn

Go:   fmt.Println("Hello, World!")
来源：http://rn.chemitech.net.cn

Ruby: puts "Hello, World!"
来源：http://oj.jianghongdianzi.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://hk.wgjwhj.cn

[A02] 变量声明与赋值
来源：http://xz.shxzskj.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://nr.yuexingan06.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://ut.hahajie.cn

JS:   let name = "Alex"; const age = 20;
来源：http://pp.huanxung.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://vy.yuntaijiaju.cn

Java: String name = "Alex"; int age = 20;
来源：http://ph.chemitech.net.cn

Go:   name := "Alex"; age := 20
来源：http://xq.jctech888.com.cn

Ruby: name = "Alex"; age = 20
来源：http://jv.gzmigu.cn

C#:   string name = "Alex"; int age = 20;
来源：http://ok.asd995.cn

[A03] 常量定义
来源：http://ze.haigaiapp.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://gv.yuexingan06.cn

PHP:  const PI = 3.14159;
来源：http://cv.gzmigu.cn

JS:   const PI = 3.14159;
来源：http://xi.jianghongdianzi.cn

TS:   const PI: number = 3.14159;
来源：http://md.huixiangedu.cn

Java: static final double PI = 3.14159;
来源：http://to.nicolike.cn

Go:   const PI = 3.14159
来源：http://pl.jianghongdianzi.cn

Ruby: PI = 3.14159
来源：http://yb.haigaiapp.cn

C#:   const double PI = 3.14159;
来源：http://gy.szsharing.cn

[A04] 判断变量类型
来源：http://ve.yuexingan06.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://gp.newstarts.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ut.haigaiapp.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://wo.colortex.cn

TS:   typeof x; x instanceof Date
来源：http://zp.shtwfgs.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://nh.jianghongdianzi.cn

Go:   reflect.TypeOf(x).Name()
来源：http://ms.yuexingan06.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://nj.haigaiapp.cn

C#:   x.GetType().Name; x is int
来源：http://tv.bookmarksfly.cn

[A05] 整数除法与取模
来源：http://wc.shxzskj.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://mb.yuntaijiaju.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://rg.hahajie.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://lv.gzmigu.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://em.szsharing.cn

Java: 7 / 2; 7 % 2
来源：http://eb.jctech888.com.cn

Go:   7 / 2; 7 % 2
来源：http://mv.colortex.cn

Ruby: 7 / 2; 7 % 2
来源：http://gu.szxytkj.cn

C#:   7 / 2; 7 % 2
来源：http://le.huixinmuqiang.cn

[A06] 字符串转数字
来源：http://oi.bjjhwx.cn

Py:   int("42"); float("3.14")
来源：http://mb.jianghongdianzi.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://yv.bookmarksfly.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ul.jianghongdianzi.cn

TS:   parseInt("42", 10); Number("42")
来源：http://nn.lnxyls.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://go.colortex.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://bc.wgjwhj.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://ga.521024.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://ns.panjiajie.cn

[A07] 数字转字符串
来源：http://it.gzmigu.cn

Py:   str(42)
来源：http://ie.chemitech.net.cn

PHP:  (string) 42; strval(42)
来源：http://vu.haigaiapp.cn

JS:   String(42); (42).toString()
来源：http://ue.huixiangedu.cn

TS:   String(42)
来源：http://or.hnjuh.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://oo.bookmarksfly.cn

Go:   strconv.Itoa(42)
来源：http://yu.hnjuh.cn

Ruby: 42.to_s
来源：http://ba.shtwfgs.cn

C#:   42.ToString()
来源：http://cg.bjjhwx.cn

[A08] 取整与四舍五入
来源：http://my.panjiajie.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ix.newstarts.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://td.9csxet.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://or.yuexingan06.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://oq.wgjwhj.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://aa.newstarts.cn


<!-- 参考信息 -->