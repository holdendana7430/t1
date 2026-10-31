代发 wailian999

[U31] Py：单测
来源：http://bb.shxzskj.cn

python -m pytest -q
来源：http://tg.chemitech.net.cn

[U32] Py：代码格式化
来源：http://bj.jianghongdianzi.cn

ruff format . && ruff check --fix .
来源：http://es.szsharing.cn

[U33] Py：打包发布
来源：http://yy.shxzukj.cn

python -m build  （依赖 pyproject.toml）
来源：http://lm.huixinmuqiang.cn

[U34] Py：判断编码
来源：http://pn.nicolike.cn

chardet.detect(raw)
来源：http://yd.bookmarksfly.cn

[U35] Py：发送邮件
来源：http://gy.bookmarksfly.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://dz.521024.cn

[U36] Py：定时任务
来源：http://rg.newstarts.cn

schedule.every(10).minutes.do(job)
来源：http://ok.yuexingan06.cn

[U37] Py：读写 Excel
来源：http://te.bjjhwx.cn

pandas.read_excel / DataFrame.to_excel
来源：http://uh.huixiangedu.cn

[U38] Py：获取脚本所在目录
来源：http://yg.muxihuayi.cn

Path(__file__).resolve().parent
来源：http://hf.nszjky.cn

[U39] Py：判断是否在交互环境
来源：http://nh.shxzskj.cn

sys.stdout.isatty()
来源：http://xs.jctech888.com.cn

[U40] Py：打印到标准错误
来源：http://jy.bookmarksfly.cn

print("err", file=sys.stderr)
来源：http://ry.huanxung.cn

[U41] PHP：初始化 Composer 项目
来源：http://jz.chemitech.net.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://zn.szsharing.cn

[U42] PHP：PSR-4 自动加载
来源：http://vy.shtwfgs.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://jm.colortex.cn

[U43] PHP：声明命名空间
来源：http://ek.jianghongdianzi.cn

namespace App\Http;
来源：http://bm.chemitech.net.cn

[U44] PHP：开启严格类型
来源：http://zo.haigaiapp.cn

declare(strict_types=1);
来源：http://th.haigaiapp.cn

[U45] PHP：类型声明与返回类型
来源：http://eh.9csxet.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://od.szsharing.cn

[U46] PHP：可空类型
来源：http://qq.colortex.cn

?string $name = null
来源：http://lb.hahajie.cn

[U47] PHP：联合类型
来源：http://tw.huixinmuqiang.cn

int|string $id
来源：http://jp.chemitech.net.cn

[U48] PHP：纯枚举
来源：http://wx.asd995.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://gg.asd995.cn

[U49] PHP：只读属性
来源：http://cs.huixinmuqiang.cn

public readonly string $name
来源：http://ls.huanxung.cn

[U50] PHP：构造器属性提升
来源：http://vp.lnxyls.cn

public function __construct(private int $id) {}
来源：http://wx.shxzskj.cn

[U51] PHP：数组解构
来源：http://kf.wgjwhj.cn

[$a, $b] = $arr;
来源：http://ny.huixiangedu.cn

[U52] PHP：箭头函数
来源：http://sy.szsharing.cn

$double = fn($x) => $x * 2;
来源：http://ge.lnxyls.cn

[U53] PHP：空合并运算符
来源：http://qs.521024.cn

$v = $a ?? $b ?? "default";
来源：http://zr.nicolike.cn

[U54] PHP：空安全调用
来源：http://wt.hahajie.cn

$obj?->method()
来源：http://py.jianghongdianzi.cn

[U55] PHP：match 表达式
来源：http://ah.shxzukj.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://se.chemitech.net.cn

[U56] PHP：命名参数
来源：http://mg.wgjwhj.cn

f(a: 1, b: 2)
来源：http://js.hahajie.cn

[U57] PHP：字符串插值
来源：http://wh.lnxyls.cn

"值: {$a}"
来源：http://mw.huanxung.cn

[U58] PHP：数组三件套
来源：http://gg.yuexingan06.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ra.panjiajie.cn

[U59] PHP：自定义排序
来源：http://dn.colortex.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ws.chemitech.net.cn

[U60] PHP：JSON 编解码
来源：http://en.hahajie.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://dj.gzmigu.cn

[U61] PHP：正则
来源：http://bi.nicolike.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://rh.yuexingan06.cn

[U62] PHP：日期对象
来源：http://mb.gzmigu.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://lb.shxzskj.cn

[U63] PHP：文件读写
来源：http://ga.bjjhwx.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://tz.muxihuayi.cn

[U64] PHP：目录遍历
来源：http://qm.wgjwhj.cn

glob("dir/*.php");  scandir("dir");
来源：http://vj.lnxyls.cn

[U65] PHP：会话
来源：http://hs.521024.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://et.shxzukj.cn

[U66] PHP：设置 Cookie
来源：http://oc.yuexingan06.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://nk.lnxyls.cn

[U67] PHP：处理文件上传
来源：http://nt.huanxung.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://dl.huanxung.cn

[U68] PHP：PDO 连接
来源：http://bq.newstarts.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ip.colortex.cn

[U69] PHP：PDO 预处理
来源：http://st.yuexingan06.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://uy.szsharing.cn

[U70] PHP：PDO 事务
来源：http://fo.jianghongdianzi.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://gf.haigaiapp.cn

[U71] PHP：抛出异常
来源：http://zs.szxytkj.cn

throw new RuntimeException("失败", 500);
来源：http://yo.9csxet.cn

[U72] PHP：写错误日志
来源：http://ee.gzmigu.cn

error_log("失败: " . $e->getMessage());
来源：http://ff.szxytkj.cn

[U73] PHP：读取 ini 配置
来源：http://qd.9csxet.cn

parse_ini_file("config.ini", true)
来源：http://vt.jctech888.com.cn

[U74] PHP：读取环境变量
来源：http://vq.yuntaijiaju.cn

getenv("APP_ENV") ?: "production"
来源：http://ps.hnjuh.cn

[U75] PHP：依赖注入
来源：http://sc.nszjky.cn

composer require psr/container
来源：http://qe.szxytkj.cn

[U76] PHP：简单路由
来源：http://yu.yuexingan06.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://lv.jctech888.com.cn

[U77] PHP：模板渲染
来源：http://di.shxzukj.cn

composer require twig/twig
来源：http://fv.shxzskj.cn

[U78] PHP：单元测试
来源：http://ca.yuexingan06.cn

composer require --dev phpunit/phpunit
来源：http://na.hahajie.cn

[U79] PHP：静态分析
来源：http://ze.hahajie.cn

composer require --dev phpstan/phpstan
来源：http://xa.huanxung.cn

[U80] PHP：代码规范修复
来源：http://sg.bookmarksfly.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://pw.szxytkj.cn

[U81] JS：初始化项目
来源：http://hf.szxytkj.cn

npm init -y;  npm i express
来源：http://vd.gzmigu.cn

[U82] JS：package.json 脚本
来源：http://ho.hnjuh.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://vo.newstarts.cn

[U83] JS：ES Module 导入导出
来源：http://lc.chemitech.net.cn

export const a = 1;  import { a } from "./m.js";
来源：http://qo.szxytkj.cn

[U84] JS：CommonJS 写法
来源：http://hb.huixinmuqiang.cn

module.exports = { a };  const { a } = require("./m");
来源：http://ll.szsharing.cn

[U85] JS：可选链
来源：http://vx.hnjuh.cn

a?.b?.c
来源：http://ll.huanxung.cn

[U86] JS：空值合并
来源：http://gf.9csxet.cn

a ?? b
来源：http://xg.gzmigu.cn

[U87] JS：解构默认值
来源：http://ey.huixiangedu.cn

const { a = 1, b = 2 } = obj;
来源：http://cb.bjjhwx.cn

[U88] JS：对象展开合并
来源：http://yu.szsharing.cn

{ ...a, ...b }
来源：http://xo.szxytkj.cn

[U89] JS：数组去重
来源：http://yh.521024.cn

[...new Set(arr)]
来源：http://zk.shxzskj.cn

[U90] JS：数字数组排序
来源：http://pd.szsharing.cn

[...arr].sort((a, b) => a - b)
来源：http://xc.newstarts.cn

[U91] JS：对象键值遍历
来源：http://mg.bjjhwx.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://qh.szxytkj.cn

[U92] JS：深拷贝
来源：http://kx.szsharing.cn

structuredClone(obj)
来源：http://xm.9csxet.cn

[U93] JS：模板字符串
来源：http://pz.shtwfgs.cn

`共 ${n} 条`
来源：http://zr.huixinmuqiang.cn

[U94] JS：箭头函数
来源：http://am.nicolike.cn

const double = x => x * 2;
来源：http://fm.shxzskj.cn

[U95] JS：Promise 包装
来源：http://xz.shxzskj.cn

new Promise((resolve, reject) => {})
来源：http://ah.gzmigu.cn

[U96] JS：async/await 与异常
来源：http://jr.haigaiapp.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://jz.shxzskj.cn

[U97] JS：并发请求
来源：http://rh.shtwfgs.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://gx.huanxung.cn

[U98] JS：fetch 带 JSON
来源：http://pd.haigaiapp.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://eb.bjjhwx.cn

[U99] JS：事件监听
来源：http://ln.lnxyls.cn

el.addEventListener("click", e => {})
来源：http://ec.shxzskj.cn

[U100] JS：DOM 查询
来源：http://vs.hnjuh.cn

document.querySelector(".item")
来源：http://wg.shtwfgs.cn

[U101] JS：classList 操作
来源：http://vb.asd995.cn

el.classList.toggle("active")
来源：http://rj.yuntaijiaju.cn

[U102] JS：本地存储
来源：http://sk.yuexingan06.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://za.shtwfgs.cn

[U103] JS：定时器
来源：http://un.szxytkj.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://qy.bjjhwx.cn

[U104] JS：防抖
来源：http://zd.colortex.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ob.chemitech.net.cn

[U105] JS：节流
来源：http://om.hnjuh.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://bq.shtwfgs.cn

[U106] JS：日期格式化
来源：http://ea.haigaiapp.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://jc.jianghongdianzi.cn

[U107] JS：数字千分位
来源：http://pa.bjjhwx.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ho.asd995.cn

[U108] JS：随机整数
来源：http://ot.lnxyls.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://rf.9csxet.cn

[U109] JS：数组分组
来源：http://lv.newstarts.cn

Object.groupBy(arr, x => x.type)
来源：http://pp.nszjky.cn

[U110] JS：数组分块
来源：http://gi.521024.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://fp.yuexingan06.cn

[U111] JS：对象转 Map
来源：http://vs.haigaiapp.cn

new Map(Object.entries(obj))
来源：http://rn.hahajie.cn

[U112] JS：字符串补位
来源：http://sb.haigaiapp.cn

"7".padStart(3, "0")
来源：http://yk.yuntaijiaju.cn

[U113] JS：正则替换全部
来源：http://oe.yuexingan06.cn

s.replaceAll("a", "b")
来源：http://aa.wgjwhj.cn

[U114] JS：JSON 深比较
来源：http://pa.bjjhwx.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://kx.newstarts.cn

[U115] JS：生成 UUID
来源：http://ac.yuexingan06.cn

crypto.randomUUID()
来源：http://wn.panjiajie.cn

[U116] JS：类型检查（JSDoc）
来源：http://wj.haigaiapp.cn

/** @param {string} name */ function f(name) {}
来源：http://bi.panjiajie.cn

[U117] JS：单元测试
来源：http://os.haigaiapp.cn

npm i -D vitest;  npx vitest
来源：http://gt.haigaiapp.cn

[U118] JS：开发服务器
来源：http://sd.bookmarksfly.cn

npm i -D vite;  npx vite
来源：http://tl.szsharing.cn

[U119] JS：生产构建
来源：http://rq.huanxung.cn

npx vite build
来源：http://bv.newstarts.cn

[U120] JS：读取环境变量（Vite）
来源：http://rl.gzmigu.cn

import.meta.env.VITE_API_URL
来源：http://in.colortex.cn

================================================================================
来源：http://pa.nicolike.cn

统计汇总
来源：http://sh.lnxyls.cn

================================================================================
来源：http://pe.521024.cn

按语言统计（条）：
来源：http://zd.panjiajie.cn

Python ......... 252
来源：http://uf.9csxet.cn

PHP ............ 252
来源：http://ad.bjjhwx.cn

JavaScript ..... 252
来源：http://vu.newstarts.cn

TypeScript ..... 212
来源：http://nv.chemitech.net.cn

Java ........... 212
来源：http://fj.szsharing.cn

Go ............. 212
来源：http://ou.bookmarksfly.cn

Ruby ........... 212
来源：http://qv.szsharing.cn

C# ............. 212
来源：http://wp.shxzukj.cn

C .............. 30
来源：http://vj.jctech888.com.cn

C++ ............ 30
来源：http://we.shxzukj.cn

SQL ............ 90
来源：http://pr.yuntaijiaju.cn

Bash ........... 80
来源：http://kn.521024.cn

Kotlin ......... 15
来源：http://kp.hahajie.cn

Swift .......... 15
来源：http://sx.gzmigu.cn

Lua ............ 10
来源：http://um.bjjhwx.cn

Perl ........... 10
来源：http://zx.shxzskj.cn

Scala .......... 10
来源：http://ji.jianghongdianzi.cn

------------------------------------
来源：http://zv.colortex.cn

合计 ........... 2106 条
来源：http://or.yuexingan06.cn

按章节统计：
来源：http://pv.colortex.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://bg.huixinmuqiang.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wc.panjiajie.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://is.bjjhwx.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ey.wgjwhj.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wh.huixiangedu.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://dr.shxzukj.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://xo.wgjwhj.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://lu.shxzskj.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://eb.nszjky.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://kp.shxzskj.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://jv.asd995.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://kl.shxzukj.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://rv.colortex.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://sj.szsharing.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://nz.hnjuh.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://eh.haigaiapp.cn

Q SQL 专题                              90
来源：http://mm.panjiajie.cn

R Bash 专题                             80
来源：http://qh.shxzukj.cn

S C / C++ 专题                          60
来源：http://dc.shtwfgs.cn

T 其他语言补充                          60
来源：http://au.bookmarksfly.cn

U 高频实用片段                         120
来源：http://ms.shxzukj.cn

------------------------------------
来源：http://ye.chemitech.net.cn

合计                                  2106 条
来源：http://jj.szsharing.cn

--------------------------------------------------------------------------------
来源：http://do.wgjwhj.cn

使用提醒
来源：http://om.shxzukj.cn

--------------------------------------------------------------------------------
来源：http://rc.bjjhwx.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ov.asd995.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ld.gzmigu.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://bp.9csxet.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://kr.hahajie.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://gg.haigaiapp.cn

—— 文件结束 ——
来源：http://bb.nszjky.cn

================================================================================
来源：http://rb.szxytkj.cn

程序语言常见例子速查手册（2024 版）
来源：http://yn.panjiajie.cn

Common Programming Examples Cheat Book
来源：http://dg.yuntaijiaju.cn

================================================================================
来源：http://un.hnjuh.cn

【收录内容】
来源：http://fd.newstarts.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://xm.jctech888.com.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://rq.jianghongdianzi.cn

SQL · Bash · C · C++
来源：http://fm.hnjuh.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wl.gzmigu.cn

【使用说明】
来源：http://vx.panjiajie.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://oy.yuntaijiaju.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://pu.nszjky.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://nf.wgjwhj.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ng.huixiangedu.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://hq.shtwfgs.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://mw.hahajie.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://dm.9csxet.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://bt.panjiajie.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ek.bookmarksfly.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://jk.huixiangedu.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://li.nszjky.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://jl.lnxyls.cn

【文件统计】
来源：http://eg.huixiangedu.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://as.asd995.cn

--------------------------------------------------------------------------------
来源：http://is.colortex.cn

目  录
来源：http://yo.hahajie.cn

--------------------------------------------------------------------------------
来源：http://jw.shxzskj.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://us.hnjuh.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://eo.asd995.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://ph.hnjuh.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://yd.shxzskj.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://cg.521024.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://kx.panjiajie.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://nb.hahajie.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://md.chemitech.net.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://rj.shxzukj.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://vv.panjiajie.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://go.shxzukj.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hd.hnjuh.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://yz.colortex.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://gr.hnjuh.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://wi.szxytkj.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://nu.jianghongdianzi.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://tz.colortex.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://up.jctech888.com.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://gl.bjjhwx.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://rd.newstarts.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://ky.jctech888.com.cn

================================================================================
来源：http://it.huixiangedu.cn

A. 基础语法与类型
来源：http://ay.bookmarksfly.cn

================================================================================
来源：http://jp.shtwfgs.cn

[A01] Hello World
来源：http://tn.haigaiapp.cn

Py:   print("Hello, World!")
来源：http://jw.yuexingan06.cn

PHP:  echo "Hello, World!";
来源：http://dc.hnjuh.cn

JS:   console.log("Hello, World!");
来源：http://nq.huixiangedu.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://vd.asd995.cn

Java: System.out.println("Hello, World!");
来源：http://mm.huixiangedu.cn

Go:   fmt.Println("Hello, World!")
来源：http://rd.yuexingan06.cn

Ruby: puts "Hello, World!"
来源：http://gp.521024.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://jr.nszjky.cn

[A02] 变量声明与赋值
来源：http://kk.gzmigu.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://lz.yuntaijiaju.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://hp.hnjuh.cn

JS:   let name = "Alex"; const age = 20;
来源：http://he.521024.cn


<!-- 参考信息 -->