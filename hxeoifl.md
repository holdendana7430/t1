代发 wailian999

[U23] Py：分块读取大文件
来源：http://cz.szsharing.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://yl.huanxung.cn

[U24] Py：路径操作
来源：http://ry.gzmigu.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://xx.bjjhwx.cn

[U25] Py：CSV 按字典读
来源：http://hp.bookmarksfly.cn

csv.DictReader(f)
来源：http://bu.hahajie.cn

[U26] Py：并发下载
来源：http://td.haigaiapp.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://pj.newstarts.cn

[U27] Py：异步 HTTP
来源：http://oy.shtwfgs.cn

aiohttp.ClientSession() 配合 async with
来源：http://re.wgjwhj.cn

[U28] Py：类型别名
来源：http://gi.wgjwhj.cn

UserId = int
来源：http://we.gzmigu.cn

[U29] Py：属性校验
来源：http://qi.shtwfgs.cn

@property 与 @x.setter 配合
来源：http://vl.9csxet.cn

[U30] Py：数据类
来源：http://hk.colortex.cn

@dataclass(slots=True)
来源：http://zh.shxzukj.cn

[U31] Py：单测
来源：http://il.hnjuh.cn

python -m pytest -q
来源：http://ec.9csxet.cn

[U32] Py：代码格式化
来源：http://ot.huanxung.cn

ruff format . && ruff check --fix .
来源：http://ud.nicolike.cn

[U33] Py：打包发布
来源：http://lc.jctech888.com.cn

python -m build  （依赖 pyproject.toml）
来源：http://vn.nszjky.cn

[U34] Py：判断编码
来源：http://lq.shxzukj.cn

chardet.detect(raw)
来源：http://pq.newstarts.cn

[U35] Py：发送邮件
来源：http://io.huixiangedu.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://fr.panjiajie.cn

[U36] Py：定时任务
来源：http://zw.9csxet.cn

schedule.every(10).minutes.do(job)
来源：http://ji.nicolike.cn

[U37] Py：读写 Excel
来源：http://mz.huixinmuqiang.cn

pandas.read_excel / DataFrame.to_excel
来源：http://fb.colortex.cn

[U38] Py：获取脚本所在目录
来源：http://xd.hnjuh.cn

Path(__file__).resolve().parent
来源：http://pq.shxzskj.cn

[U39] Py：判断是否在交互环境
来源：http://gu.szsharing.cn

sys.stdout.isatty()
来源：http://jv.szxytkj.cn

[U40] Py：打印到标准错误
来源：http://sv.szxytkj.cn

print("err", file=sys.stderr)
来源：http://zd.shxzskj.cn

[U41] PHP：初始化 Composer 项目
来源：http://bw.chemitech.net.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://es.shtwfgs.cn

[U42] PHP：PSR-4 自动加载
来源：http://uo.shtwfgs.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://tj.yuntaijiaju.cn

[U43] PHP：声明命名空间
来源：http://hx.bookmarksfly.cn

namespace App\Http;
来源：http://wg.panjiajie.cn

[U44] PHP：开启严格类型
来源：http://bl.gzmigu.cn

declare(strict_types=1);
来源：http://cu.newstarts.cn

[U45] PHP：类型声明与返回类型
来源：http://bg.jianghongdianzi.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://vu.haigaiapp.cn

[U46] PHP：可空类型
来源：http://fq.wgjwhj.cn

?string $name = null
来源：http://gu.jctech888.com.cn

[U47] PHP：联合类型
来源：http://mk.panjiajie.cn

int|string $id
来源：http://nx.newstarts.cn

[U48] PHP：纯枚举
来源：http://pc.muxihuayi.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://gu.jianghongdianzi.cn

[U49] PHP：只读属性
来源：http://ob.nszjky.cn

public readonly string $name
来源：http://pp.hahajie.cn

[U50] PHP：构造器属性提升
来源：http://ok.shxzskj.cn

public function __construct(private int $id) {}
来源：http://zm.nicolike.cn

[U51] PHP：数组解构
来源：http://hi.nicolike.cn

[$a, $b] = $arr;
来源：http://db.wgjwhj.cn

[U52] PHP：箭头函数
来源：http://uy.colortex.cn

$double = fn($x) => $x * 2;
来源：http://fi.asd995.cn

[U53] PHP：空合并运算符
来源：http://ci.huanxung.cn

$v = $a ?? $b ?? "default";
来源：http://hh.panjiajie.cn

[U54] PHP：空安全调用
来源：http://pp.colortex.cn

$obj?->method()
来源：http://jw.huanxung.cn

[U55] PHP：match 表达式
来源：http://jo.asd995.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://am.bjjhwx.cn

[U56] PHP：命名参数
来源：http://vp.yuntaijiaju.cn

f(a: 1, b: 2)
来源：http://rd.jianghongdianzi.cn

[U57] PHP：字符串插值
来源：http://sa.521024.cn

"值: {$a}"
来源：http://xd.shxzukj.cn

[U58] PHP：数组三件套
来源：http://tq.chemitech.net.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://os.huanxung.cn

[U59] PHP：自定义排序
来源：http://ju.lnxyls.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ij.chemitech.net.cn

[U60] PHP：JSON 编解码
来源：http://hk.asd995.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://kx.szxytkj.cn

[U61] PHP：正则
来源：http://jo.9csxet.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://jx.huixiangedu.cn

[U62] PHP：日期对象
来源：http://vx.yuexingan06.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://yf.asd995.cn

[U63] PHP：文件读写
来源：http://ys.yuexingan06.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://gt.haigaiapp.cn

[U64] PHP：目录遍历
来源：http://pz.haigaiapp.cn

glob("dir/*.php");  scandir("dir");
来源：http://pc.jctech888.com.cn

[U65] PHP：会话
来源：http://vu.chemitech.net.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://gi.jctech888.com.cn

[U66] PHP：设置 Cookie
来源：http://mo.chemitech.net.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wk.nicolike.cn

[U67] PHP：处理文件上传
来源：http://aq.shxzskj.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://iw.yuexingan06.cn

[U68] PHP：PDO 连接
来源：http://la.huixinmuqiang.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://bu.szxytkj.cn

[U69] PHP：PDO 预处理
来源：http://qq.szsharing.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://dw.hnjuh.cn

[U70] PHP：PDO 事务
来源：http://rf.shxzskj.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://tr.nicolike.cn

[U71] PHP：抛出异常
来源：http://bb.muxihuayi.cn

throw new RuntimeException("失败", 500);
来源：http://sy.9csxet.cn

[U72] PHP：写错误日志
来源：http://ul.bookmarksfly.cn

error_log("失败: " . $e->getMessage());
来源：http://gf.haigaiapp.cn

[U73] PHP：读取 ini 配置
来源：http://sq.9csxet.cn

parse_ini_file("config.ini", true)
来源：http://pq.newstarts.cn

[U74] PHP：读取环境变量
来源：http://nf.bjjhwx.cn

getenv("APP_ENV") ?: "production"
来源：http://pt.shxzukj.cn

[U75] PHP：依赖注入
来源：http://zu.hahajie.cn

composer require psr/container
来源：http://xp.panjiajie.cn

[U76] PHP：简单路由
来源：http://nq.gzmigu.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://sd.colortex.cn

[U77] PHP：模板渲染
来源：http://du.haigaiapp.cn

composer require twig/twig
来源：http://au.bookmarksfly.cn

[U78] PHP：单元测试
来源：http://wi.wgjwhj.cn

composer require --dev phpunit/phpunit
来源：http://bl.huixinmuqiang.cn

[U79] PHP：静态分析
来源：http://oa.gzmigu.cn

composer require --dev phpstan/phpstan
来源：http://my.lnxyls.cn

[U80] PHP：代码规范修复
来源：http://kx.hnjuh.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://wf.shxzukj.cn

[U81] JS：初始化项目
来源：http://oq.huanxung.cn

npm init -y;  npm i express
来源：http://ka.yuexingan06.cn

[U82] JS：package.json 脚本
来源：http://lw.521024.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://yv.asd995.cn

[U83] JS：ES Module 导入导出
来源：http://ti.wgjwhj.cn

export const a = 1;  import { a } from "./m.js";
来源：http://iy.colortex.cn

[U84] JS：CommonJS 写法
来源：http://yz.hahajie.cn

module.exports = { a };  const { a } = require("./m");
来源：http://mb.nszjky.cn

[U85] JS：可选链
来源：http://dc.szxytkj.cn

a?.b?.c
来源：http://im.jctech888.com.cn

[U86] JS：空值合并
来源：http://xj.bookmarksfly.cn

a ?? b
来源：http://lc.colortex.cn

[U87] JS：解构默认值
来源：http://zn.nszjky.cn

const { a = 1, b = 2 } = obj;
来源：http://oe.nicolike.cn

[U88] JS：对象展开合并
来源：http://mv.nszjky.cn

{ ...a, ...b }
来源：http://ow.huanxung.cn

[U89] JS：数组去重
来源：http://fo.wgjwhj.cn

[...new Set(arr)]
来源：http://ui.wgjwhj.cn

[U90] JS：数字数组排序
来源：http://dj.bookmarksfly.cn

[...arr].sort((a, b) => a - b)
来源：http://qc.chemitech.net.cn

[U91] JS：对象键值遍历
来源：http://gc.9csxet.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://qc.newstarts.cn

[U92] JS：深拷贝
来源：http://tt.huanxung.cn

structuredClone(obj)
来源：http://fc.chemitech.net.cn

[U93] JS：模板字符串
来源：http://hx.huixiangedu.cn

`共 ${n} 条`
来源：http://yf.lnxyls.cn

[U94] JS：箭头函数
来源：http://gs.bookmarksfly.cn

const double = x => x * 2;
来源：http://px.bookmarksfly.cn

[U95] JS：Promise 包装
来源：http://hw.yuexingan06.cn

new Promise((resolve, reject) => {})
来源：http://md.haigaiapp.cn

[U96] JS：async/await 与异常
来源：http://vk.muxihuayi.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://by.lnxyls.cn

[U97] JS：并发请求
来源：http://qu.newstarts.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://rs.shxzskj.cn

[U98] JS：fetch 带 JSON
来源：http://as.jianghongdianzi.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://if.nszjky.cn

[U99] JS：事件监听
来源：http://tk.nicolike.cn

el.addEventListener("click", e => {})
来源：http://wb.szxytkj.cn

[U100] JS：DOM 查询
来源：http://pe.shxzukj.cn

document.querySelector(".item")
来源：http://vn.asd995.cn

[U101] JS：classList 操作
来源：http://ix.bookmarksfly.cn

el.classList.toggle("active")
来源：http://dn.chemitech.net.cn

[U102] JS：本地存储
来源：http://vw.szxytkj.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://yr.hahajie.cn

[U103] JS：定时器
来源：http://ei.huanxung.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://qn.lnxyls.cn

[U104] JS：防抖
来源：http://lj.9csxet.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xu.jctech888.com.cn

[U105] JS：节流
来源：http://er.bookmarksfly.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://cf.asd995.cn

[U106] JS：日期格式化
来源：http://xv.wgjwhj.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://sz.asd995.cn

[U107] JS：数字千分位
来源：http://sl.colortex.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ic.huixiangedu.cn

[U108] JS：随机整数
来源：http://mw.yuntaijiaju.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://vu.szsharing.cn

[U109] JS：数组分组
来源：http://ma.jianghongdianzi.cn

Object.groupBy(arr, x => x.type)
来源：http://mb.gzmigu.cn

[U110] JS：数组分块
来源：http://xi.muxihuayi.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://vp.yuntaijiaju.cn

[U111] JS：对象转 Map
来源：http://ll.nszjky.cn

new Map(Object.entries(obj))
来源：http://bk.jianghongdianzi.cn

[U112] JS：字符串补位
来源：http://px.9csxet.cn

"7".padStart(3, "0")
来源：http://hb.yuexingan06.cn

[U113] JS：正则替换全部
来源：http://ez.asd995.cn

s.replaceAll("a", "b")
来源：http://pt.yuexingan06.cn

[U114] JS：JSON 深比较
来源：http://nb.muxihuayi.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://bm.colortex.cn

[U115] JS：生成 UUID
来源：http://ew.bookmarksfly.cn

crypto.randomUUID()
来源：http://ur.lnxyls.cn

[U116] JS：类型检查（JSDoc）
来源：http://xt.huixiangedu.cn

/** @param {string} name */ function f(name) {}
来源：http://sc.nszjky.cn

[U117] JS：单元测试
来源：http://ij.hnjuh.cn

npm i -D vitest;  npx vitest
来源：http://wg.nszjky.cn

[U118] JS：开发服务器
来源：http://ph.colortex.cn

npm i -D vite;  npx vite
来源：http://mm.shxzskj.cn

[U119] JS：生产构建
来源：http://sb.chemitech.net.cn

npx vite build
来源：http://tt.wgjwhj.cn

[U120] JS：读取环境变量（Vite）
来源：http://px.newstarts.cn

import.meta.env.VITE_API_URL
来源：http://fg.szsharing.cn

================================================================================
来源：http://zx.bookmarksfly.cn

统计汇总
来源：http://is.wgjwhj.cn

================================================================================
来源：http://zc.szsharing.cn

按语言统计（条）：
来源：http://dh.gzmigu.cn

Python ......... 252
来源：http://pm.lnxyls.cn

PHP ............ 252
来源：http://pa.jctech888.com.cn

JavaScript ..... 252
来源：http://ig.lnxyls.cn

TypeScript ..... 212
来源：http://cn.shxzskj.cn

Java ........... 212
来源：http://og.gzmigu.cn

Go ............. 212
来源：http://ro.muxihuayi.cn

Ruby ........... 212
来源：http://sh.huanxung.cn

C# ............. 212
来源：http://yi.haigaiapp.cn

C .............. 30
来源：http://ub.bjjhwx.cn

C++ ............ 30
来源：http://ff.shxzukj.cn

SQL ............ 90
来源：http://ps.jianghongdianzi.cn

Bash ........... 80
来源：http://ys.shxzukj.cn

Kotlin ......... 15
来源：http://dk.huixinmuqiang.cn

Swift .......... 15
来源：http://to.jianghongdianzi.cn

Lua ............ 10
来源：http://aa.jianghongdianzi.cn

Perl ........... 10
来源：http://jx.szsharing.cn

Scala .......... 10
来源：http://dw.huixiangedu.cn

------------------------------------
来源：http://wi.shxzukj.cn

合计 ........... 2106 条
来源：http://ma.shtwfgs.cn

按章节统计：
来源：http://iu.asd995.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://in.gzmigu.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://jr.shxzukj.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://pe.szxytkj.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://dz.bjjhwx.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wg.bookmarksfly.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ip.shxzukj.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wa.muxihuayi.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://po.newstarts.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://jv.jctech888.com.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://sw.wgjwhj.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://bm.huixiangedu.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://jh.521024.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://tx.nicolike.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://dc.hahajie.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://bb.wgjwhj.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://sj.bookmarksfly.cn

Q SQL 专题                              90
来源：http://vz.newstarts.cn

R Bash 专题                             80
来源：http://vh.panjiajie.cn

S C / C++ 专题                          60
来源：http://wh.huixiangedu.cn

T 其他语言补充                          60
来源：http://vq.gzmigu.cn

U 高频实用片段                         120
来源：http://tk.colortex.cn

------------------------------------
来源：http://ko.jianghongdianzi.cn

合计                                  2106 条
来源：http://ip.chemitech.net.cn

--------------------------------------------------------------------------------
来源：http://so.9csxet.cn

使用提醒
来源：http://vp.szxytkj.cn

--------------------------------------------------------------------------------
来源：http://dd.bookmarksfly.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://qf.huanxung.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://bf.haigaiapp.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://yy.yuntaijiaju.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://rg.panjiajie.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://jc.shxzskj.cn

—— 文件结束 ——
来源：http://zr.yuntaijiaju.cn

================================================================================
来源：http://jy.521024.cn

程序语言常见例子速查手册（2024 版）
来源：http://lb.yuexingan06.cn

Common Programming Examples Cheat Book
来源：http://qq.szsharing.cn

================================================================================
来源：http://hc.huixinmuqiang.cn

【收录内容】
来源：http://hf.panjiajie.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://eu.521024.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://vf.asd995.cn

SQL · Bash · C · C++
来源：http://oi.hahajie.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://oi.gzmigu.cn

【使用说明】
来源：http://da.muxihuayi.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://em.hahajie.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ek.gzmigu.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://fn.shxzukj.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://qu.9csxet.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://nt.asd995.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://cd.bookmarksfly.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://za.haigaiapp.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://mb.bookmarksfly.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ou.hahajie.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://jg.chemitech.net.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://xh.shtwfgs.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://gv.huanxung.cn

【文件统计】
来源：http://dp.bjjhwx.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://cq.lnxyls.cn

--------------------------------------------------------------------------------
来源：http://qq.521024.cn

目  录
来源：http://af.shxzukj.cn

--------------------------------------------------------------------------------
来源：http://fh.shxzukj.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ta.bookmarksfly.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://mt.huanxung.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://dj.yuntaijiaju.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://tl.muxihuayi.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://bz.newstarts.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://af.panjiajie.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://nz.nszjky.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://za.lnxyls.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://cj.521024.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://dr.yuexingan06.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://lq.shxzukj.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://rf.lnxyls.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://rw.lnxyls.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://gf.gzmigu.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://sx.huixinmuqiang.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://jc.9csxet.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://fs.yuntaijiaju.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://ip.9csxet.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://jq.muxihuayi.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://je.9csxet.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://gb.521024.cn


<!-- 参考信息 -->