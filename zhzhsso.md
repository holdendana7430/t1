代发 wailian999

[U53] PHP：空合并运算符
来源：http://kw.jianghongdianzi.cn

$v = $a ?? $b ?? "default";
来源：http://db.muxihuayi.cn

[U54] PHP：空安全调用
来源：http://ci.hnjuh.cn

$obj?->method()
来源：http://zf.colortex.cn

[U55] PHP：match 表达式
来源：http://mh.yuexingan06.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://lm.jctech888.com.cn

[U56] PHP：命名参数
来源：http://ow.muxihuayi.cn

f(a: 1, b: 2)
来源：http://qi.nicolike.cn

[U57] PHP：字符串插值
来源：http://sa.huixinmuqiang.cn

"值: {$a}"
来源：http://vf.huanxung.cn

[U58] PHP：数组三件套
来源：http://kv.bookmarksfly.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://qk.hahajie.cn

[U59] PHP：自定义排序
来源：http://ui.nicolike.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://jm.jianghongdianzi.cn

[U60] PHP：JSON 编解码
来源：http://re.shxzskj.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://xy.szsharing.cn

[U61] PHP：正则
来源：http://dk.jianghongdianzi.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://jo.panjiajie.cn

[U62] PHP：日期对象
来源：http://hj.colortex.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://jh.jianghongdianzi.cn

[U63] PHP：文件读写
来源：http://qq.yuntaijiaju.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://pb.newstarts.cn

[U64] PHP：目录遍历
来源：http://bw.huixiangedu.cn

glob("dir/*.php");  scandir("dir");
来源：http://cq.muxihuayi.cn

[U65] PHP：会话
来源：http://tw.jctech888.com.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://vf.huixiangedu.cn

[U66] PHP：设置 Cookie
来源：http://hi.shxzukj.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://oy.newstarts.cn

[U67] PHP：处理文件上传
来源：http://cc.nszjky.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://nz.jianghongdianzi.cn

[U68] PHP：PDO 连接
来源：http://vk.shxzukj.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mb.chemitech.net.cn

[U69] PHP：PDO 预处理
来源：http://pj.hnjuh.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ev.huixiangedu.cn

[U70] PHP：PDO 事务
来源：http://pq.jianghongdianzi.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://qr.haigaiapp.cn

[U71] PHP：抛出异常
来源：http://ep.lnxyls.cn

throw new RuntimeException("失败", 500);
来源：http://ib.gzmigu.cn

[U72] PHP：写错误日志
来源：http://oi.szxytkj.cn

error_log("失败: " . $e->getMessage());
来源：http://fg.yuntaijiaju.cn

[U73] PHP：读取 ini 配置
来源：http://pc.521024.cn

parse_ini_file("config.ini", true)
来源：http://lh.nicolike.cn

[U74] PHP：读取环境变量
来源：http://zd.lnxyls.cn

getenv("APP_ENV") ?: "production"
来源：http://tc.huanxung.cn

[U75] PHP：依赖注入
来源：http://zd.newstarts.cn

composer require psr/container
来源：http://cn.muxihuayi.cn

[U76] PHP：简单路由
来源：http://dj.hahajie.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://uu.521024.cn

[U77] PHP：模板渲染
来源：http://dj.huixiangedu.cn

composer require twig/twig
来源：http://ah.colortex.cn

[U78] PHP：单元测试
来源：http://wa.huixiangedu.cn

composer require --dev phpunit/phpunit
来源：http://tq.newstarts.cn

[U79] PHP：静态分析
来源：http://ki.newstarts.cn

composer require --dev phpstan/phpstan
来源：http://rc.gzmigu.cn

[U80] PHP：代码规范修复
来源：http://lk.haigaiapp.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://yh.nicolike.cn

[U81] JS：初始化项目
来源：http://ts.yuntaijiaju.cn

npm init -y;  npm i express
来源：http://om.hnjuh.cn

[U82] JS：package.json 脚本
来源：http://zr.szsharing.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://nl.yuexingan06.cn

[U83] JS：ES Module 导入导出
来源：http://ze.shtwfgs.cn

export const a = 1;  import { a } from "./m.js";
来源：http://dm.haigaiapp.cn

[U84] JS：CommonJS 写法
来源：http://bo.shtwfgs.cn

module.exports = { a };  const { a } = require("./m");
来源：http://io.521024.cn

[U85] JS：可选链
来源：http://ft.bjjhwx.cn

a?.b?.c
来源：http://af.yuexingan06.cn

[U86] JS：空值合并
来源：http://si.newstarts.cn

a ?? b
来源：http://cx.panjiajie.cn

[U87] JS：解构默认值
来源：http://ir.hnjuh.cn

const { a = 1, b = 2 } = obj;
来源：http://zm.szsharing.cn

[U88] JS：对象展开合并
来源：http://go.szxytkj.cn

{ ...a, ...b }
来源：http://pt.colortex.cn

[U89] JS：数组去重
来源：http://xn.yuntaijiaju.cn

[...new Set(arr)]
来源：http://sh.newstarts.cn

[U90] JS：数字数组排序
来源：http://ey.bjjhwx.cn

[...arr].sort((a, b) => a - b)
来源：http://xo.chemitech.net.cn

[U91] JS：对象键值遍历
来源：http://al.yuntaijiaju.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://jt.newstarts.cn

[U92] JS：深拷贝
来源：http://ax.jianghongdianzi.cn

structuredClone(obj)
来源：http://dl.521024.cn

[U93] JS：模板字符串
来源：http://my.muxihuayi.cn

`共 ${n} 条`
来源：http://ef.shxzukj.cn

[U94] JS：箭头函数
来源：http://ir.hahajie.cn

const double = x => x * 2;
来源：http://ar.panjiajie.cn

[U95] JS：Promise 包装
来源：http://aj.wgjwhj.cn

new Promise((resolve, reject) => {})
来源：http://mn.hnjuh.cn

[U96] JS：async/await 与异常
来源：http://kd.muxihuayi.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mf.nszjky.cn

[U97] JS：并发请求
来源：http://os.lnxyls.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://sw.jianghongdianzi.cn

[U98] JS：fetch 带 JSON
来源：http://ft.chemitech.net.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://rj.szsharing.cn

[U99] JS：事件监听
来源：http://gz.jianghongdianzi.cn

el.addEventListener("click", e => {})
来源：http://nb.shtwfgs.cn

[U100] JS：DOM 查询
来源：http://xx.gzmigu.cn

document.querySelector(".item")
来源：http://ty.521024.cn

[U101] JS：classList 操作
来源：http://nu.szsharing.cn

el.classList.toggle("active")
来源：http://pa.bookmarksfly.cn

[U102] JS：本地存储
来源：http://zw.asd995.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ro.521024.cn

[U103] JS：定时器
来源：http://kf.huanxung.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ay.huixiangedu.cn

[U104] JS：防抖
来源：http://fz.panjiajie.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bk.hahajie.cn

[U105] JS：节流
来源：http://gd.colortex.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://rv.bjjhwx.cn

[U106] JS：日期格式化
来源：http://ww.jianghongdianzi.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://aj.shxzskj.cn

[U107] JS：数字千分位
来源：http://fa.hnjuh.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://nn.huixiangedu.cn

[U108] JS：随机整数
来源：http://sn.newstarts.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://of.szxytkj.cn

[U109] JS：数组分组
来源：http://vw.jctech888.com.cn

Object.groupBy(arr, x => x.type)
来源：http://pn.lnxyls.cn

[U110] JS：数组分块
来源：http://pb.nszjky.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://uc.shxzukj.cn

[U111] JS：对象转 Map
来源：http://vg.jctech888.com.cn

new Map(Object.entries(obj))
来源：http://kl.newstarts.cn

[U112] JS：字符串补位
来源：http://lq.lnxyls.cn

"7".padStart(3, "0")
来源：http://ay.9csxet.cn

[U113] JS：正则替换全部
来源：http://xv.bookmarksfly.cn

s.replaceAll("a", "b")
来源：http://kd.yuntaijiaju.cn

[U114] JS：JSON 深比较
来源：http://xe.newstarts.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://ny.bjjhwx.cn

[U115] JS：生成 UUID
来源：http://co.panjiajie.cn

crypto.randomUUID()
来源：http://zx.nicolike.cn

[U116] JS：类型检查（JSDoc）
来源：http://ln.asd995.cn

/** @param {string} name */ function f(name) {}
来源：http://rq.jctech888.com.cn

[U117] JS：单元测试
来源：http://bm.hahajie.cn

npm i -D vitest;  npx vitest
来源：http://iu.panjiajie.cn

[U118] JS：开发服务器
来源：http://wi.wgjwhj.cn

npm i -D vite;  npx vite
来源：http://dp.hahajie.cn

[U119] JS：生产构建
来源：http://mo.bjjhwx.cn

npx vite build
来源：http://hk.wgjwhj.cn

[U120] JS：读取环境变量（Vite）
来源：http://jx.huanxung.cn

import.meta.env.VITE_API_URL
来源：http://um.huixinmuqiang.cn

================================================================================
来源：http://ry.chemitech.net.cn

统计汇总
来源：http://bw.yuexingan06.cn

================================================================================
来源：http://rv.chemitech.net.cn

按语言统计（条）：
来源：http://gx.9csxet.cn

Python ......... 252
来源：http://ay.521024.cn

PHP ............ 252
来源：http://if.hahajie.cn

JavaScript ..... 252
来源：http://cx.nszjky.cn

TypeScript ..... 212
来源：http://ra.szsharing.cn

Java ........... 212
来源：http://zt.huixiangedu.cn

Go ............. 212
来源：http://ki.huanxung.cn

Ruby ........... 212
来源：http://vi.chemitech.net.cn

C# ............. 212
来源：http://fh.shxzskj.cn

C .............. 30
来源：http://ck.colortex.cn

C++ ............ 30
来源：http://tr.chemitech.net.cn

SQL ............ 90
来源：http://sw.jctech888.com.cn

Bash ........... 80
来源：http://bt.521024.cn

Kotlin ......... 15
来源：http://ui.gzmigu.cn

Swift .......... 15
来源：http://uv.nicolike.cn

Lua ............ 10
来源：http://qz.bjjhwx.cn

Perl ........... 10
来源：http://zp.panjiajie.cn

Scala .......... 10
来源：http://ve.chemitech.net.cn

------------------------------------
来源：http://at.hahajie.cn

合计 ........... 2106 条
来源：http://my.newstarts.cn

按章节统计：
来源：http://lr.gzmigu.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://di.shtwfgs.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mk.szxytkj.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://vn.asd995.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://kj.chemitech.net.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://pt.huixinmuqiang.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://vp.521024.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mq.asd995.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ds.chemitech.net.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://zm.yuntaijiaju.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://pe.szsharing.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://kz.lnxyls.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ot.bjjhwx.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ob.huanxung.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ow.huanxung.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://kv.yuexingan06.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ym.jianghongdianzi.cn

Q SQL 专题                              90
来源：http://uq.haigaiapp.cn

R Bash 专题                             80
来源：http://tx.huixinmuqiang.cn

S C / C++ 专题                          60
来源：http://ik.yuexingan06.cn

T 其他语言补充                          60
来源：http://qk.shxzskj.cn

U 高频实用片段                         120
来源：http://im.szxytkj.cn

------------------------------------
来源：http://xw.huixinmuqiang.cn

合计                                  2106 条
来源：http://sr.521024.cn

--------------------------------------------------------------------------------
来源：http://au.shtwfgs.cn

使用提醒
来源：http://fa.bookmarksfly.cn

--------------------------------------------------------------------------------
来源：http://xd.haigaiapp.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://by.muxihuayi.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://xk.bjjhwx.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://yo.panjiajie.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://ns.chemitech.net.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ol.jctech888.com.cn

—— 文件结束 ——
来源：http://ib.wgjwhj.cn

================================================================================
来源：http://oq.jctech888.com.cn

程序语言常见例子速查手册（2024 版）
来源：http://pa.shtwfgs.cn

Common Programming Examples Cheat Book
来源：http://ui.szsharing.cn

================================================================================
来源：http://os.huixinmuqiang.cn

【收录内容】
来源：http://ed.shtwfgs.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://nh.muxihuayi.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://fc.szsharing.cn

SQL · Bash · C · C++
来源：http://qi.newstarts.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://fl.lnxyls.cn

【使用说明】
来源：http://ls.bookmarksfly.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://vy.jctech888.com.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hg.nicolike.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hf.hnjuh.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://zc.bookmarksfly.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://pz.shxzukj.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ck.panjiajie.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://kw.haigaiapp.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://zf.szsharing.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://uo.asd995.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://fz.colortex.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hi.asd995.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://zg.huanxung.cn

【文件统计】
来源：http://ym.colortex.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://kw.haigaiapp.cn

--------------------------------------------------------------------------------
来源：http://an.szxytkj.cn

目  录
来源：http://nr.haigaiapp.cn

--------------------------------------------------------------------------------
来源：http://wb.huanxung.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://qt.asd995.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://wv.wgjwhj.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://rf.wgjwhj.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://xz.huixiangedu.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://sb.nicolike.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://kx.521024.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://ok.9csxet.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.yuexingan06.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ip.wgjwhj.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hv.szsharing.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://lf.hnjuh.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://nc.huixiangedu.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://xr.asd995.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://tn.jianghongdianzi.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ea.szsharing.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://ti.muxihuayi.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://at.yuntaijiaju.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://ug.hahajie.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://mi.newstarts.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ne.shtwfgs.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://zz.huixinmuqiang.cn

================================================================================
来源：http://rt.panjiajie.cn

A. 基础语法与类型
来源：http://yb.huixiangedu.cn

================================================================================
来源：http://wb.haigaiapp.cn

[A01] Hello World
来源：http://yv.jianghongdianzi.cn

Py:   print("Hello, World!")
来源：http://uj.yuntaijiaju.cn

PHP:  echo "Hello, World!";
来源：http://gq.muxihuayi.cn

JS:   console.log("Hello, World!");
来源：http://tz.bjjhwx.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://qw.lnxyls.cn

Java: System.out.println("Hello, World!");
来源：http://po.wgjwhj.cn

Go:   fmt.Println("Hello, World!")
来源：http://tw.jianghongdianzi.cn

Ruby: puts "Hello, World!"
来源：http://ha.colortex.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://zh.szsharing.cn

[A02] 变量声明与赋值
来源：http://wf.jianghongdianzi.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://vc.szxytkj.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://dn.newstarts.cn

JS:   let name = "Alex"; const age = 20;
来源：http://op.wgjwhj.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://uv.muxihuayi.cn

Java: String name = "Alex"; int age = 20;
来源：http://es.huanxung.cn

Go:   name := "Alex"; age := 20
来源：http://aj.9csxet.cn

Ruby: name = "Alex"; age = 20
来源：http://ou.bjjhwx.cn

C#:   string name = "Alex"; int age = 20;
来源：http://px.jctech888.com.cn

[A03] 常量定义
来源：http://fq.hnjuh.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://kk.huixiangedu.cn

PHP:  const PI = 3.14159;
来源：http://if.9csxet.cn

JS:   const PI = 3.14159;
来源：http://ss.chemitech.net.cn

TS:   const PI: number = 3.14159;
来源：http://pc.jianghongdianzi.cn

Java: static final double PI = 3.14159;
来源：http://sd.nszjky.cn

Go:   const PI = 3.14159
来源：http://je.lnxyls.cn

Ruby: PI = 3.14159
来源：http://ya.panjiajie.cn

C#:   const double PI = 3.14159;
来源：http://im.bookmarksfly.cn

[A04] 判断变量类型
来源：http://ol.haigaiapp.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://fx.jctech888.com.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://wk.jctech888.com.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://ix.bookmarksfly.cn

TS:   typeof x; x instanceof Date
来源：http://jf.szsharing.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://kw.9csxet.cn

Go:   reflect.TypeOf(x).Name()
来源：http://oc.asd995.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://hn.bjjhwx.cn

C#:   x.GetType().Name; x is int
来源：http://zf.muxihuayi.cn

[A05] 整数除法与取模
来源：http://xi.huixiangedu.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://fi.shtwfgs.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://aa.panjiajie.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://vq.gzmigu.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://zs.szxytkj.cn

Java: 7 / 2; 7 % 2
来源：http://lp.nszjky.cn

Go:   7 / 2; 7 % 2
来源：http://ia.9csxet.cn

Ruby: 7 / 2; 7 % 2
来源：http://yb.jianghongdianzi.cn

C#:   7 / 2; 7 % 2
来源：http://bj.chemitech.net.cn

[A06] 字符串转数字
来源：http://vb.bookmarksfly.cn

Py:   int("42"); float("3.14")
来源：http://km.shxzukj.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://eb.chemitech.net.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://fy.shtwfgs.cn

TS:   parseInt("42", 10); Number("42")
来源：http://xe.gzmigu.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://iq.colortex.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://mk.jctech888.com.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://ij.bookmarksfly.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://bl.szxytkj.cn

[A07] 数字转字符串
来源：http://gh.521024.cn

Py:   str(42)
来源：http://ue.shtwfgs.cn

PHP:  (string) 42; strval(42)
来源：http://ji.huanxung.cn


<!-- 参考信息 -->