代发 wailian999

[U33] Py：打包发布
来源：http://yy.asd995.cn

python -m build  （依赖 pyproject.toml）
来源：http://uf.gzmigu.cn

[U34] Py：判断编码
来源：http://jx.yuexingan06.cn

chardet.detect(raw)
来源：http://mr.nszjky.cn

[U35] Py：发送邮件
来源：http://vt.wgjwhj.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://tb.szsharing.cn

[U36] Py：定时任务
来源：http://pu.shxzskj.cn

schedule.every(10).minutes.do(job)
来源：http://ht.521024.cn

[U37] Py：读写 Excel
来源：http://lz.shtwfgs.cn

pandas.read_excel / DataFrame.to_excel
来源：http://rq.huixiangedu.cn

[U38] Py：获取脚本所在目录
来源：http://rc.huixinmuqiang.cn

Path(__file__).resolve().parent
来源：http://pp.hahajie.cn

[U39] Py：判断是否在交互环境
来源：http://gv.shtwfgs.cn

sys.stdout.isatty()
来源：http://mh.yuexingan06.cn

[U40] Py：打印到标准错误
来源：http://cx.bjjhwx.cn

print("err", file=sys.stderr)
来源：http://wn.asd995.cn

[U41] PHP：初始化 Composer 项目
来源：http://il.521024.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://uf.hnjuh.cn

[U42] PHP：PSR-4 自动加载
来源：http://ry.shxzskj.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hq.huanxung.cn

[U43] PHP：声明命名空间
来源：http://do.huixinmuqiang.cn

namespace App\Http;
来源：http://es.jianghongdianzi.cn

[U44] PHP：开启严格类型
来源：http://xs.nicolike.cn

declare(strict_types=1);
来源：http://tv.szsharing.cn

[U45] PHP：类型声明与返回类型
来源：http://ad.9csxet.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://bq.szxytkj.cn

[U46] PHP：可空类型
来源：http://hc.newstarts.cn

?string $name = null
来源：http://di.9csxet.cn

[U47] PHP：联合类型
来源：http://lq.bjjhwx.cn

int|string $id
来源：http://am.chemitech.net.cn

[U48] PHP：纯枚举
来源：http://wx.nicolike.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ia.shxzskj.cn

[U49] PHP：只读属性
来源：http://mi.nszjky.cn

public readonly string $name
来源：http://uo.huixinmuqiang.cn

[U50] PHP：构造器属性提升
来源：http://vi.bjjhwx.cn

public function __construct(private int $id) {}
来源：http://rd.yuntaijiaju.cn

[U51] PHP：数组解构
来源：http://om.jctech888.com.cn

[$a, $b] = $arr;
来源：http://tp.szsharing.cn

[U52] PHP：箭头函数
来源：http://nb.shtwfgs.cn

$double = fn($x) => $x * 2;
来源：http://zb.asd995.cn

[U53] PHP：空合并运算符
来源：http://og.szxytkj.cn

$v = $a ?? $b ?? "default";
来源：http://ze.wgjwhj.cn

[U54] PHP：空安全调用
来源：http://za.shxzukj.cn

$obj?->method()
来源：http://ld.shxzukj.cn

[U55] PHP：match 表达式
来源：http://ej.jctech888.com.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://jb.panjiajie.cn

[U56] PHP：命名参数
来源：http://dj.bjjhwx.cn

f(a: 1, b: 2)
来源：http://mn.jctech888.com.cn

[U57] PHP：字符串插值
来源：http://xw.haigaiapp.cn

"值: {$a}"
来源：http://vw.shtwfgs.cn

[U58] PHP：数组三件套
来源：http://de.chemitech.net.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://to.chemitech.net.cn

[U59] PHP：自定义排序
来源：http://ax.9csxet.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://cu.yuntaijiaju.cn

[U60] PHP：JSON 编解码
来源：http://qk.jianghongdianzi.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ky.newstarts.cn

[U61] PHP：正则
来源：http://ho.shxzukj.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wh.panjiajie.cn

[U62] PHP：日期对象
来源：http://iw.nszjky.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://yl.bjjhwx.cn

[U63] PHP：文件读写
来源：http://ca.panjiajie.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://nc.huixinmuqiang.cn

[U64] PHP：目录遍历
来源：http://kb.huanxung.cn

glob("dir/*.php");  scandir("dir");
来源：http://hv.yuexingan06.cn

[U65] PHP：会话
来源：http://we.asd995.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://ti.huixiangedu.cn

[U66] PHP：设置 Cookie
来源：http://zy.jctech888.com.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://qz.shxzukj.cn

[U67] PHP：处理文件上传
来源：http://gj.hnjuh.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://cp.hnjuh.cn

[U68] PHP：PDO 连接
来源：http://od.hnjuh.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://in.hnjuh.cn

[U69] PHP：PDO 预处理
来源：http://sx.9csxet.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ss.huanxung.cn

[U70] PHP：PDO 事务
来源：http://nr.wgjwhj.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://uj.shtwfgs.cn

[U71] PHP：抛出异常
来源：http://od.chemitech.net.cn

throw new RuntimeException("失败", 500);
来源：http://iy.huanxung.cn

[U72] PHP：写错误日志
来源：http://av.nicolike.cn

error_log("失败: " . $e->getMessage());
来源：http://mc.lnxyls.cn

[U73] PHP：读取 ini 配置
来源：http://cg.huanxung.cn

parse_ini_file("config.ini", true)
来源：http://mm.colortex.cn

[U74] PHP：读取环境变量
来源：http://dr.bookmarksfly.cn

getenv("APP_ENV") ?: "production"
来源：http://ef.nicolike.cn

[U75] PHP：依赖注入
来源：http://nn.nicolike.cn

composer require psr/container
来源：http://po.jianghongdianzi.cn

[U76] PHP：简单路由
来源：http://zs.muxihuayi.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ab.szsharing.cn

[U77] PHP：模板渲染
来源：http://ev.newstarts.cn

composer require twig/twig
来源：http://vn.hnjuh.cn

[U78] PHP：单元测试
来源：http://gu.asd995.cn

composer require --dev phpunit/phpunit
来源：http://zt.gzmigu.cn

[U79] PHP：静态分析
来源：http://hv.szsharing.cn

composer require --dev phpstan/phpstan
来源：http://ah.newstarts.cn

[U80] PHP：代码规范修复
来源：http://yt.9csxet.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://ba.521024.cn

[U81] JS：初始化项目
来源：http://nx.wgjwhj.cn

npm init -y;  npm i express
来源：http://km.jianghongdianzi.cn

[U82] JS：package.json 脚本
来源：http://ts.lnxyls.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://zt.jctech888.com.cn

[U83] JS：ES Module 导入导出
来源：http://qa.521024.cn

export const a = 1;  import { a } from "./m.js";
来源：http://rk.nszjky.cn

[U84] JS：CommonJS 写法
来源：http://rj.szxytkj.cn

module.exports = { a };  const { a } = require("./m");
来源：http://yq.bookmarksfly.cn

[U85] JS：可选链
来源：http://jw.bookmarksfly.cn

a?.b?.c
来源：http://iw.chemitech.net.cn

[U86] JS：空值合并
来源：http://wp.huanxung.cn

a ?? b
来源：http://ga.wgjwhj.cn

[U87] JS：解构默认值
来源：http://zj.nszjky.cn

const { a = 1, b = 2 } = obj;
来源：http://jy.chemitech.net.cn

[U88] JS：对象展开合并
来源：http://xr.9csxet.cn

{ ...a, ...b }
来源：http://fk.bjjhwx.cn

[U89] JS：数组去重
来源：http://xi.muxihuayi.cn

[...new Set(arr)]
来源：http://ln.521024.cn

[U90] JS：数字数组排序
来源：http://wo.bookmarksfly.cn

[...arr].sort((a, b) => a - b)
来源：http://vr.huixiangedu.cn

[U91] JS：对象键值遍历
来源：http://gi.chemitech.net.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://eo.jianghongdianzi.cn

[U92] JS：深拷贝
来源：http://hg.jctech888.com.cn

structuredClone(obj)
来源：http://bg.hnjuh.cn

[U93] JS：模板字符串
来源：http://nr.yuntaijiaju.cn

`共 ${n} 条`
来源：http://sl.wgjwhj.cn

[U94] JS：箭头函数
来源：http://ll.colortex.cn

const double = x => x * 2;
来源：http://rn.newstarts.cn

[U95] JS：Promise 包装
来源：http://gq.szxytkj.cn

new Promise((resolve, reject) => {})
来源：http://ds.yuexingan06.cn

[U96] JS：async/await 与异常
来源：http://nx.colortex.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wm.szsharing.cn

[U97] JS：并发请求
来源：http://ac.jctech888.com.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://yv.asd995.cn

[U98] JS：fetch 带 JSON
来源：http://rz.huixiangedu.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://zz.asd995.cn

[U99] JS：事件监听
来源：http://eu.shxzskj.cn

el.addEventListener("click", e => {})
来源：http://ej.9csxet.cn

[U100] JS：DOM 查询
来源：http://np.newstarts.cn

document.querySelector(".item")
来源：http://bl.muxihuayi.cn

[U101] JS：classList 操作
来源：http://op.szsharing.cn

el.classList.toggle("active")
来源：http://lg.lnxyls.cn

[U102] JS：本地存储
来源：http://zu.gzmigu.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://an.chemitech.net.cn

[U103] JS：定时器
来源：http://ue.panjiajie.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://so.asd995.cn

[U104] JS：防抖
来源：http://rm.huanxung.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fu.9csxet.cn

[U105] JS：节流
来源：http://wc.bjjhwx.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ml.hnjuh.cn

[U106] JS：日期格式化
来源：http://ra.jianghongdianzi.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ta.newstarts.cn

[U107] JS：数字千分位
来源：http://oi.wgjwhj.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ks.bjjhwx.cn

[U108] JS：随机整数
来源：http://sd.lnxyls.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://be.shxzukj.cn

[U109] JS：数组分组
来源：http://os.nszjky.cn

Object.groupBy(arr, x => x.type)
来源：http://nr.521024.cn

[U110] JS：数组分块
来源：http://si.yuexingan06.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ow.haigaiapp.cn

[U111] JS：对象转 Map
来源：http://tz.shxzukj.cn

new Map(Object.entries(obj))
来源：http://sb.bjjhwx.cn

[U112] JS：字符串补位
来源：http://wh.nicolike.cn

"7".padStart(3, "0")
来源：http://jv.yuntaijiaju.cn

[U113] JS：正则替换全部
来源：http://yt.chemitech.net.cn

s.replaceAll("a", "b")
来源：http://cz.chemitech.net.cn

[U114] JS：JSON 深比较
来源：http://nc.bookmarksfly.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://ky.panjiajie.cn

[U115] JS：生成 UUID
来源：http://re.haigaiapp.cn

crypto.randomUUID()
来源：http://rm.jianghongdianzi.cn

[U116] JS：类型检查（JSDoc）
来源：http://jl.wgjwhj.cn

/** @param {string} name */ function f(name) {}
来源：http://qg.nszjky.cn

[U117] JS：单元测试
来源：http://zs.huanxung.cn

npm i -D vitest;  npx vitest
来源：http://ep.hnjuh.cn

[U118] JS：开发服务器
来源：http://ft.jctech888.com.cn

npm i -D vite;  npx vite
来源：http://ls.colortex.cn

[U119] JS：生产构建
来源：http://db.panjiajie.cn

npx vite build
来源：http://zd.huanxung.cn

[U120] JS：读取环境变量（Vite）
来源：http://cz.yuexingan06.cn

import.meta.env.VITE_API_URL
来源：http://em.szxytkj.cn

================================================================================
来源：http://po.hahajie.cn

统计汇总
来源：http://pg.gzmigu.cn

================================================================================
来源：http://de.9csxet.cn

按语言统计（条）：
来源：http://kb.bookmarksfly.cn

Python ......... 252
来源：http://dg.shxzskj.cn

PHP ............ 252
来源：http://bx.asd995.cn

JavaScript ..... 252
来源：http://qz.shxzskj.cn

TypeScript ..... 212
来源：http://vq.shtwfgs.cn

Java ........... 212
来源：http://ng.wgjwhj.cn

Go ............. 212
来源：http://df.gzmigu.cn

Ruby ........... 212
来源：http://lh.bjjhwx.cn

C# ............. 212
来源：http://hc.jianghongdianzi.cn

C .............. 30
来源：http://ov.jianghongdianzi.cn

C++ ............ 30
来源：http://dw.jianghongdianzi.cn

SQL ............ 90
来源：http://dd.szsharing.cn

Bash ........... 80
来源：http://si.chemitech.net.cn

Kotlin ......... 15
来源：http://md.wgjwhj.cn

Swift .......... 15
来源：http://sc.hnjuh.cn

Lua ............ 10
来源：http://qv.haigaiapp.cn

Perl ........... 10
来源：http://ip.9csxet.cn

Scala .......... 10
来源：http://vz.shtwfgs.cn

------------------------------------
来源：http://ce.nicolike.cn

合计 ........... 2106 条
来源：http://ft.hnjuh.cn

按章节统计：
来源：http://ux.newstarts.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ae.nicolike.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://iq.shxzukj.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ya.panjiajie.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hs.521024.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ab.colortex.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://xz.chemitech.net.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://dc.colortex.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wr.jctech888.com.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hp.nicolike.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://po.jianghongdianzi.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://fu.jctech888.com.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ei.yuexingan06.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ic.lnxyls.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://us.haigaiapp.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://js.bjjhwx.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://dd.shxzskj.cn

Q SQL 专题                              90
来源：http://jf.jctech888.com.cn

R Bash 专题                             80
来源：http://uz.521024.cn

S C / C++ 专题                          60
来源：http://fl.jianghongdianzi.cn

T 其他语言补充                          60
来源：http://vv.gzmigu.cn

U 高频实用片段                         120
来源：http://wz.haigaiapp.cn

------------------------------------
来源：http://kh.521024.cn

合计                                  2106 条
来源：http://uk.shxzukj.cn

--------------------------------------------------------------------------------
来源：http://fv.szxytkj.cn

使用提醒
来源：http://ia.hahajie.cn

--------------------------------------------------------------------------------
来源：http://xj.yuexingan06.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://bo.hahajie.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://vz.shxzskj.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://nl.9csxet.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://gf.yuexingan06.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ji.newstarts.cn

—— 文件结束 ——
来源：http://uw.huanxung.cn

================================================================================
来源：http://hp.hahajie.cn

程序语言常见例子速查手册（2024 版）
来源：http://dd.gzmigu.cn

Common Programming Examples Cheat Book
来源：http://vu.hnjuh.cn

================================================================================
来源：http://ij.shtwfgs.cn

【收录内容】
来源：http://wu.shtwfgs.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://gk.nicolike.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://bn.huanxung.cn

SQL · Bash · C · C++
来源：http://gl.jctech888.com.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wh.yuexingan06.cn

【使用说明】
来源：http://ex.hnjuh.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://un.nszjky.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ll.muxihuayi.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://sx.jianghongdianzi.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://gz.shtwfgs.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://rx.lnxyls.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wq.gzmigu.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ty.wgjwhj.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://jf.huanxung.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://qq.muxihuayi.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://gx.521024.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ht.wgjwhj.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://xl.huanxung.cn

【文件统计】
来源：http://ik.shxzskj.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ke.jctech888.com.cn

--------------------------------------------------------------------------------
来源：http://kn.yuexingan06.cn

目  录
来源：http://ph.muxihuayi.cn

--------------------------------------------------------------------------------
来源：http://mv.szxytkj.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://fi.jianghongdianzi.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://lx.yuexingan06.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://ct.hahajie.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://vu.nszjky.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://gy.521024.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://uo.jianghongdianzi.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://fv.chemitech.net.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://dv.shxzukj.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ee.haigaiapp.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://xk.hahajie.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://cs.lnxyls.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://jy.gzmigu.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://xh.asd995.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ny.shxzskj.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://sy.nszjky.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://nb.asd995.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ju.wgjwhj.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://zv.newstarts.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://kq.shxzukj.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://jc.gzmigu.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://qg.colortex.cn

================================================================================
来源：http://av.haigaiapp.cn

A. 基础语法与类型
来源：http://sq.huixinmuqiang.cn

================================================================================
来源：http://bd.newstarts.cn

[A01] Hello World
来源：http://pf.szsharing.cn

Py:   print("Hello, World!")
来源：http://bi.lnxyls.cn

PHP:  echo "Hello, World!";
来源：http://gt.hahajie.cn

JS:   console.log("Hello, World!");
来源：http://jj.hahajie.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://bi.9csxet.cn

Java: System.out.println("Hello, World!");
来源：http://xa.shxzskj.cn

Go:   fmt.Println("Hello, World!")
来源：http://hz.wgjwhj.cn

Ruby: puts "Hello, World!"
来源：http://ev.szxytkj.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://hm.newstarts.cn

[A02] 变量声明与赋值
来源：http://bt.bookmarksfly.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://yj.shxzukj.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://xt.szxytkj.cn

JS:   let name = "Alex"; const age = 20;
来源：http://rk.nicolike.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://yy.yuntaijiaju.cn

Java: String name = "Alex"; int age = 20;
来源：http://mj.szxytkj.cn

Go:   name := "Alex"; age := 20
来源：http://mn.huixinmuqiang.cn

Ruby: name = "Alex"; age = 20
来源：http://ea.wgjwhj.cn


<!-- 参考信息 -->