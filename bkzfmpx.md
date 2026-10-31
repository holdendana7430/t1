代发 wailian999

[U35] Py：发送邮件
来源：http://ug.muxihuayi.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://bs.521024.cn

[U36] Py：定时任务
来源：http://bs.haigaiapp.cn

schedule.every(10).minutes.do(job)
来源：http://pj.bjjhwx.cn

[U37] Py：读写 Excel
来源：http://cf.wgjwhj.cn

pandas.read_excel / DataFrame.to_excel
来源：http://lo.nicolike.cn

[U38] Py：获取脚本所在目录
来源：http://ez.yuexingan06.cn

Path(__file__).resolve().parent
来源：http://ey.panjiajie.cn

[U39] Py：判断是否在交互环境
来源：http://la.yuntaijiaju.cn

sys.stdout.isatty()
来源：http://ak.asd995.cn

[U40] Py：打印到标准错误
来源：http://gy.huanxung.cn

print("err", file=sys.stderr)
来源：http://qi.huanxung.cn

[U41] PHP：初始化 Composer 项目
来源：http://ml.haigaiapp.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://qw.9csxet.cn

[U42] PHP：PSR-4 自动加载
来源：http://fm.huixiangedu.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://sc.521024.cn

[U43] PHP：声明命名空间
来源：http://bi.gzmigu.cn

namespace App\Http;
来源：http://dq.hahajie.cn

[U44] PHP：开启严格类型
来源：http://my.haigaiapp.cn

declare(strict_types=1);
来源：http://fj.huixiangedu.cn

[U45] PHP：类型声明与返回类型
来源：http://sg.lnxyls.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://qu.newstarts.cn

[U46] PHP：可空类型
来源：http://kk.colortex.cn

?string $name = null
来源：http://ux.gzmigu.cn

[U47] PHP：联合类型
来源：http://mq.shxzukj.cn

int|string $id
来源：http://xy.hnjuh.cn

[U48] PHP：纯枚举
来源：http://vi.asd995.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://tv.shxzskj.cn

[U49] PHP：只读属性
来源：http://se.nicolike.cn

public readonly string $name
来源：http://ru.nszjky.cn

[U50] PHP：构造器属性提升
来源：http://id.muxihuayi.cn

public function __construct(private int $id) {}
来源：http://dz.newstarts.cn

[U51] PHP：数组解构
来源：http://oh.jianghongdianzi.cn

[$a, $b] = $arr;
来源：http://sy.nszjky.cn

[U52] PHP：箭头函数
来源：http://al.hnjuh.cn

$double = fn($x) => $x * 2;
来源：http://kf.newstarts.cn

[U53] PHP：空合并运算符
来源：http://di.shxzukj.cn

$v = $a ?? $b ?? "default";
来源：http://wz.huixiangedu.cn

[U54] PHP：空安全调用
来源：http://wx.haigaiapp.cn

$obj?->method()
来源：http://gw.9csxet.cn

[U55] PHP：match 表达式
来源：http://la.haigaiapp.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://co.gzmigu.cn

[U56] PHP：命名参数
来源：http://lq.huixiangedu.cn

f(a: 1, b: 2)
来源：http://ct.asd995.cn

[U57] PHP：字符串插值
来源：http://ew.asd995.cn

"值: {$a}"
来源：http://yn.bjjhwx.cn

[U58] PHP：数组三件套
来源：http://sf.haigaiapp.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://zh.9csxet.cn

[U59] PHP：自定义排序
来源：http://qp.panjiajie.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://nj.nszjky.cn

[U60] PHP：JSON 编解码
来源：http://kb.panjiajie.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://fq.huanxung.cn

[U61] PHP：正则
来源：http://iw.chemitech.net.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://iz.9csxet.cn

[U62] PHP：日期对象
来源：http://jc.hahajie.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://qc.jctech888.com.cn

[U63] PHP：文件读写
来源：http://so.huixinmuqiang.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ua.bookmarksfly.cn

[U64] PHP：目录遍历
来源：http://vr.521024.cn

glob("dir/*.php");  scandir("dir");
来源：http://nz.shxzukj.cn

[U65] PHP：会话
来源：http://yx.nicolike.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://rf.chemitech.net.cn

[U66] PHP：设置 Cookie
来源：http://ta.bookmarksfly.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ju.asd995.cn

[U67] PHP：处理文件上传
来源：http://ry.wgjwhj.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://la.shxzskj.cn

[U68] PHP：PDO 连接
来源：http://ct.yuntaijiaju.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ij.wgjwhj.cn

[U69] PHP：PDO 预处理
来源：http://rr.521024.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hx.colortex.cn

[U70] PHP：PDO 事务
来源：http://ze.nicolike.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://zr.nszjky.cn

[U71] PHP：抛出异常
来源：http://yx.asd995.cn

throw new RuntimeException("失败", 500);
来源：http://nz.jctech888.com.cn

[U72] PHP：写错误日志
来源：http://uy.shxzskj.cn

error_log("失败: " . $e->getMessage());
来源：http://ls.nicolike.cn

[U73] PHP：读取 ini 配置
来源：http://tu.521024.cn

parse_ini_file("config.ini", true)
来源：http://ac.newstarts.cn

[U74] PHP：读取环境变量
来源：http://nu.chemitech.net.cn

getenv("APP_ENV") ?: "production"
来源：http://yi.hnjuh.cn

[U75] PHP：依赖注入
来源：http://np.chemitech.net.cn

composer require psr/container
来源：http://we.bjjhwx.cn

[U76] PHP：简单路由
来源：http://fl.hnjuh.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://gl.huanxung.cn

[U77] PHP：模板渲染
来源：http://iq.colortex.cn

composer require twig/twig
来源：http://ea.shxzukj.cn

[U78] PHP：单元测试
来源：http://fv.huanxung.cn

composer require --dev phpunit/phpunit
来源：http://lo.muxihuayi.cn

[U79] PHP：静态分析
来源：http://xo.muxihuayi.cn

composer require --dev phpstan/phpstan
来源：http://qu.521024.cn

[U80] PHP：代码规范修复
来源：http://rn.huixinmuqiang.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://vm.chemitech.net.cn

[U81] JS：初始化项目
来源：http://nc.gzmigu.cn

npm init -y;  npm i express
来源：http://wj.muxihuayi.cn

[U82] JS：package.json 脚本
来源：http://xx.hnjuh.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://xx.nszjky.cn

[U83] JS：ES Module 导入导出
来源：http://nk.bjjhwx.cn

export const a = 1;  import { a } from "./m.js";
来源：http://jc.asd995.cn

[U84] JS：CommonJS 写法
来源：http://jk.hahajie.cn

module.exports = { a };  const { a } = require("./m");
来源：http://sj.szsharing.cn

[U85] JS：可选链
来源：http://qd.jianghongdianzi.cn

a?.b?.c
来源：http://cc.bookmarksfly.cn

[U86] JS：空值合并
来源：http://qj.gzmigu.cn

a ?? b
来源：http://et.shtwfgs.cn

[U87] JS：解构默认值
来源：http://fk.jctech888.com.cn

const { a = 1, b = 2 } = obj;
来源：http://xh.newstarts.cn

[U88] JS：对象展开合并
来源：http://gk.lnxyls.cn

{ ...a, ...b }
来源：http://zw.hnjuh.cn

[U89] JS：数组去重
来源：http://zs.wgjwhj.cn

[...new Set(arr)]
来源：http://zr.hahajie.cn

[U90] JS：数字数组排序
来源：http://zs.bookmarksfly.cn

[...arr].sort((a, b) => a - b)
来源：http://yq.hnjuh.cn

[U91] JS：对象键值遍历
来源：http://cz.huixinmuqiang.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://lf.gzmigu.cn

[U92] JS：深拷贝
来源：http://ww.jianghongdianzi.cn

structuredClone(obj)
来源：http://oy.shxzukj.cn

[U93] JS：模板字符串
来源：http://ey.wgjwhj.cn

`共 ${n} 条`
来源：http://bt.gzmigu.cn

[U94] JS：箭头函数
来源：http://oi.huixinmuqiang.cn

const double = x => x * 2;
来源：http://ru.gzmigu.cn

[U95] JS：Promise 包装
来源：http://po.colortex.cn

new Promise((resolve, reject) => {})
来源：http://ik.szxytkj.cn

[U96] JS：async/await 与异常
来源：http://ya.chemitech.net.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ze.huixiangedu.cn

[U97] JS：并发请求
来源：http://ix.lnxyls.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://fa.muxihuayi.cn

[U98] JS：fetch 带 JSON
来源：http://kn.yuntaijiaju.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://od.yuntaijiaju.cn

[U99] JS：事件监听
来源：http://ms.jctech888.com.cn

el.addEventListener("click", e => {})
来源：http://ol.bjjhwx.cn

[U100] JS：DOM 查询
来源：http://kw.bjjhwx.cn

document.querySelector(".item")
来源：http://ii.shxzskj.cn

[U101] JS：classList 操作
来源：http://xs.jctech888.com.cn

el.classList.toggle("active")
来源：http://el.gzmigu.cn

[U102] JS：本地存储
来源：http://xo.9csxet.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://rz.bjjhwx.cn

[U103] JS：定时器
来源：http://tv.muxihuayi.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://xa.colortex.cn

[U104] JS：防抖
来源：http://tx.9csxet.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pq.shxzukj.cn

[U105] JS：节流
来源：http://qu.hahajie.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://nz.shtwfgs.cn

[U106] JS：日期格式化
来源：http://xu.haigaiapp.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://lc.haigaiapp.cn

[U107] JS：数字千分位
来源：http://pc.huanxung.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://xe.nszjky.cn

[U108] JS：随机整数
来源：http://gc.yuexingan06.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mt.jianghongdianzi.cn

[U109] JS：数组分组
来源：http://fk.bookmarksfly.cn

Object.groupBy(arr, x => x.type)
来源：http://sn.jctech888.com.cn

[U110] JS：数组分块
来源：http://wt.chemitech.net.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ya.huixiangedu.cn

[U111] JS：对象转 Map
来源：http://hv.521024.cn

new Map(Object.entries(obj))
来源：http://tk.bookmarksfly.cn

[U112] JS：字符串补位
来源：http://oz.szsharing.cn

"7".padStart(3, "0")
来源：http://uf.shtwfgs.cn

[U113] JS：正则替换全部
来源：http://qo.hahajie.cn

s.replaceAll("a", "b")
来源：http://ty.szsharing.cn

[U114] JS：JSON 深比较
来源：http://co.szxytkj.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://vo.bjjhwx.cn

[U115] JS：生成 UUID
来源：http://jb.shxzukj.cn

crypto.randomUUID()
来源：http://zl.521024.cn

[U116] JS：类型检查（JSDoc）
来源：http://xl.hahajie.cn

/** @param {string} name */ function f(name) {}
来源：http://aq.gzmigu.cn

[U117] JS：单元测试
来源：http://xn.asd995.cn

npm i -D vitest;  npx vitest
来源：http://gz.szsharing.cn

[U118] JS：开发服务器
来源：http://eb.colortex.cn

npm i -D vite;  npx vite
来源：http://kb.jctech888.com.cn

[U119] JS：生产构建
来源：http://ss.muxihuayi.cn

npx vite build
来源：http://zj.yuexingan06.cn

[U120] JS：读取环境变量（Vite）
来源：http://ap.shxzukj.cn

import.meta.env.VITE_API_URL
来源：http://oz.521024.cn

================================================================================
来源：http://ke.shtwfgs.cn

统计汇总
来源：http://cm.szsharing.cn

================================================================================
来源：http://rn.bookmarksfly.cn

按语言统计（条）：
来源：http://zg.panjiajie.cn

Python ......... 252
来源：http://js.nicolike.cn

PHP ............ 252
来源：http://mj.hahajie.cn

JavaScript ..... 252
来源：http://jk.yuntaijiaju.cn

TypeScript ..... 212
来源：http://ew.gzmigu.cn

Java ........... 212
来源：http://jg.chemitech.net.cn

Go ............. 212
来源：http://ii.shxzskj.cn

Ruby ........... 212
来源：http://cf.haigaiapp.cn

C# ............. 212
来源：http://bl.shtwfgs.cn

C .............. 30
来源：http://hb.bookmarksfly.cn

C++ ............ 30
来源：http://fo.bjjhwx.cn

SQL ............ 90
来源：http://sg.bookmarksfly.cn

Bash ........... 80
来源：http://yq.gzmigu.cn

Kotlin ......... 15
来源：http://eg.szxytkj.cn

Swift .......... 15
来源：http://ca.9csxet.cn

Lua ............ 10
来源：http://vo.hahajie.cn

Perl ........... 10
来源：http://va.haigaiapp.cn

Scala .......... 10
来源：http://gc.yuexingan06.cn

------------------------------------
来源：http://eh.shxzskj.cn

合计 ........... 2106 条
来源：http://dv.newstarts.cn

按章节统计：
来源：http://es.haigaiapp.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://xg.asd995.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ns.newstarts.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ms.huixinmuqiang.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://lg.jianghongdianzi.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://gg.jianghongdianzi.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ts.haigaiapp.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://cg.9csxet.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://cr.hnjuh.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://tb.chemitech.net.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://yp.huixinmuqiang.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://tt.chemitech.net.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://gu.wgjwhj.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://vv.muxihuayi.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://il.nicolike.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ly.chemitech.net.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ej.colortex.cn

Q SQL 专题                              90
来源：http://zg.panjiajie.cn

R Bash 专题                             80
来源：http://xv.jianghongdianzi.cn

S C / C++ 专题                          60
来源：http://jz.bookmarksfly.cn

T 其他语言补充                          60
来源：http://ej.hnjuh.cn

U 高频实用片段                         120
来源：http://tp.521024.cn

------------------------------------
来源：http://jk.yuexingan06.cn

合计                                  2106 条
来源：http://ud.hnjuh.cn

--------------------------------------------------------------------------------
来源：http://ra.bookmarksfly.cn

使用提醒
来源：http://il.shxzukj.cn

--------------------------------------------------------------------------------
来源：http://sd.panjiajie.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://mf.jianghongdianzi.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ql.asd995.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ti.huixiangedu.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://st.521024.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://pj.muxihuayi.cn

—— 文件结束 ——
来源：http://ys.jctech888.com.cn

================================================================================
来源：http://un.shxzskj.cn

程序语言常见例子速查手册（2024 版）
来源：http://iv.521024.cn

Common Programming Examples Cheat Book
来源：http://xt.nicolike.cn

================================================================================
来源：http://ex.hahajie.cn

【收录内容】
来源：http://iu.9csxet.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://fb.shtwfgs.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://lr.shxzskj.cn

SQL · Bash · C · C++
来源：http://pk.chemitech.net.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://be.yuexingan06.cn

【使用说明】
来源：http://qc.huanxung.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://kh.yuntaijiaju.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://em.gzmigu.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://oh.huanxung.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ar.jianghongdianzi.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://dz.colortex.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://qq.hnjuh.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://vn.huixinmuqiang.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://fw.haigaiapp.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ae.521024.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://gf.shxzskj.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://dl.muxihuayi.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://pp.szxytkj.cn

【文件统计】
来源：http://ck.chemitech.net.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ec.jctech888.com.cn

--------------------------------------------------------------------------------
来源：http://ci.nszjky.cn

目  录
来源：http://cm.colortex.cn

--------------------------------------------------------------------------------
来源：http://fw.colortex.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ko.lnxyls.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://qo.muxihuayi.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://jc.szxytkj.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://xs.szsharing.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://uc.9csxet.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://du.bjjhwx.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://yt.huanxung.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ej.shxzukj.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://kj.jctech888.com.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://jh.hahajie.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ix.hahajie.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://ag.hnjuh.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://ud.lnxyls.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://tq.asd995.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://tt.lnxyls.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://lq.huanxung.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://mo.wgjwhj.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://lw.yuexingan06.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://aq.huixinmuqiang.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://gv.szxytkj.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://te.huanxung.cn

================================================================================
来源：http://vg.hahajie.cn

A. 基础语法与类型
来源：http://qf.chemitech.net.cn

================================================================================
来源：http://le.yuntaijiaju.cn

[A01] Hello World
来源：http://qp.nszjky.cn

Py:   print("Hello, World!")
来源：http://ax.asd995.cn

PHP:  echo "Hello, World!";
来源：http://se.nicolike.cn

JS:   console.log("Hello, World!");
来源：http://fr.huixinmuqiang.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://nb.nszjky.cn

Java: System.out.println("Hello, World!");
来源：http://fb.chemitech.net.cn

Go:   fmt.Println("Hello, World!")
来源：http://ou.szxytkj.cn

Ruby: puts "Hello, World!"
来源：http://je.yuexingan06.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://wv.bjjhwx.cn

[A02] 变量声明与赋值
来源：http://nx.gzmigu.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ea.haigaiapp.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://qw.hahajie.cn

JS:   let name = "Alex"; const age = 20;
来源：http://xc.nicolike.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://wr.huanxung.cn

Java: String name = "Alex"; int age = 20;
来源：http://go.521024.cn

Go:   name := "Alex"; age := 20
来源：http://tu.huixiangedu.cn

Ruby: name = "Alex"; age = 20
来源：http://bv.521024.cn

C#:   string name = "Alex"; int age = 20;
来源：http://lt.jianghongdianzi.cn

[A03] 常量定义
来源：http://du.shtwfgs.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://oy.9csxet.cn

PHP:  const PI = 3.14159;
来源：http://qf.jianghongdianzi.cn


<!-- 参考信息 -->