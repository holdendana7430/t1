代发 wailian999

[U49] PHP：只读属性
来源：http://dn.hnjuh.cn

public readonly string $name
来源：http://hh.shxzukj.cn

[U50] PHP：构造器属性提升
来源：http://np.nszjky.cn

public function __construct(private int $id) {}
来源：http://zi.panjiajie.cn

[U51] PHP：数组解构
来源：http://xh.jctech888.com.cn

[$a, $b] = $arr;
来源：http://ai.asd995.cn

[U52] PHP：箭头函数
来源：http://cf.muxihuayi.cn

$double = fn($x) => $x * 2;
来源：http://fm.asd995.cn

[U53] PHP：空合并运算符
来源：http://it.hahajie.cn

$v = $a ?? $b ?? "default";
来源：http://po.shxzskj.cn

[U54] PHP：空安全调用
来源：http://xk.chemitech.net.cn

$obj?->method()
来源：http://st.haigaiapp.cn

[U55] PHP：match 表达式
来源：http://vb.521024.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://kq.asd995.cn

[U56] PHP：命名参数
来源：http://wu.szxytkj.cn

f(a: 1, b: 2)
来源：http://kf.gzmigu.cn

[U57] PHP：字符串插值
来源：http://um.szsharing.cn

"值: {$a}"
来源：http://bq.9csxet.cn

[U58] PHP：数组三件套
来源：http://dr.huixinmuqiang.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mp.newstarts.cn

[U59] PHP：自定义排序
来源：http://uq.yuntaijiaju.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mw.bookmarksfly.cn

[U60] PHP：JSON 编解码
来源：http://jc.gzmigu.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ek.gzmigu.cn

[U61] PHP：正则
来源：http://oa.521024.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://zc.szxytkj.cn

[U62] PHP：日期对象
来源：http://nl.muxihuayi.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://pq.panjiajie.cn

[U63] PHP：文件读写
来源：http://zr.shxzskj.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://qf.asd995.cn

[U64] PHP：目录遍历
来源：http://dj.wgjwhj.cn

glob("dir/*.php");  scandir("dir");
来源：http://qt.shxzukj.cn

[U65] PHP：会话
来源：http://lx.gzmigu.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://jn.asd995.cn

[U66] PHP：设置 Cookie
来源：http://ew.asd995.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://iw.jianghongdianzi.cn

[U67] PHP：处理文件上传
来源：http://kh.haigaiapp.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://fl.chemitech.net.cn

[U68] PHP：PDO 连接
来源：http://io.huixiangedu.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ge.chemitech.net.cn

[U69] PHP：PDO 预处理
来源：http://di.yuntaijiaju.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://fz.wgjwhj.cn

[U70] PHP：PDO 事务
来源：http://rr.gzmigu.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://bj.jctech888.com.cn

[U71] PHP：抛出异常
来源：http://pd.jianghongdianzi.cn

throw new RuntimeException("失败", 500);
来源：http://ke.hahajie.cn

[U72] PHP：写错误日志
来源：http://mw.muxihuayi.cn

error_log("失败: " . $e->getMessage());
来源：http://iy.huixiangedu.cn

[U73] PHP：读取 ini 配置
来源：http://ur.yuexingan06.cn

parse_ini_file("config.ini", true)
来源：http://xa.521024.cn

[U74] PHP：读取环境变量
来源：http://vy.huixinmuqiang.cn

getenv("APP_ENV") ?: "production"
来源：http://bs.szxytkj.cn

[U75] PHP：依赖注入
来源：http://yy.colortex.cn

composer require psr/container
来源：http://mm.9csxet.cn

[U76] PHP：简单路由
来源：http://al.colortex.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://fd.huixinmuqiang.cn

[U77] PHP：模板渲染
来源：http://fd.yuntaijiaju.cn

composer require twig/twig
来源：http://no.huixinmuqiang.cn

[U78] PHP：单元测试
来源：http://zs.panjiajie.cn

composer require --dev phpunit/phpunit
来源：http://lj.shtwfgs.cn

[U79] PHP：静态分析
来源：http://bx.bookmarksfly.cn

composer require --dev phpstan/phpstan
来源：http://fe.gzmigu.cn

[U80] PHP：代码规范修复
来源：http://vt.szxytkj.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://yq.haigaiapp.cn

[U81] JS：初始化项目
来源：http://pa.szxytkj.cn

npm init -y;  npm i express
来源：http://pb.colortex.cn

[U82] JS：package.json 脚本
来源：http://vg.szxytkj.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://eb.nicolike.cn

[U83] JS：ES Module 导入导出
来源：http://ko.wgjwhj.cn

export const a = 1;  import { a } from "./m.js";
来源：http://sw.gzmigu.cn

[U84] JS：CommonJS 写法
来源：http://ou.yuntaijiaju.cn

module.exports = { a };  const { a } = require("./m");
来源：http://qb.wgjwhj.cn

[U85] JS：可选链
来源：http://gd.9csxet.cn

a?.b?.c
来源：http://li.asd995.cn

[U86] JS：空值合并
来源：http://qk.yuntaijiaju.cn

a ?? b
来源：http://pl.9csxet.cn

[U87] JS：解构默认值
来源：http://rv.huanxung.cn

const { a = 1, b = 2 } = obj;
来源：http://lt.szxytkj.cn

[U88] JS：对象展开合并
来源：http://bw.newstarts.cn

{ ...a, ...b }
来源：http://zo.hahajie.cn

[U89] JS：数组去重
来源：http://pe.huixiangedu.cn

[...new Set(arr)]
来源：http://xj.gzmigu.cn

[U90] JS：数字数组排序
来源：http://lm.521024.cn

[...arr].sort((a, b) => a - b)
来源：http://rp.nicolike.cn

[U91] JS：对象键值遍历
来源：http://re.huanxung.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://rl.bjjhwx.cn

[U92] JS：深拷贝
来源：http://zo.shxzukj.cn

structuredClone(obj)
来源：http://ab.jctech888.com.cn

[U93] JS：模板字符串
来源：http://kt.muxihuayi.cn

`共 ${n} 条`
来源：http://gg.szsharing.cn

[U94] JS：箭头函数
来源：http://ck.wgjwhj.cn

const double = x => x * 2;
来源：http://nv.shxzukj.cn

[U95] JS：Promise 包装
来源：http://ku.colortex.cn

new Promise((resolve, reject) => {})
来源：http://te.shxzukj.cn

[U96] JS：async/await 与异常
来源：http://jh.shtwfgs.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ev.yuntaijiaju.cn

[U97] JS：并发请求
来源：http://yk.shxzukj.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://hj.bookmarksfly.cn

[U98] JS：fetch 带 JSON
来源：http://lb.muxihuayi.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://we.muxihuayi.cn

[U99] JS：事件监听
来源：http://iw.gzmigu.cn

el.addEventListener("click", e => {})
来源：http://um.huanxung.cn

[U100] JS：DOM 查询
来源：http://ok.521024.cn

document.querySelector(".item")
来源：http://kh.huixinmuqiang.cn

[U101] JS：classList 操作
来源：http://zs.szxytkj.cn

el.classList.toggle("active")
来源：http://fw.szxytkj.cn

[U102] JS：本地存储
来源：http://bx.521024.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://pz.shxzukj.cn

[U103] JS：定时器
来源：http://fa.szsharing.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://sb.lnxyls.cn

[U104] JS：防抖
来源：http://ws.hahajie.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jn.lnxyls.cn

[U105] JS：节流
来源：http://ls.nszjky.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://gt.shtwfgs.cn

[U106] JS：日期格式化
来源：http://ah.nicolike.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://yk.panjiajie.cn

[U107] JS：数字千分位
来源：http://yx.lnxyls.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://nq.chemitech.net.cn

[U108] JS：随机整数
来源：http://fh.9csxet.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ni.newstarts.cn

[U109] JS：数组分组
来源：http://pg.gzmigu.cn

Object.groupBy(arr, x => x.type)
来源：http://wr.hahajie.cn

[U110] JS：数组分块
来源：http://lp.huixiangedu.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://yr.huanxung.cn

[U111] JS：对象转 Map
来源：http://cp.huanxung.cn

new Map(Object.entries(obj))
来源：http://nz.huixiangedu.cn

[U112] JS：字符串补位
来源：http://yw.shxzskj.cn

"7".padStart(3, "0")
来源：http://dk.jctech888.com.cn

[U113] JS：正则替换全部
来源：http://il.huanxung.cn

s.replaceAll("a", "b")
来源：http://re.wgjwhj.cn

[U114] JS：JSON 深比较
来源：http://tk.lnxyls.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://hh.jianghongdianzi.cn

[U115] JS：生成 UUID
来源：http://np.huanxung.cn

crypto.randomUUID()
来源：http://wx.huanxung.cn

[U116] JS：类型检查（JSDoc）
来源：http://ke.newstarts.cn

/** @param {string} name */ function f(name) {}
来源：http://kd.nicolike.cn

[U117] JS：单元测试
来源：http://th.bookmarksfly.cn

npm i -D vitest;  npx vitest
来源：http://ep.nszjky.cn

[U118] JS：开发服务器
来源：http://si.bjjhwx.cn

npm i -D vite;  npx vite
来源：http://pg.huixinmuqiang.cn

[U119] JS：生产构建
来源：http://ym.colortex.cn

npx vite build
来源：http://uz.huixiangedu.cn

[U120] JS：读取环境变量（Vite）
来源：http://ss.huixinmuqiang.cn

import.meta.env.VITE_API_URL
来源：http://wv.chemitech.net.cn

================================================================================
来源：http://gw.hahajie.cn

统计汇总
来源：http://fi.huixinmuqiang.cn

================================================================================
来源：http://rx.yuntaijiaju.cn

按语言统计（条）：
来源：http://zr.521024.cn

Python ......... 252
来源：http://pc.huixiangedu.cn

PHP ............ 252
来源：http://xi.jctech888.com.cn

JavaScript ..... 252
来源：http://og.shxzskj.cn

TypeScript ..... 212
来源：http://mu.huanxung.cn

Java ........... 212
来源：http://zz.jctech888.com.cn

Go ............. 212
来源：http://lx.hahajie.cn

Ruby ........... 212
来源：http://wf.jctech888.com.cn

C# ............. 212
来源：http://wd.haigaiapp.cn

C .............. 30
来源：http://ak.yuntaijiaju.cn

C++ ............ 30
来源：http://el.yuntaijiaju.cn

SQL ............ 90
来源：http://xc.lnxyls.cn

Bash ........... 80
来源：http://kf.huixinmuqiang.cn

Kotlin ......... 15
来源：http://iv.huanxung.cn

Swift .......... 15
来源：http://qw.huixiangedu.cn

Lua ............ 10
来源：http://je.szsharing.cn

Perl ........... 10
来源：http://xr.szsharing.cn

Scala .......... 10
来源：http://kq.521024.cn

------------------------------------
来源：http://jp.nicolike.cn

合计 ........... 2106 条
来源：http://zx.huanxung.cn

按章节统计：
来源：http://ej.chemitech.net.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://gm.yuntaijiaju.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://um.muxihuayi.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://rs.huanxung.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://vz.jianghongdianzi.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://cu.haigaiapp.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://qf.bookmarksfly.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wu.hnjuh.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://zs.jctech888.com.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://yf.nszjky.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://xo.huixiangedu.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://uv.shxzukj.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://fq.nicolike.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://it.muxihuayi.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ts.9csxet.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://qv.szsharing.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://dt.wgjwhj.cn

Q SQL 专题                              90
来源：http://jm.jctech888.com.cn

R Bash 专题                             80
来源：http://ll.nicolike.cn

S C / C++ 专题                          60
来源：http://nq.muxihuayi.cn

T 其他语言补充                          60
来源：http://pq.shxzukj.cn

U 高频实用片段                         120
来源：http://wd.szxytkj.cn

------------------------------------
来源：http://jf.9csxet.cn

合计                                  2106 条
来源：http://aj.szsharing.cn

--------------------------------------------------------------------------------
来源：http://fy.hnjuh.cn

使用提醒
来源：http://yc.shtwfgs.cn

--------------------------------------------------------------------------------
来源：http://rd.nszjky.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ml.bookmarksfly.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://oi.muxihuayi.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ta.jctech888.com.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://qc.huanxung.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hh.9csxet.cn

—— 文件结束 ——
来源：http://av.gzmigu.cn

================================================================================
来源：http://dn.shtwfgs.cn

程序语言常见例子速查手册（2024 版）
来源：http://ra.asd995.cn

Common Programming Examples Cheat Book
来源：http://ak.panjiajie.cn

================================================================================
来源：http://ng.jianghongdianzi.cn

【收录内容】
来源：http://gm.huixinmuqiang.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://ho.hnjuh.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://xr.huanxung.cn

SQL · Bash · C · C++
来源：http://dw.hnjuh.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://qt.chemitech.net.cn

【使用说明】
来源：http://rp.hnjuh.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hd.bookmarksfly.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://nf.shxzskj.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://qm.521024.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://zf.jianghongdianzi.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://fa.shxzskj.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://sk.szxytkj.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ku.shxzskj.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://lu.9csxet.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://sh.jianghongdianzi.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://jo.jctech888.com.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://qq.chemitech.net.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://rk.jctech888.com.cn

【文件统计】
来源：http://wo.521024.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ik.9csxet.cn

--------------------------------------------------------------------------------
来源：http://zx.nszjky.cn

目  录
来源：http://kk.bookmarksfly.cn

--------------------------------------------------------------------------------
来源：http://yt.yuexingan06.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://wk.jctech888.com.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://dl.9csxet.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://ln.haigaiapp.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://vp.huixiangedu.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://bs.yuexingan06.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://mi.chemitech.net.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://ri.colortex.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://sr.huixinmuqiang.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://nr.haigaiapp.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://yw.huixinmuqiang.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://fj.gzmigu.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://cl.newstarts.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://so.asd995.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ey.chemitech.net.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://aq.bjjhwx.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://za.haigaiapp.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://xo.521024.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://tu.newstarts.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://pd.jianghongdianzi.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://xi.huixiangedu.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://oa.9csxet.cn

================================================================================
来源：http://an.chemitech.net.cn

A. 基础语法与类型
来源：http://xu.shxzskj.cn

================================================================================
来源：http://ql.bjjhwx.cn

[A01] Hello World
来源：http://ak.nicolike.cn

Py:   print("Hello, World!")
来源：http://fx.shxzskj.cn

PHP:  echo "Hello, World!";
来源：http://ze.bookmarksfly.cn

JS:   console.log("Hello, World!");
来源：http://jy.shtwfgs.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ym.newstarts.cn

Java: System.out.println("Hello, World!");
来源：http://ll.yuntaijiaju.cn

Go:   fmt.Println("Hello, World!")
来源：http://iu.nicolike.cn

Ruby: puts "Hello, World!"
来源：http://gz.asd995.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://lc.9csxet.cn

[A02] 变量声明与赋值
来源：http://sp.huanxung.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://fh.hnjuh.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://rc.bookmarksfly.cn

JS:   let name = "Alex"; const age = 20;
来源：http://bw.huixiangedu.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://pw.huixinmuqiang.cn

Java: String name = "Alex"; int age = 20;
来源：http://mg.shxzskj.cn

Go:   name := "Alex"; age := 20
来源：http://hk.9csxet.cn

Ruby: name = "Alex"; age = 20
来源：http://uy.jianghongdianzi.cn

C#:   string name = "Alex"; int age = 20;
来源：http://zu.yuntaijiaju.cn

[A03] 常量定义
来源：http://dc.lnxyls.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://qp.nszjky.cn

PHP:  const PI = 3.14159;
来源：http://zj.huanxung.cn

JS:   const PI = 3.14159;
来源：http://pt.yuexingan06.cn

TS:   const PI: number = 3.14159;
来源：http://ea.huanxung.cn

Java: static final double PI = 3.14159;
来源：http://mk.hahajie.cn

Go:   const PI = 3.14159
来源：http://yv.newstarts.cn

Ruby: PI = 3.14159
来源：http://jb.muxihuayi.cn

C#:   const double PI = 3.14159;
来源：http://gu.bjjhwx.cn

[A04] 判断变量类型
来源：http://ny.hahajie.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://zt.bookmarksfly.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://bt.bjjhwx.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://un.hnjuh.cn

TS:   typeof x; x instanceof Date
来源：http://un.bjjhwx.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://od.panjiajie.cn

Go:   reflect.TypeOf(x).Name()
来源：http://zt.bookmarksfly.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://wy.bjjhwx.cn

C#:   x.GetType().Name; x is int
来源：http://hg.521024.cn

[A05] 整数除法与取模
来源：http://ov.shxzskj.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://jc.huixinmuqiang.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://lc.lnxyls.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://vg.9csxet.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://jq.hnjuh.cn

Java: 7 / 2; 7 % 2
来源：http://in.jctech888.com.cn

Go:   7 / 2; 7 % 2
来源：http://my.shxzskj.cn

Ruby: 7 / 2; 7 % 2
来源：http://zk.asd995.cn

C#:   7 / 2; 7 % 2
来源：http://ql.jctech888.com.cn

[A06] 字符串转数字
来源：http://xb.colortex.cn

Py:   int("42"); float("3.14")
来源：http://jg.newstarts.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://dt.hahajie.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://zc.yuntaijiaju.cn


<!-- 参考信息 -->