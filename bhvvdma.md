代发 wailian999

[U49] PHP：只读属性
来源：http://zb.chemitech.net.cn

public readonly string $name
来源：http://np.colortex.cn

[U50] PHP：构造器属性提升
来源：http://wc.jctech888.com.cn

public function __construct(private int $id) {}
来源：http://ot.szxytkj.cn

[U51] PHP：数组解构
来源：http://ju.hahajie.cn

[$a, $b] = $arr;
来源：http://uc.huixiangedu.cn

[U52] PHP：箭头函数
来源：http://tu.newstarts.cn

$double = fn($x) => $x * 2;
来源：http://tz.yuntaijiaju.cn

[U53] PHP：空合并运算符
来源：http://hc.colortex.cn

$v = $a ?? $b ?? "default";
来源：http://la.huixinmuqiang.cn

[U54] PHP：空安全调用
来源：http://qp.lnxyls.cn

$obj?->method()
来源：http://gn.chemitech.net.cn

[U55] PHP：match 表达式
来源：http://re.jctech888.com.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ys.chemitech.net.cn

[U56] PHP：命名参数
来源：http://wl.szsharing.cn

f(a: 1, b: 2)
来源：http://sd.lnxyls.cn

[U57] PHP：字符串插值
来源：http://fl.shtwfgs.cn

"值: {$a}"
来源：http://ox.huixiangedu.cn

[U58] PHP：数组三件套
来源：http://uu.hahajie.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ry.muxihuayi.cn

[U59] PHP：自定义排序
来源：http://fl.huixiangedu.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://gr.muxihuayi.cn

[U60] PHP：JSON 编解码
来源：http://cz.shxzukj.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://kf.521024.cn

[U61] PHP：正则
来源：http://uw.521024.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://vo.panjiajie.cn

[U62] PHP：日期对象
来源：http://uy.nicolike.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ef.9csxet.cn

[U63] PHP：文件读写
来源：http://qx.muxihuayi.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://lj.asd995.cn

[U64] PHP：目录遍历
来源：http://xk.jianghongdianzi.cn

glob("dir/*.php");  scandir("dir");
来源：http://un.bookmarksfly.cn

[U65] PHP：会话
来源：http://kq.wgjwhj.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://uv.hnjuh.cn

[U66] PHP：设置 Cookie
来源：http://ph.jctech888.com.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://fg.huanxung.cn

[U67] PHP：处理文件上传
来源：http://qz.gzmigu.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://yj.shxzskj.cn

[U68] PHP：PDO 连接
来源：http://uu.lnxyls.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ni.huixinmuqiang.cn

[U69] PHP：PDO 预处理
来源：http://xj.colortex.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://km.nicolike.cn

[U70] PHP：PDO 事务
来源：http://zb.yuexingan06.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://td.9csxet.cn

[U71] PHP：抛出异常
来源：http://oe.yuntaijiaju.cn

throw new RuntimeException("失败", 500);
来源：http://wf.muxihuayi.cn

[U72] PHP：写错误日志
来源：http://ap.bookmarksfly.cn

error_log("失败: " . $e->getMessage());
来源：http://of.gzmigu.cn

[U73] PHP：读取 ini 配置
来源：http://xb.szsharing.cn

parse_ini_file("config.ini", true)
来源：http://jl.wgjwhj.cn

[U74] PHP：读取环境变量
来源：http://co.huanxung.cn

getenv("APP_ENV") ?: "production"
来源：http://ly.muxihuayi.cn

[U75] PHP：依赖注入
来源：http://lv.bookmarksfly.cn

composer require psr/container
来源：http://ko.muxihuayi.cn

[U76] PHP：简单路由
来源：http://uv.jctech888.com.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://nr.huanxung.cn

[U77] PHP：模板渲染
来源：http://ak.nszjky.cn

composer require twig/twig
来源：http://cy.jctech888.com.cn

[U78] PHP：单元测试
来源：http://kc.shxzskj.cn

composer require --dev phpunit/phpunit
来源：http://yr.wgjwhj.cn

[U79] PHP：静态分析
来源：http://rm.yuntaijiaju.cn

composer require --dev phpstan/phpstan
来源：http://nl.521024.cn

[U80] PHP：代码规范修复
来源：http://qx.nicolike.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://ys.shxzukj.cn

[U81] JS：初始化项目
来源：http://iq.nszjky.cn

npm init -y;  npm i express
来源：http://tz.szsharing.cn

[U82] JS：package.json 脚本
来源：http://st.yuexingan06.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://dl.chemitech.net.cn

[U83] JS：ES Module 导入导出
来源：http://tg.nicolike.cn

export const a = 1;  import { a } from "./m.js";
来源：http://ql.nszjky.cn

[U84] JS：CommonJS 写法
来源：http://ef.nszjky.cn

module.exports = { a };  const { a } = require("./m");
来源：http://pm.yuntaijiaju.cn

[U85] JS：可选链
来源：http://yf.chemitech.net.cn

a?.b?.c
来源：http://xg.muxihuayi.cn

[U86] JS：空值合并
来源：http://ts.gzmigu.cn

a ?? b
来源：http://gl.asd995.cn

[U87] JS：解构默认值
来源：http://fg.jctech888.com.cn

const { a = 1, b = 2 } = obj;
来源：http://la.yuntaijiaju.cn

[U88] JS：对象展开合并
来源：http://oe.lnxyls.cn

{ ...a, ...b }
来源：http://zb.yuexingan06.cn

[U89] JS：数组去重
来源：http://gu.huixiangedu.cn

[...new Set(arr)]
来源：http://sm.shtwfgs.cn

[U90] JS：数字数组排序
来源：http://bx.9csxet.cn

[...arr].sort((a, b) => a - b)
来源：http://se.shxzskj.cn

[U91] JS：对象键值遍历
来源：http://nn.nicolike.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://nz.lnxyls.cn

[U92] JS：深拷贝
来源：http://jf.asd995.cn

structuredClone(obj)
来源：http://nk.jctech888.com.cn

[U93] JS：模板字符串
来源：http://wd.newstarts.cn

`共 ${n} 条`
来源：http://sj.shxzskj.cn

[U94] JS：箭头函数
来源：http://fv.huixinmuqiang.cn

const double = x => x * 2;
来源：http://hh.shxzukj.cn

[U95] JS：Promise 包装
来源：http://tq.muxihuayi.cn

new Promise((resolve, reject) => {})
来源：http://ak.jctech888.com.cn

[U96] JS：async/await 与异常
来源：http://vz.hahajie.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://dp.lnxyls.cn

[U97] JS：并发请求
来源：http://zy.shtwfgs.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://wr.colortex.cn

[U98] JS：fetch 带 JSON
来源：http://cp.hahajie.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://vr.wgjwhj.cn

[U99] JS：事件监听
来源：http://ok.521024.cn

el.addEventListener("click", e => {})
来源：http://si.muxihuayi.cn

[U100] JS：DOM 查询
来源：http://zf.yuntaijiaju.cn

document.querySelector(".item")
来源：http://uf.yuexingan06.cn

[U101] JS：classList 操作
来源：http://cn.haigaiapp.cn

el.classList.toggle("active")
来源：http://sq.wgjwhj.cn

[U102] JS：本地存储
来源：http://sb.asd995.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://do.panjiajie.cn

[U103] JS：定时器
来源：http://fn.jctech888.com.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://kx.yuexingan06.cn

[U104] JS：防抖
来源：http://rs.521024.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://sc.hahajie.cn

[U105] JS：节流
来源：http://lr.hahajie.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://bp.szsharing.cn

[U106] JS：日期格式化
来源：http://iz.nicolike.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://if.bookmarksfly.cn

[U107] JS：数字千分位
来源：http://ze.chemitech.net.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://op.asd995.cn

[U108] JS：随机整数
来源：http://ky.colortex.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://js.huixinmuqiang.cn

[U109] JS：数组分组
来源：http://eu.lnxyls.cn

Object.groupBy(arr, x => x.type)
来源：http://uy.bjjhwx.cn

[U110] JS：数组分块
来源：http://sv.hnjuh.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://bg.jianghongdianzi.cn

[U111] JS：对象转 Map
来源：http://ev.nicolike.cn

new Map(Object.entries(obj))
来源：http://jz.yuntaijiaju.cn

[U112] JS：字符串补位
来源：http://vp.muxihuayi.cn

"7".padStart(3, "0")
来源：http://jq.jctech888.com.cn

[U113] JS：正则替换全部
来源：http://ar.huanxung.cn

s.replaceAll("a", "b")
来源：http://pd.bookmarksfly.cn

[U114] JS：JSON 深比较
来源：http://uv.hahajie.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://ep.jianghongdianzi.cn

[U115] JS：生成 UUID
来源：http://uv.shtwfgs.cn

crypto.randomUUID()
来源：http://yf.newstarts.cn

[U116] JS：类型检查（JSDoc）
来源：http://br.muxihuayi.cn

/** @param {string} name */ function f(name) {}
来源：http://fn.chemitech.net.cn

[U117] JS：单元测试
来源：http://gc.521024.cn

npm i -D vitest;  npx vitest
来源：http://gb.panjiajie.cn

[U118] JS：开发服务器
来源：http://op.muxihuayi.cn

npm i -D vite;  npx vite
来源：http://mv.521024.cn

[U119] JS：生产构建
来源：http://rv.haigaiapp.cn

npx vite build
来源：http://ji.9csxet.cn

[U120] JS：读取环境变量（Vite）
来源：http://xy.yuexingan06.cn

import.meta.env.VITE_API_URL
来源：http://gi.muxihuayi.cn

================================================================================
来源：http://er.lnxyls.cn

统计汇总
来源：http://tp.hnjuh.cn

================================================================================
来源：http://ry.hnjuh.cn

按语言统计（条）：
来源：http://eg.nicolike.cn

Python ......... 252
来源：http://ij.muxihuayi.cn

PHP ............ 252
来源：http://mp.jctech888.com.cn

JavaScript ..... 252
来源：http://ol.9csxet.cn

TypeScript ..... 212
来源：http://sq.wgjwhj.cn

Java ........... 212
来源：http://hp.shxzukj.cn

Go ............. 212
来源：http://ha.huixiangedu.cn

Ruby ........... 212
来源：http://lg.huanxung.cn

C# ............. 212
来源：http://zt.jianghongdianzi.cn

C .............. 30
来源：http://zy.hnjuh.cn

C++ ............ 30
来源：http://ka.bjjhwx.cn

SQL ............ 90
来源：http://sn.newstarts.cn

Bash ........... 80
来源：http://be.wgjwhj.cn

Kotlin ......... 15
来源：http://ad.huixiangedu.cn

Swift .......... 15
来源：http://qt.hahajie.cn

Lua ............ 10
来源：http://oy.huixinmuqiang.cn

Perl ........... 10
来源：http://va.huanxung.cn

Scala .......... 10
来源：http://bk.huixinmuqiang.cn

------------------------------------
来源：http://nt.asd995.cn

合计 ........... 2106 条
来源：http://jt.bjjhwx.cn

按章节统计：
来源：http://fd.haigaiapp.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ot.bjjhwx.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://jj.gzmigu.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ou.chemitech.net.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://cj.newstarts.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ve.lnxyls.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://zw.asd995.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://zs.shtwfgs.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://od.panjiajie.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://kw.wgjwhj.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ge.huixiangedu.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://xt.wgjwhj.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://yc.huixiangedu.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://vy.panjiajie.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ep.huixiangedu.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://qe.muxihuayi.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://cj.newstarts.cn

Q SQL 专题                              90
来源：http://md.shtwfgs.cn

R Bash 专题                             80
来源：http://nu.huixiangedu.cn

S C / C++ 专题                          60
来源：http://az.9csxet.cn

T 其他语言补充                          60
来源：http://qt.szsharing.cn

U 高频实用片段                         120
来源：http://ks.bookmarksfly.cn

------------------------------------
来源：http://pq.huixinmuqiang.cn

合计                                  2106 条
来源：http://wu.yuntaijiaju.cn

--------------------------------------------------------------------------------
来源：http://zp.szxytkj.cn

使用提醒
来源：http://fa.521024.cn

--------------------------------------------------------------------------------
来源：http://fj.shxzskj.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wt.asd995.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://zy.huixiangedu.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://we.shtwfgs.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://qi.nicolike.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://sf.yuexingan06.cn

—— 文件结束 ——
来源：http://tp.9csxet.cn

================================================================================
来源：http://nd.newstarts.cn

程序语言常见例子速查手册（2024 版）
来源：http://lk.bookmarksfly.cn

Common Programming Examples Cheat Book
来源：http://fx.wgjwhj.cn

================================================================================
来源：http://xb.9csxet.cn

【收录内容】
来源：http://xq.chemitech.net.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://oh.lnxyls.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://tu.yuntaijiaju.cn

SQL · Bash · C · C++
来源：http://yl.szxytkj.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wd.shxzskj.cn

【使用说明】
来源：http://rq.521024.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://kc.yuexingan06.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://gw.newstarts.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://co.huixinmuqiang.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ft.panjiajie.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://ma.shxzukj.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://zz.521024.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://bl.huixiangedu.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://cd.shtwfgs.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://zg.huanxung.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://gm.szsharing.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ks.szxytkj.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://od.nicolike.cn

【文件统计】
来源：http://vm.asd995.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://xb.9csxet.cn

--------------------------------------------------------------------------------
来源：http://hp.yuexingan06.cn

目  录
来源：http://vm.hnjuh.cn

--------------------------------------------------------------------------------
来源：http://mp.gzmigu.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://kx.szxytkj.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://lg.9csxet.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://xx.wgjwhj.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://mw.shtwfgs.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://ye.yuntaijiaju.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://uy.muxihuayi.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://qq.521024.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://pf.colortex.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://dl.huixiangedu.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://sh.huanxung.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://bx.gzmigu.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://wb.huanxung.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://yj.9csxet.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ge.huanxung.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://pf.colortex.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hq.muxihuayi.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://yf.gzmigu.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://gb.chemitech.net.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://iy.newstarts.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://is.nicolike.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://ce.hnjuh.cn

================================================================================
来源：http://jw.szxytkj.cn

A. 基础语法与类型
来源：http://bs.lnxyls.cn

================================================================================
来源：http://zi.newstarts.cn

[A01] Hello World
来源：http://qd.lnxyls.cn

Py:   print("Hello, World!")
来源：http://al.jctech888.com.cn

PHP:  echo "Hello, World!";
来源：http://aa.bookmarksfly.cn

JS:   console.log("Hello, World!");
来源：http://mz.huixiangedu.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://qh.gzmigu.cn

Java: System.out.println("Hello, World!");
来源：http://ds.yuexingan06.cn

Go:   fmt.Println("Hello, World!")
来源：http://im.nszjky.cn

Ruby: puts "Hello, World!"
来源：http://gc.shxzskj.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://rj.colortex.cn

[A02] 变量声明与赋值
来源：http://kv.jctech888.com.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://lk.shtwfgs.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://yr.asd995.cn

JS:   let name = "Alex"; const age = 20;
来源：http://og.521024.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://bf.jctech888.com.cn

Java: String name = "Alex"; int age = 20;
来源：http://yd.lnxyls.cn

Go:   name := "Alex"; age := 20
来源：http://zb.huanxung.cn

Ruby: name = "Alex"; age = 20
来源：http://cw.hnjuh.cn

C#:   string name = "Alex"; int age = 20;
来源：http://il.huixinmuqiang.cn

[A03] 常量定义
来源：http://ly.9csxet.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://vw.wgjwhj.cn

PHP:  const PI = 3.14159;
来源：http://ve.chemitech.net.cn

JS:   const PI = 3.14159;
来源：http://ux.hahajie.cn

TS:   const PI: number = 3.14159;
来源：http://ke.jctech888.com.cn

Java: static final double PI = 3.14159;
来源：http://gz.huanxung.cn

Go:   const PI = 3.14159
来源：http://rc.yuntaijiaju.cn

Ruby: PI = 3.14159
来源：http://rq.jianghongdianzi.cn

C#:   const double PI = 3.14159;
来源：http://bw.yuntaijiaju.cn

[A04] 判断变量类型
来源：http://ih.szsharing.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://bc.yuntaijiaju.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://te.bookmarksfly.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://bh.colortex.cn

TS:   typeof x; x instanceof Date
来源：http://tt.shxzskj.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ps.haigaiapp.cn

Go:   reflect.TypeOf(x).Name()
来源：http://ze.nszjky.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://cf.huixiangedu.cn

C#:   x.GetType().Name; x is int
来源：http://cr.bookmarksfly.cn

[A05] 整数除法与取模
来源：http://em.521024.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://nd.asd995.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://ax.gzmigu.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://tw.yuntaijiaju.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://wj.newstarts.cn

Java: 7 / 2; 7 % 2
来源：http://mh.huixinmuqiang.cn

Go:   7 / 2; 7 % 2
来源：http://xp.huanxung.cn

Ruby: 7 / 2; 7 % 2
来源：http://ae.shxzskj.cn

C#:   7 / 2; 7 % 2
来源：http://mi.haigaiapp.cn

[A06] 字符串转数字
来源：http://gg.asd995.cn

Py:   int("42"); float("3.14")
来源：http://mh.521024.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://lb.huixinmuqiang.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://vm.wgjwhj.cn


<!-- 参考信息 -->