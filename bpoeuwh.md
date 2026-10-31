代发 wailian999

[U47] PHP：联合类型
来源：http://rh.9csxet.cn

int|string $id
来源：http://wv.shxzskj.cn

[U48] PHP：纯枚举
来源：http://gw.bjjhwx.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://jo.shxzukj.cn

[U49] PHP：只读属性
来源：http://py.shtwfgs.cn

public readonly string $name
来源：http://wy.jianghongdianzi.cn

[U50] PHP：构造器属性提升
来源：http://ui.huanxung.cn

public function __construct(private int $id) {}
来源：http://pu.newstarts.cn

[U51] PHP：数组解构
来源：http://ws.newstarts.cn

[$a, $b] = $arr;
来源：http://st.hnjuh.cn

[U52] PHP：箭头函数
来源：http://qq.shxzskj.cn

$double = fn($x) => $x * 2;
来源：http://bp.hnjuh.cn

[U53] PHP：空合并运算符
来源：http://qp.yuexingan06.cn

$v = $a ?? $b ?? "default";
来源：http://hh.szsharing.cn

[U54] PHP：空安全调用
来源：http://oi.newstarts.cn

$obj?->method()
来源：http://li.hnjuh.cn

[U55] PHP：match 表达式
来源：http://su.huanxung.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://sh.yuntaijiaju.cn

[U56] PHP：命名参数
来源：http://kp.bjjhwx.cn

f(a: 1, b: 2)
来源：http://kv.chemitech.net.cn

[U57] PHP：字符串插值
来源：http://fo.colortex.cn

"值: {$a}"
来源：http://rm.lnxyls.cn

[U58] PHP：数组三件套
来源：http://vq.hahajie.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://nt.muxihuayi.cn

[U59] PHP：自定义排序
来源：http://uh.colortex.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://gc.shxzskj.cn

[U60] PHP：JSON 编解码
来源：http://yb.hnjuh.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://pf.bookmarksfly.cn

[U61] PHP：正则
来源：http://gl.gzmigu.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://jk.haigaiapp.cn

[U62] PHP：日期对象
来源：http://lj.colortex.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ii.huixiangedu.cn

[U63] PHP：文件读写
来源：http://rv.521024.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://is.panjiajie.cn

[U64] PHP：目录遍历
来源：http://wx.huixiangedu.cn

glob("dir/*.php");  scandir("dir");
来源：http://my.huixinmuqiang.cn

[U65] PHP：会话
来源：http://cr.521024.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://dh.shxzskj.cn

[U66] PHP：设置 Cookie
来源：http://eu.gzmigu.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://pu.chemitech.net.cn

[U67] PHP：处理文件上传
来源：http://pa.huixinmuqiang.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://zt.huixinmuqiang.cn

[U68] PHP：PDO 连接
来源：http://cu.asd995.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://nd.wgjwhj.cn

[U69] PHP：PDO 预处理
来源：http://nx.haigaiapp.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://oq.nicolike.cn

[U70] PHP：PDO 事务
来源：http://as.lnxyls.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://jy.szsharing.cn

[U71] PHP：抛出异常
来源：http://ow.szsharing.cn

throw new RuntimeException("失败", 500);
来源：http://ma.szsharing.cn

[U72] PHP：写错误日志
来源：http://uv.szsharing.cn

error_log("失败: " . $e->getMessage());
来源：http://rf.asd995.cn

[U73] PHP：读取 ini 配置
来源：http://bd.bookmarksfly.cn

parse_ini_file("config.ini", true)
来源：http://cv.shxzskj.cn

[U74] PHP：读取环境变量
来源：http://ie.asd995.cn

getenv("APP_ENV") ?: "production"
来源：http://mp.lnxyls.cn

[U75] PHP：依赖注入
来源：http://th.nicolike.cn

composer require psr/container
来源：http://jw.521024.cn

[U76] PHP：简单路由
来源：http://jx.bjjhwx.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mg.yuexingan06.cn

[U77] PHP：模板渲染
来源：http://bo.huanxung.cn

composer require twig/twig
来源：http://xr.yuexingan06.cn

[U78] PHP：单元测试
来源：http://al.shxzskj.cn

composer require --dev phpunit/phpunit
来源：http://es.nszjky.cn

[U79] PHP：静态分析
来源：http://uw.9csxet.cn

composer require --dev phpstan/phpstan
来源：http://sw.panjiajie.cn

[U80] PHP：代码规范修复
来源：http://fx.gzmigu.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://fw.shxzskj.cn

[U81] JS：初始化项目
来源：http://qe.shtwfgs.cn

npm init -y;  npm i express
来源：http://sd.nicolike.cn

[U82] JS：package.json 脚本
来源：http://bw.hnjuh.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://qq.jctech888.com.cn

[U83] JS：ES Module 导入导出
来源：http://cm.szxytkj.cn

export const a = 1;  import { a } from "./m.js";
来源：http://yo.jctech888.com.cn

[U84] JS：CommonJS 写法
来源：http://su.gzmigu.cn

module.exports = { a };  const { a } = require("./m");
来源：http://ld.shxzukj.cn

[U85] JS：可选链
来源：http://vj.521024.cn

a?.b?.c
来源：http://ck.9csxet.cn

[U86] JS：空值合并
来源：http://fq.521024.cn

a ?? b
来源：http://fa.bjjhwx.cn

[U87] JS：解构默认值
来源：http://ei.9csxet.cn

const { a = 1, b = 2 } = obj;
来源：http://jv.shxzukj.cn

[U88] JS：对象展开合并
来源：http://gx.szxytkj.cn

{ ...a, ...b }
来源：http://xn.panjiajie.cn

[U89] JS：数组去重
来源：http://ii.hnjuh.cn

[...new Set(arr)]
来源：http://xb.bookmarksfly.cn

[U90] JS：数字数组排序
来源：http://vm.asd995.cn

[...arr].sort((a, b) => a - b)
来源：http://jb.yuntaijiaju.cn

[U91] JS：对象键值遍历
来源：http://gw.lnxyls.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ph.shxzskj.cn

[U92] JS：深拷贝
来源：http://re.bjjhwx.cn

structuredClone(obj)
来源：http://vy.huixiangedu.cn

[U93] JS：模板字符串
来源：http://ls.asd995.cn

`共 ${n} 条`
来源：http://ap.9csxet.cn

[U94] JS：箭头函数
来源：http://dk.huixiangedu.cn

const double = x => x * 2;
来源：http://fg.521024.cn

[U95] JS：Promise 包装
来源：http://yy.asd995.cn

new Promise((resolve, reject) => {})
来源：http://pk.bjjhwx.cn

[U96] JS：async/await 与异常
来源：http://jc.haigaiapp.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://fp.yuntaijiaju.cn

[U97] JS：并发请求
来源：http://gu.muxihuayi.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://jy.bjjhwx.cn

[U98] JS：fetch 带 JSON
来源：http://ad.szsharing.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://dr.huixiangedu.cn

[U99] JS：事件监听
来源：http://uz.nicolike.cn

el.addEventListener("click", e => {})
来源：http://dm.lnxyls.cn

[U100] JS：DOM 查询
来源：http://ly.hnjuh.cn

document.querySelector(".item")
来源：http://ku.colortex.cn

[U101] JS：classList 操作
来源：http://oq.yuexingan06.cn

el.classList.toggle("active")
来源：http://dp.huanxung.cn

[U102] JS：本地存储
来源：http://uh.panjiajie.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://as.haigaiapp.cn

[U103] JS：定时器
来源：http://ff.521024.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mm.bjjhwx.cn

[U104] JS：防抖
来源：http://mx.bookmarksfly.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://sx.haigaiapp.cn

[U105] JS：节流
来源：http://pf.lnxyls.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://sq.haigaiapp.cn

[U106] JS：日期格式化
来源：http://vk.nszjky.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://us.hnjuh.cn

[U107] JS：数字千分位
来源：http://ri.chemitech.net.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://km.gzmigu.cn

[U108] JS：随机整数
来源：http://og.huixiangedu.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://cp.newstarts.cn

[U109] JS：数组分组
来源：http://zs.huanxung.cn

Object.groupBy(arr, x => x.type)
来源：http://kz.haigaiapp.cn

[U110] JS：数组分块
来源：http://zr.newstarts.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hn.wgjwhj.cn

[U111] JS：对象转 Map
来源：http://ys.shxzskj.cn

new Map(Object.entries(obj))
来源：http://jb.wgjwhj.cn

[U112] JS：字符串补位
来源：http://su.haigaiapp.cn

"7".padStart(3, "0")
来源：http://qw.colortex.cn

[U113] JS：正则替换全部
来源：http://ry.colortex.cn

s.replaceAll("a", "b")
来源：http://yg.9csxet.cn

[U114] JS：JSON 深比较
来源：http://ta.jianghongdianzi.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://aj.huanxung.cn

[U115] JS：生成 UUID
来源：http://mr.muxihuayi.cn

crypto.randomUUID()
来源：http://mj.jctech888.com.cn

[U116] JS：类型检查（JSDoc）
来源：http://ss.panjiajie.cn

/** @param {string} name */ function f(name) {}
来源：http://oz.bjjhwx.cn

[U117] JS：单元测试
来源：http://zi.shxzukj.cn

npm i -D vitest;  npx vitest
来源：http://wj.jctech888.com.cn

[U118] JS：开发服务器
来源：http://zt.gzmigu.cn

npm i -D vite;  npx vite
来源：http://ch.huanxung.cn

[U119] JS：生产构建
来源：http://sb.wgjwhj.cn

npx vite build
来源：http://xj.hnjuh.cn

[U120] JS：读取环境变量（Vite）
来源：http://el.shxzukj.cn

import.meta.env.VITE_API_URL
来源：http://oj.nszjky.cn

================================================================================
来源：http://ee.jctech888.com.cn

统计汇总
来源：http://wd.hnjuh.cn

================================================================================
来源：http://ks.szsharing.cn

按语言统计（条）：
来源：http://xb.chemitech.net.cn

Python ......... 252
来源：http://jn.colortex.cn

PHP ............ 252
来源：http://wg.jctech888.com.cn

JavaScript ..... 252
来源：http://yt.bookmarksfly.cn

TypeScript ..... 212
来源：http://zm.chemitech.net.cn

Java ........... 212
来源：http://uj.hnjuh.cn

Go ............. 212
来源：http://tm.panjiajie.cn

Ruby ........... 212
来源：http://ov.lnxyls.cn

C# ............. 212
来源：http://jm.huixiangedu.cn

C .............. 30
来源：http://dn.shtwfgs.cn

C++ ............ 30
来源：http://gm.yuexingan06.cn

SQL ............ 90
来源：http://cr.chemitech.net.cn

Bash ........... 80
来源：http://ck.gzmigu.cn

Kotlin ......... 15
来源：http://it.asd995.cn

Swift .......... 15
来源：http://hw.gzmigu.cn

Lua ............ 10
来源：http://sn.muxihuayi.cn

Perl ........... 10
来源：http://cx.bjjhwx.cn

Scala .......... 10
来源：http://zd.shtwfgs.cn

------------------------------------
来源：http://ke.szsharing.cn

合计 ........... 2106 条
来源：http://by.lnxyls.cn

按章节统计：
来源：http://kd.yuexingan06.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://xn.shtwfgs.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ck.yuexingan06.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wm.jianghongdianzi.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://yh.haigaiapp.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://qt.asd995.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://yb.bjjhwx.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://cg.colortex.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ob.gzmigu.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://la.panjiajie.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://zg.bookmarksfly.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://xg.shxzskj.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ym.yuexingan06.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://zg.521024.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://cm.nszjky.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://uv.gzmigu.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wu.jctech888.com.cn

Q SQL 专题                              90
来源：http://jy.haigaiapp.cn

R Bash 专题                             80
来源：http://tv.shxzukj.cn

S C / C++ 专题                          60
来源：http://dt.shxzskj.cn

T 其他语言补充                          60
来源：http://hd.jianghongdianzi.cn

U 高频实用片段                         120
来源：http://rd.panjiajie.cn

------------------------------------
来源：http://co.muxihuayi.cn

合计                                  2106 条
来源：http://lz.newstarts.cn

--------------------------------------------------------------------------------
来源：http://kp.asd995.cn

使用提醒
来源：http://er.asd995.cn

--------------------------------------------------------------------------------
来源：http://kf.lnxyls.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ss.gzmigu.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://np.9csxet.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://yo.nszjky.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://ro.yuntaijiaju.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ry.muxihuayi.cn

—— 文件结束 ——
来源：http://oj.asd995.cn

================================================================================
来源：http://wh.newstarts.cn

程序语言常见例子速查手册（2024 版）
来源：http://wh.haigaiapp.cn

Common Programming Examples Cheat Book
来源：http://ix.yuntaijiaju.cn

================================================================================
来源：http://wz.yuexingan06.cn

【收录内容】
来源：http://tt.jianghongdianzi.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://nk.nicolike.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hp.nicolike.cn

SQL · Bash · C · C++
来源：http://ic.jianghongdianzi.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://rv.bookmarksfly.cn

【使用说明】
来源：http://gp.haigaiapp.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hb.hahajie.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ye.jianghongdianzi.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://st.521024.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://yq.panjiajie.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://dq.nicolike.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wi.shxzskj.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://cr.colortex.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://pm.newstarts.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ck.wgjwhj.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ju.lnxyls.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://vy.yuexingan06.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://er.szxytkj.cn

【文件统计】
来源：http://pk.haigaiapp.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://be.szsharing.cn

--------------------------------------------------------------------------------
来源：http://eu.colortex.cn

目  录
来源：http://cd.gzmigu.cn

--------------------------------------------------------------------------------
来源：http://xp.jianghongdianzi.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://if.asd995.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://nd.yuexingan06.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://be.haigaiapp.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://tu.shtwfgs.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://qj.huixiangedu.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://el.521024.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://fy.hnjuh.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://zo.szsharing.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://qx.newstarts.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://xi.szsharing.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://aw.wgjwhj.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://ma.haigaiapp.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://gt.bookmarksfly.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://vv.9csxet.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://xu.521024.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hl.nszjky.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://pc.newstarts.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://kb.nicolike.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://fs.asd995.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://qi.yuntaijiaju.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hq.yuexingan06.cn

================================================================================
来源：http://rp.nicolike.cn

A. 基础语法与类型
来源：http://da.chemitech.net.cn

================================================================================
来源：http://ol.chemitech.net.cn

[A01] Hello World
来源：http://kb.bjjhwx.cn

Py:   print("Hello, World!")
来源：http://wq.bjjhwx.cn

PHP:  echo "Hello, World!";
来源：http://xp.nszjky.cn

JS:   console.log("Hello, World!");
来源：http://ei.huixinmuqiang.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://av.szsharing.cn

Java: System.out.println("Hello, World!");
来源：http://ds.521024.cn

Go:   fmt.Println("Hello, World!")
来源：http://lp.huanxung.cn

Ruby: puts "Hello, World!"
来源：http://wt.hnjuh.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://sn.szxytkj.cn

[A02] 变量声明与赋值
来源：http://oe.gzmigu.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ir.gzmigu.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://ex.yuexingan06.cn

JS:   let name = "Alex"; const age = 20;
来源：http://mg.bjjhwx.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://en.yuexingan06.cn

Java: String name = "Alex"; int age = 20;
来源：http://co.szsharing.cn

Go:   name := "Alex"; age := 20
来源：http://zf.huixiangedu.cn

Ruby: name = "Alex"; age = 20
来源：http://lb.huanxung.cn

C#:   string name = "Alex"; int age = 20;
来源：http://od.nicolike.cn

[A03] 常量定义
来源：http://qy.shxzskj.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://bl.huixiangedu.cn

PHP:  const PI = 3.14159;
来源：http://gj.huixiangedu.cn

JS:   const PI = 3.14159;
来源：http://hw.szsharing.cn

TS:   const PI: number = 3.14159;
来源：http://km.huixiangedu.cn

Java: static final double PI = 3.14159;
来源：http://he.shxzskj.cn

Go:   const PI = 3.14159
来源：http://dy.lnxyls.cn

Ruby: PI = 3.14159
来源：http://xm.bjjhwx.cn

C#:   const double PI = 3.14159;
来源：http://qe.bookmarksfly.cn

[A04] 判断变量类型
来源：http://qv.bjjhwx.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://rp.hnjuh.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://pi.nicolike.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://ad.bjjhwx.cn

TS:   typeof x; x instanceof Date
来源：http://mz.huixinmuqiang.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ny.huanxung.cn

Go:   reflect.TypeOf(x).Name()
来源：http://zv.huanxung.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://wq.muxihuayi.cn

C#:   x.GetType().Name; x is int
来源：http://jt.huixiangedu.cn

[A05] 整数除法与取模
来源：http://th.jctech888.com.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://wr.bjjhwx.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://ph.huanxung.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hn.bookmarksfly.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://yt.huixiangedu.cn

Java: 7 / 2; 7 % 2
来源：http://nz.521024.cn

Go:   7 / 2; 7 % 2
来源：http://xe.shxzskj.cn

Ruby: 7 / 2; 7 % 2
来源：http://du.jctech888.com.cn

C#:   7 / 2; 7 % 2
来源：http://ps.szsharing.cn


<!-- 参考信息 -->