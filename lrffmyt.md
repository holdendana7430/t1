代发 wailian999

[U25] Py：CSV 按字典读
来源：http://kw.newstarts.cn

csv.DictReader(f)
来源：http://sx.yuexingan06.cn

[U26] Py：并发下载
来源：http://ta.newstarts.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://sw.jctech888.com.cn

[U27] Py：异步 HTTP
来源：http://me.muxihuayi.cn

aiohttp.ClientSession() 配合 async with
来源：http://ws.521024.cn

[U28] Py：类型别名
来源：http://yo.newstarts.cn

UserId = int
来源：http://uw.szsharing.cn

[U29] Py：属性校验
来源：http://wy.muxihuayi.cn

@property 与 @x.setter 配合
来源：http://wt.huanxung.cn

[U30] Py：数据类
来源：http://vn.huixiangedu.cn

@dataclass(slots=True)
来源：http://na.lnxyls.cn

[U31] Py：单测
来源：http://hj.huixiangedu.cn

python -m pytest -q
来源：http://if.szxytkj.cn

[U32] Py：代码格式化
来源：http://jl.panjiajie.cn

ruff format . && ruff check --fix .
来源：http://zn.521024.cn

[U33] Py：打包发布
来源：http://tn.chemitech.net.cn

python -m build  （依赖 pyproject.toml）
来源：http://kk.colortex.cn

[U34] Py：判断编码
来源：http://wj.asd995.cn

chardet.detect(raw)
来源：http://kk.huanxung.cn

[U35] Py：发送邮件
来源：http://ly.huanxung.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://pe.nszjky.cn

[U36] Py：定时任务
来源：http://uz.szxytkj.cn

schedule.every(10).minutes.do(job)
来源：http://at.haigaiapp.cn

[U37] Py：读写 Excel
来源：http://kr.521024.cn

pandas.read_excel / DataFrame.to_excel
来源：http://uj.chemitech.net.cn

[U38] Py：获取脚本所在目录
来源：http://xe.muxihuayi.cn

Path(__file__).resolve().parent
来源：http://bo.colortex.cn

[U39] Py：判断是否在交互环境
来源：http://as.huixinmuqiang.cn

sys.stdout.isatty()
来源：http://hd.wgjwhj.cn

[U40] Py：打印到标准错误
来源：http://zc.chemitech.net.cn

print("err", file=sys.stderr)
来源：http://lz.asd995.cn

[U41] PHP：初始化 Composer 项目
来源：http://wq.lnxyls.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://rl.yuexingan06.cn

[U42] PHP：PSR-4 自动加载
来源：http://oh.huixiangedu.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://rc.newstarts.cn

[U43] PHP：声明命名空间
来源：http://ug.jctech888.com.cn

namespace App\Http;
来源：http://yq.muxihuayi.cn

[U44] PHP：开启严格类型
来源：http://ho.asd995.cn

declare(strict_types=1);
来源：http://ne.wgjwhj.cn

[U45] PHP：类型声明与返回类型
来源：http://be.colortex.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://ou.haigaiapp.cn

[U46] PHP：可空类型
来源：http://ia.9csxet.cn

?string $name = null
来源：http://ol.huixinmuqiang.cn

[U47] PHP：联合类型
来源：http://bf.521024.cn

int|string $id
来源：http://or.hahajie.cn

[U48] PHP：纯枚举
来源：http://ms.521024.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://de.yuntaijiaju.cn

[U49] PHP：只读属性
来源：http://fa.bookmarksfly.cn

public readonly string $name
来源：http://st.shtwfgs.cn

[U50] PHP：构造器属性提升
来源：http://zj.hahajie.cn

public function __construct(private int $id) {}
来源：http://kd.chemitech.net.cn

[U51] PHP：数组解构
来源：http://xo.wgjwhj.cn

[$a, $b] = $arr;
来源：http://js.jctech888.com.cn

[U52] PHP：箭头函数
来源：http://jf.shxzskj.cn

$double = fn($x) => $x * 2;
来源：http://nc.muxihuayi.cn

[U53] PHP：空合并运算符
来源：http://pb.hnjuh.cn

$v = $a ?? $b ?? "default";
来源：http://ib.hnjuh.cn

[U54] PHP：空安全调用
来源：http://vh.jctech888.com.cn

$obj?->method()
来源：http://tr.wgjwhj.cn

[U55] PHP：match 表达式
来源：http://ka.asd995.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://lb.jianghongdianzi.cn

[U56] PHP：命名参数
来源：http://nj.shxzskj.cn

f(a: 1, b: 2)
来源：http://cr.bjjhwx.cn

[U57] PHP：字符串插值
来源：http://oj.yuntaijiaju.cn

"值: {$a}"
来源：http://cj.shtwfgs.cn

[U58] PHP：数组三件套
来源：http://bt.bookmarksfly.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://nr.521024.cn

[U59] PHP：自定义排序
来源：http://pa.nicolike.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://fo.huixinmuqiang.cn

[U60] PHP：JSON 编解码
来源：http://nr.gzmigu.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://nw.muxihuayi.cn

[U61] PHP：正则
来源：http://nc.shxzskj.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://fa.szxytkj.cn

[U62] PHP：日期对象
来源：http://wl.yuexingan06.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://jv.yuexingan06.cn

[U63] PHP：文件读写
来源：http://up.panjiajie.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://eh.wgjwhj.cn

[U64] PHP：目录遍历
来源：http://du.panjiajie.cn

glob("dir/*.php");  scandir("dir");
来源：http://ej.yuexingan06.cn

[U65] PHP：会话
来源：http://io.bookmarksfly.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://ka.chemitech.net.cn

[U66] PHP：设置 Cookie
来源：http://vd.lnxyls.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ys.newstarts.cn

[U67] PHP：处理文件上传
来源：http://ql.panjiajie.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://yv.bjjhwx.cn

[U68] PHP：PDO 连接
来源：http://tz.shxzskj.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://fs.jctech888.com.cn

[U69] PHP：PDO 预处理
来源：http://ac.haigaiapp.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://je.hnjuh.cn

[U70] PHP：PDO 事务
来源：http://ip.jianghongdianzi.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://pp.hahajie.cn

[U71] PHP：抛出异常
来源：http://gs.jianghongdianzi.cn

throw new RuntimeException("失败", 500);
来源：http://ri.huixiangedu.cn

[U72] PHP：写错误日志
来源：http://pm.lnxyls.cn

error_log("失败: " . $e->getMessage());
来源：http://ub.newstarts.cn

[U73] PHP：读取 ini 配置
来源：http://fm.chemitech.net.cn

parse_ini_file("config.ini", true)
来源：http://nn.bjjhwx.cn

[U74] PHP：读取环境变量
来源：http://cm.bjjhwx.cn

getenv("APP_ENV") ?: "production"
来源：http://ag.shxzskj.cn

[U75] PHP：依赖注入
来源：http://gx.wgjwhj.cn

composer require psr/container
来源：http://ts.9csxet.cn

[U76] PHP：简单路由
来源：http://zl.hnjuh.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://fb.asd995.cn

[U77] PHP：模板渲染
来源：http://uw.colortex.cn

composer require twig/twig
来源：http://mg.asd995.cn

[U78] PHP：单元测试
来源：http://ko.shxzskj.cn

composer require --dev phpunit/phpunit
来源：http://ra.asd995.cn

[U79] PHP：静态分析
来源：http://bx.szxytkj.cn

composer require --dev phpstan/phpstan
来源：http://nq.nszjky.cn

[U80] PHP：代码规范修复
来源：http://ge.yuexingan06.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://io.hahajie.cn

[U81] JS：初始化项目
来源：http://yc.521024.cn

npm init -y;  npm i express
来源：http://er.huixinmuqiang.cn

[U82] JS：package.json 脚本
来源：http://ti.chemitech.net.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://yh.asd995.cn

[U83] JS：ES Module 导入导出
来源：http://lo.lnxyls.cn

export const a = 1;  import { a } from "./m.js";
来源：http://oi.jctech888.com.cn

[U84] JS：CommonJS 写法
来源：http://ti.lnxyls.cn

module.exports = { a };  const { a } = require("./m");
来源：http://pu.shxzskj.cn

[U85] JS：可选链
来源：http://qr.chemitech.net.cn

a?.b?.c
来源：http://ua.521024.cn

[U86] JS：空值合并
来源：http://yo.bookmarksfly.cn

a ?? b
来源：http://jd.9csxet.cn

[U87] JS：解构默认值
来源：http://eu.jctech888.com.cn

const { a = 1, b = 2 } = obj;
来源：http://hb.yuexingan06.cn

[U88] JS：对象展开合并
来源：http://gp.szxytkj.cn

{ ...a, ...b }
来源：http://ab.huanxung.cn

[U89] JS：数组去重
来源：http://js.szsharing.cn

[...new Set(arr)]
来源：http://qf.yuntaijiaju.cn

[U90] JS：数字数组排序
来源：http://dv.hahajie.cn

[...arr].sort((a, b) => a - b)
来源：http://lk.haigaiapp.cn

[U91] JS：对象键值遍历
来源：http://po.hahajie.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://om.9csxet.cn

[U92] JS：深拷贝
来源：http://gq.chemitech.net.cn

structuredClone(obj)
来源：http://ma.asd995.cn

[U93] JS：模板字符串
来源：http://sn.szxytkj.cn

`共 ${n} 条`
来源：http://zo.jianghongdianzi.cn

[U94] JS：箭头函数
来源：http://yi.panjiajie.cn

const double = x => x * 2;
来源：http://qw.huanxung.cn

[U95] JS：Promise 包装
来源：http://pt.huixinmuqiang.cn

new Promise((resolve, reject) => {})
来源：http://js.521024.cn

[U96] JS：async/await 与异常
来源：http://ze.asd995.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://yl.nszjky.cn

[U97] JS：并发请求
来源：http://nk.bookmarksfly.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://co.nszjky.cn

[U98] JS：fetch 带 JSON
来源：http://qi.panjiajie.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ae.lnxyls.cn

[U99] JS：事件监听
来源：http://pc.huixiangedu.cn

el.addEventListener("click", e => {})
来源：http://lh.jctech888.com.cn

[U100] JS：DOM 查询
来源：http://um.9csxet.cn

document.querySelector(".item")
来源：http://ha.lnxyls.cn

[U101] JS：classList 操作
来源：http://qm.lnxyls.cn

el.classList.toggle("active")
来源：http://ru.shtwfgs.cn

[U102] JS：本地存储
来源：http://ka.huixinmuqiang.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://dt.muxihuayi.cn

[U103] JS：定时器
来源：http://bf.nicolike.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://bp.yuntaijiaju.cn

[U104] JS：防抖
来源：http://wk.shtwfgs.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jw.bookmarksfly.cn

[U105] JS：节流
来源：http://yc.hahajie.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ti.gzmigu.cn

[U106] JS：日期格式化
来源：http://zc.jianghongdianzi.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ra.wgjwhj.cn

[U107] JS：数字千分位
来源：http://fr.521024.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ur.jctech888.com.cn

[U108] JS：随机整数
来源：http://zv.hahajie.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://uw.jianghongdianzi.cn

[U109] JS：数组分组
来源：http://md.muxihuayi.cn

Object.groupBy(arr, x => x.type)
来源：http://rs.shxzukj.cn

[U110] JS：数组分块
来源：http://su.panjiajie.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ax.nszjky.cn

[U111] JS：对象转 Map
来源：http://gh.yuntaijiaju.cn

new Map(Object.entries(obj))
来源：http://rv.shxzukj.cn

[U112] JS：字符串补位
来源：http://fd.newstarts.cn

"7".padStart(3, "0")
来源：http://tb.shtwfgs.cn

[U113] JS：正则替换全部
来源：http://us.huixinmuqiang.cn

s.replaceAll("a", "b")
来源：http://gl.huanxung.cn

[U114] JS：JSON 深比较
来源：http://fr.shxzukj.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://ez.gzmigu.cn

[U115] JS：生成 UUID
来源：http://ip.huanxung.cn

crypto.randomUUID()
来源：http://tr.szsharing.cn

[U116] JS：类型检查（JSDoc）
来源：http://qn.newstarts.cn

/** @param {string} name */ function f(name) {}
来源：http://uy.muxihuayi.cn

[U117] JS：单元测试
来源：http://gr.huixinmuqiang.cn

npm i -D vitest;  npx vitest
来源：http://fh.gzmigu.cn

[U118] JS：开发服务器
来源：http://tz.nicolike.cn

npm i -D vite;  npx vite
来源：http://qz.colortex.cn

[U119] JS：生产构建
来源：http://vw.521024.cn

npx vite build
来源：http://tg.yuntaijiaju.cn

[U120] JS：读取环境变量（Vite）
来源：http://sq.gzmigu.cn

import.meta.env.VITE_API_URL
来源：http://zr.bjjhwx.cn

================================================================================
来源：http://oy.huixinmuqiang.cn

统计汇总
来源：http://kk.chemitech.net.cn

================================================================================
来源：http://fy.hnjuh.cn

按语言统计（条）：
来源：http://tf.newstarts.cn

Python ......... 252
来源：http://ff.huanxung.cn

PHP ............ 252
来源：http://kg.wgjwhj.cn

JavaScript ..... 252
来源：http://in.huanxung.cn

TypeScript ..... 212
来源：http://pj.haigaiapp.cn

Java ........... 212
来源：http://lj.huixiangedu.cn

Go ............. 212
来源：http://cv.yuexingan06.cn

Ruby ........... 212
来源：http://pz.asd995.cn

C# ............. 212
来源：http://bl.muxihuayi.cn

C .............. 30
来源：http://vl.shxzukj.cn

C++ ............ 30
来源：http://bg.yuntaijiaju.cn

SQL ............ 90
来源：http://pb.hnjuh.cn

Bash ........... 80
来源：http://si.shxzukj.cn

Kotlin ......... 15
来源：http://pr.bookmarksfly.cn

Swift .......... 15
来源：http://kd.huixinmuqiang.cn

Lua ............ 10
来源：http://co.asd995.cn

Perl ........... 10
来源：http://cf.9csxet.cn

Scala .......... 10
来源：http://lz.lnxyls.cn

------------------------------------
来源：http://xk.jianghongdianzi.cn

合计 ........... 2106 条
来源：http://vd.lnxyls.cn

按章节统计：
来源：http://ky.huixiangedu.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://pz.bookmarksfly.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ip.huixinmuqiang.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://we.9csxet.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ri.asd995.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://nd.wgjwhj.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://yd.panjiajie.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://st.9csxet.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://zr.huanxung.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://pt.haigaiapp.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://pn.panjiajie.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://xl.nszjky.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://cs.gzmigu.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://zf.jianghongdianzi.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hf.shxzukj.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://cy.asd995.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://gx.nszjky.cn

Q SQL 专题                              90
来源：http://pu.521024.cn

R Bash 专题                             80
来源：http://yg.9csxet.cn

S C / C++ 专题                          60
来源：http://ny.huixiangedu.cn

T 其他语言补充                          60
来源：http://hd.panjiajie.cn

U 高频实用片段                         120
来源：http://tw.yuntaijiaju.cn

------------------------------------
来源：http://uj.bookmarksfly.cn

合计                                  2106 条
来源：http://we.szxytkj.cn

--------------------------------------------------------------------------------
来源：http://dl.haigaiapp.cn

使用提醒
来源：http://hb.panjiajie.cn

--------------------------------------------------------------------------------
来源：http://su.shtwfgs.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://fl.huanxung.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://gh.szxytkj.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ec.yuexingan06.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://nu.jianghongdianzi.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://kk.huixiangedu.cn

—— 文件结束 ——
来源：http://mk.jctech888.com.cn

================================================================================
来源：http://tj.lnxyls.cn

程序语言常见例子速查手册（2024 版）
来源：http://pw.wgjwhj.cn

Common Programming Examples Cheat Book
来源：http://lz.chemitech.net.cn

================================================================================
来源：http://ya.9csxet.cn

【收录内容】
来源：http://wb.hahajie.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://jz.huanxung.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://yd.yuexingan06.cn

SQL · Bash · C · C++
来源：http://ev.bookmarksfly.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://sz.hahajie.cn

【使用说明】
来源：http://aj.muxihuayi.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://bh.haigaiapp.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://yp.nszjky.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://nj.bjjhwx.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://in.nszjky.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://gz.chemitech.net.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://xa.asd995.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://bu.yuntaijiaju.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ia.muxihuayi.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://im.lnxyls.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://jw.panjiajie.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://vt.colortex.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ha.newstarts.cn

【文件统计】
来源：http://va.szxytkj.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://pg.huixiangedu.cn

--------------------------------------------------------------------------------
来源：http://aj.lnxyls.cn

目  录
来源：http://kd.hahajie.cn

--------------------------------------------------------------------------------
来源：http://dr.shxzskj.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://yt.gzmigu.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://nt.bjjhwx.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://ij.gzmigu.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ri.bjjhwx.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://kn.shxzukj.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://wy.colortex.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://ou.bookmarksfly.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://tk.haigaiapp.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://lu.jianghongdianzi.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://id.gzmigu.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://nz.jctech888.com.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://ae.huixinmuqiang.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://ie.haigaiapp.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://th.bjjhwx.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://dg.521024.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://wk.newstarts.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://pl.nicolike.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://nb.yuntaijiaju.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://ec.colortex.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://yc.yuntaijiaju.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mw.wgjwhj.cn

================================================================================
来源：http://ym.huixiangedu.cn

A. 基础语法与类型
来源：http://bs.haigaiapp.cn

================================================================================
来源：http://dl.chemitech.net.cn

[A01] Hello World
来源：http://dk.huixiangedu.cn


<!-- 参考信息 -->