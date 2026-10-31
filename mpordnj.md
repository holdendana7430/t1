代发 wailian999

[U23] Py：分块读取大文件
来源：http://dp.wgjwhj.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://zy.szxytkj.cn

[U24] Py：路径操作
来源：http://qz.jctech888.com.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://qv.nszjky.cn

[U25] Py：CSV 按字典读
来源：http://cf.haigaiapp.cn

csv.DictReader(f)
来源：http://xo.shxzskj.cn

[U26] Py：并发下载
来源：http://tr.colortex.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://eb.shxzskj.cn

[U27] Py：异步 HTTP
来源：http://zl.jianghongdianzi.cn

aiohttp.ClientSession() 配合 async with
来源：http://pp.huanxung.cn

[U28] Py：类型别名
来源：http://dn.muxihuayi.cn

UserId = int
来源：http://jg.9csxet.cn

[U29] Py：属性校验
来源：http://wn.panjiajie.cn

@property 与 @x.setter 配合
来源：http://na.huixiangedu.cn

[U30] Py：数据类
来源：http://bj.shxzukj.cn

@dataclass(slots=True)
来源：http://bz.nicolike.cn

[U31] Py：单测
来源：http://gp.hnjuh.cn

python -m pytest -q
来源：http://kj.shxzskj.cn

[U32] Py：代码格式化
来源：http://di.521024.cn

ruff format . && ruff check --fix .
来源：http://gk.wgjwhj.cn

[U33] Py：打包发布
来源：http://ht.jctech888.com.cn

python -m build  （依赖 pyproject.toml）
来源：http://an.newstarts.cn

[U34] Py：判断编码
来源：http://cl.shxzskj.cn

chardet.detect(raw)
来源：http://xl.shxzskj.cn

[U35] Py：发送邮件
来源：http://mn.nicolike.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://pt.lnxyls.cn

[U36] Py：定时任务
来源：http://vd.wgjwhj.cn

schedule.every(10).minutes.do(job)
来源：http://yn.chemitech.net.cn

[U37] Py：读写 Excel
来源：http://sp.jianghongdianzi.cn

pandas.read_excel / DataFrame.to_excel
来源：http://xl.shtwfgs.cn

[U38] Py：获取脚本所在目录
来源：http://tf.gzmigu.cn

Path(__file__).resolve().parent
来源：http://nv.huixiangedu.cn

[U39] Py：判断是否在交互环境
来源：http://ra.szxytkj.cn

sys.stdout.isatty()
来源：http://ce.gzmigu.cn

[U40] Py：打印到标准错误
来源：http://gr.gzmigu.cn

print("err", file=sys.stderr)
来源：http://px.huixinmuqiang.cn

[U41] PHP：初始化 Composer 项目
来源：http://oz.chemitech.net.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://dd.yuntaijiaju.cn

[U42] PHP：PSR-4 自动加载
来源：http://bv.shxzukj.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://fw.colortex.cn

[U43] PHP：声明命名空间
来源：http://ot.lnxyls.cn

namespace App\Http;
来源：http://rk.yuntaijiaju.cn

[U44] PHP：开启严格类型
来源：http://kl.nicolike.cn

declare(strict_types=1);
来源：http://jo.hahajie.cn

[U45] PHP：类型声明与返回类型
来源：http://lc.asd995.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://it.gzmigu.cn

[U46] PHP：可空类型
来源：http://ck.newstarts.cn

?string $name = null
来源：http://dn.shxzskj.cn

[U47] PHP：联合类型
来源：http://up.wgjwhj.cn

int|string $id
来源：http://wn.huixiangedu.cn

[U48] PHP：纯枚举
来源：http://iz.szsharing.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ki.hahajie.cn

[U49] PHP：只读属性
来源：http://qa.muxihuayi.cn

public readonly string $name
来源：http://nu.nszjky.cn

[U50] PHP：构造器属性提升
来源：http://ji.huanxung.cn

public function __construct(private int $id) {}
来源：http://te.gzmigu.cn

[U51] PHP：数组解构
来源：http://kw.521024.cn

[$a, $b] = $arr;
来源：http://zs.shxzukj.cn

[U52] PHP：箭头函数
来源：http://hx.asd995.cn

$double = fn($x) => $x * 2;
来源：http://om.jctech888.com.cn

[U53] PHP：空合并运算符
来源：http://vw.lnxyls.cn

$v = $a ?? $b ?? "default";
来源：http://zg.huanxung.cn

[U54] PHP：空安全调用
来源：http://jg.lnxyls.cn

$obj?->method()
来源：http://vw.521024.cn

[U55] PHP：match 表达式
来源：http://cp.colortex.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://dv.shxzskj.cn

[U56] PHP：命名参数
来源：http://xo.521024.cn

f(a: 1, b: 2)
来源：http://gs.colortex.cn

[U57] PHP：字符串插值
来源：http://gj.jianghongdianzi.cn

"值: {$a}"
来源：http://tm.newstarts.cn

[U58] PHP：数组三件套
来源：http://ph.huixinmuqiang.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ul.newstarts.cn

[U59] PHP：自定义排序
来源：http://ak.huixiangedu.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wo.9csxet.cn

[U60] PHP：JSON 编解码
来源：http://ai.nszjky.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://zq.bookmarksfly.cn

[U61] PHP：正则
来源：http://ir.yuntaijiaju.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://du.panjiajie.cn

[U62] PHP：日期对象
来源：http://jn.shxzskj.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://vm.szsharing.cn

[U63] PHP：文件读写
来源：http://mk.haigaiapp.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://vn.panjiajie.cn

[U64] PHP：目录遍历
来源：http://ds.huixiangedu.cn

glob("dir/*.php");  scandir("dir");
来源：http://qc.jianghongdianzi.cn

[U65] PHP：会话
来源：http://zt.nicolike.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://pq.nszjky.cn

[U66] PHP：设置 Cookie
来源：http://on.colortex.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://pz.gzmigu.cn

[U67] PHP：处理文件上传
来源：http://fc.haigaiapp.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://jm.nicolike.cn

[U68] PHP：PDO 连接
来源：http://pm.colortex.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://bf.shtwfgs.cn

[U69] PHP：PDO 预处理
来源：http://ta.gzmigu.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://rp.huixinmuqiang.cn

[U70] PHP：PDO 事务
来源：http://xd.haigaiapp.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://vr.hnjuh.cn

[U71] PHP：抛出异常
来源：http://na.szxytkj.cn

throw new RuntimeException("失败", 500);
来源：http://xg.szxytkj.cn

[U72] PHP：写错误日志
来源：http://ma.chemitech.net.cn

error_log("失败: " . $e->getMessage());
来源：http://so.huixiangedu.cn

[U73] PHP：读取 ini 配置
来源：http://xz.yuntaijiaju.cn

parse_ini_file("config.ini", true)
来源：http://wa.hnjuh.cn

[U74] PHP：读取环境变量
来源：http://ao.jianghongdianzi.cn

getenv("APP_ENV") ?: "production"
来源：http://ka.nicolike.cn

[U75] PHP：依赖注入
来源：http://um.nszjky.cn

composer require psr/container
来源：http://ly.panjiajie.cn

[U76] PHP：简单路由
来源：http://sh.huixinmuqiang.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://xj.colortex.cn

[U77] PHP：模板渲染
来源：http://rb.hahajie.cn

composer require twig/twig
来源：http://jx.hnjuh.cn

[U78] PHP：单元测试
来源：http://yg.szxytkj.cn

composer require --dev phpunit/phpunit
来源：http://xt.gzmigu.cn

[U79] PHP：静态分析
来源：http://cs.szxytkj.cn

composer require --dev phpstan/phpstan
来源：http://uo.hnjuh.cn

[U80] PHP：代码规范修复
来源：http://rx.szsharing.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://ar.shxzskj.cn

[U81] JS：初始化项目
来源：http://ge.szsharing.cn

npm init -y;  npm i express
来源：http://oy.nicolike.cn

[U82] JS：package.json 脚本
来源：http://ff.szxytkj.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ki.muxihuayi.cn

[U83] JS：ES Module 导入导出
来源：http://yg.haigaiapp.cn

export const a = 1;  import { a } from "./m.js";
来源：http://zi.colortex.cn

[U84] JS：CommonJS 写法
来源：http://bw.shxzskj.cn

module.exports = { a };  const { a } = require("./m");
来源：http://rf.yuexingan06.cn

[U85] JS：可选链
来源：http://la.yuexingan06.cn

a?.b?.c
来源：http://qr.lnxyls.cn

[U86] JS：空值合并
来源：http://ei.shxzukj.cn

a ?? b
来源：http://sl.colortex.cn

[U87] JS：解构默认值
来源：http://lc.yuexingan06.cn

const { a = 1, b = 2 } = obj;
来源：http://yv.newstarts.cn

[U88] JS：对象展开合并
来源：http://at.hahajie.cn

{ ...a, ...b }
来源：http://lk.huixinmuqiang.cn

[U89] JS：数组去重
来源：http://ko.yuntaijiaju.cn

[...new Set(arr)]
来源：http://qs.shxzukj.cn

[U90] JS：数字数组排序
来源：http://lu.huixinmuqiang.cn

[...arr].sort((a, b) => a - b)
来源：http://es.yuntaijiaju.cn

[U91] JS：对象键值遍历
来源：http://cw.colortex.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mm.521024.cn

[U92] JS：深拷贝
来源：http://zd.shtwfgs.cn

structuredClone(obj)
来源：http://jc.bjjhwx.cn

[U93] JS：模板字符串
来源：http://it.nicolike.cn

`共 ${n} 条`
来源：http://xj.colortex.cn

[U94] JS：箭头函数
来源：http://js.bookmarksfly.cn

const double = x => x * 2;
来源：http://ns.9csxet.cn

[U95] JS：Promise 包装
来源：http://ro.haigaiapp.cn

new Promise((resolve, reject) => {})
来源：http://wv.gzmigu.cn

[U96] JS：async/await 与异常
来源：http://bj.9csxet.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://yb.huixinmuqiang.cn

[U97] JS：并发请求
来源：http://sn.gzmigu.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://sy.wgjwhj.cn

[U98] JS：fetch 带 JSON
来源：http://yw.nszjky.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://sw.nszjky.cn

[U99] JS：事件监听
来源：http://cm.shtwfgs.cn

el.addEventListener("click", e => {})
来源：http://fc.hnjuh.cn

[U100] JS：DOM 查询
来源：http://bs.asd995.cn

document.querySelector(".item")
来源：http://us.shxzukj.cn

[U101] JS：classList 操作
来源：http://wo.yuexingan06.cn

el.classList.toggle("active")
来源：http://ri.yuexingan06.cn

[U102] JS：本地存储
来源：http://ts.lnxyls.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ek.yuntaijiaju.cn

[U103] JS：定时器
来源：http://qv.hahajie.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://xs.panjiajie.cn

[U104] JS：防抖
来源：http://zo.panjiajie.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://sw.shtwfgs.cn

[U105] JS：节流
来源：http://wc.wgjwhj.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://pi.wgjwhj.cn

[U106] JS：日期格式化
来源：http://iu.yuntaijiaju.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ir.nszjky.cn

[U107] JS：数字千分位
来源：http://he.shxzukj.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://vk.shxzukj.cn

[U108] JS：随机整数
来源：http://js.newstarts.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://uu.yuexingan06.cn

[U109] JS：数组分组
来源：http://ee.muxihuayi.cn

Object.groupBy(arr, x => x.type)
来源：http://yw.jctech888.com.cn

[U110] JS：数组分块
来源：http://sc.panjiajie.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://uy.muxihuayi.cn

[U111] JS：对象转 Map
来源：http://mb.shtwfgs.cn

new Map(Object.entries(obj))
来源：http://sa.jianghongdianzi.cn

[U112] JS：字符串补位
来源：http://cp.521024.cn

"7".padStart(3, "0")
来源：http://dx.huixiangedu.cn

[U113] JS：正则替换全部
来源：http://mo.nszjky.cn

s.replaceAll("a", "b")
来源：http://ld.szsharing.cn

[U114] JS：JSON 深比较
来源：http://cd.huixinmuqiang.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://qr.muxihuayi.cn

[U115] JS：生成 UUID
来源：http://aq.jianghongdianzi.cn

crypto.randomUUID()
来源：http://qo.chemitech.net.cn

[U116] JS：类型检查（JSDoc）
来源：http://xv.muxihuayi.cn

/** @param {string} name */ function f(name) {}
来源：http://ca.haigaiapp.cn

[U117] JS：单元测试
来源：http://sk.hahajie.cn

npm i -D vitest;  npx vitest
来源：http://wx.9csxet.cn

[U118] JS：开发服务器
来源：http://vn.huanxung.cn

npm i -D vite;  npx vite
来源：http://iy.hahajie.cn

[U119] JS：生产构建
来源：http://tv.huanxung.cn

npx vite build
来源：http://rg.szsharing.cn

[U120] JS：读取环境变量（Vite）
来源：http://aq.szsharing.cn

import.meta.env.VITE_API_URL
来源：http://ra.szxytkj.cn

================================================================================
来源：http://ai.wgjwhj.cn

统计汇总
来源：http://us.szxytkj.cn

================================================================================
来源：http://ia.huixinmuqiang.cn

按语言统计（条）：
来源：http://bm.shxzukj.cn

Python ......... 252
来源：http://pp.szxytkj.cn

PHP ............ 252
来源：http://gg.nicolike.cn

JavaScript ..... 252
来源：http://yw.asd995.cn

TypeScript ..... 212
来源：http://oh.nszjky.cn

Java ........... 212
来源：http://ar.jianghongdianzi.cn

Go ............. 212
来源：http://rp.jctech888.com.cn

Ruby ........... 212
来源：http://sv.jianghongdianzi.cn

C# ............. 212
来源：http://kr.jianghongdianzi.cn

C .............. 30
来源：http://id.asd995.cn

C++ ............ 30
来源：http://xz.bookmarksfly.cn

SQL ............ 90
来源：http://kk.huanxung.cn

Bash ........... 80
来源：http://pd.huixiangedu.cn

Kotlin ......... 15
来源：http://eo.bookmarksfly.cn

Swift .......... 15
来源：http://ng.colortex.cn

Lua ............ 10
来源：http://jp.hnjuh.cn

Perl ........... 10
来源：http://wy.szxytkj.cn

Scala .......... 10
来源：http://iq.jctech888.com.cn

------------------------------------
来源：http://yp.wgjwhj.cn

合计 ........... 2106 条
来源：http://rg.newstarts.cn

按章节统计：
来源：http://tl.jianghongdianzi.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://oh.yuntaijiaju.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://nh.wgjwhj.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ch.gzmigu.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://cy.shxzukj.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ve.huixiangedu.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://gq.colortex.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://yg.szxytkj.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://nl.panjiajie.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ir.bookmarksfly.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ac.bookmarksfly.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ci.huixiangedu.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ir.haigaiapp.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://oz.yuexingan06.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://jf.nicolike.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ib.muxihuayi.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://iv.muxihuayi.cn

Q SQL 专题                              90
来源：http://vd.gzmigu.cn

R Bash 专题                             80
来源：http://jj.shxzukj.cn

S C / C++ 专题                          60
来源：http://vg.lnxyls.cn

T 其他语言补充                          60
来源：http://cc.shtwfgs.cn

U 高频实用片段                         120
来源：http://vi.shtwfgs.cn

------------------------------------
来源：http://aq.bookmarksfly.cn

合计                                  2106 条
来源：http://ze.haigaiapp.cn

--------------------------------------------------------------------------------
来源：http://iy.nicolike.cn

使用提醒
来源：http://qy.521024.cn

--------------------------------------------------------------------------------
来源：http://xq.521024.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://tq.muxihuayi.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://gz.yuntaijiaju.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://jh.colortex.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://ro.nicolike.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://vg.asd995.cn

—— 文件结束 ——
来源：http://eq.bookmarksfly.cn

================================================================================
来源：http://oe.shxzskj.cn

程序语言常见例子速查手册（2024 版）
来源：http://qm.szxytkj.cn

Common Programming Examples Cheat Book
来源：http://ur.jctech888.com.cn

================================================================================
来源：http://kv.huixiangedu.cn

【收录内容】
来源：http://ea.shxzukj.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://fm.nszjky.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://mt.colortex.cn

SQL · Bash · C · C++
来源：http://ug.yuntaijiaju.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://oa.chemitech.net.cn

【使用说明】
来源：http://pa.gzmigu.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://md.hnjuh.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://kf.jianghongdianzi.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://sc.szxytkj.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://py.haigaiapp.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://kn.jianghongdianzi.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ni.panjiajie.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://rz.9csxet.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ue.hahajie.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://dp.bookmarksfly.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://zs.bookmarksfly.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://lp.szxytkj.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://zq.muxihuayi.cn

【文件统计】
来源：http://ol.yuexingan06.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://py.hahajie.cn

--------------------------------------------------------------------------------
来源：http://jj.jianghongdianzi.cn

目  录
来源：http://bj.yuexingan06.cn

--------------------------------------------------------------------------------
来源：http://yw.wgjwhj.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ic.jctech888.com.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://wr.panjiajie.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://tu.huixinmuqiang.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://yz.bjjhwx.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://kz.hahajie.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://yy.huanxung.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://su.yuntaijiaju.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://xy.nszjky.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://jt.huixinmuqiang.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://de.jianghongdianzi.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://wg.bjjhwx.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hp.haigaiapp.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://py.yuexingan06.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ii.wgjwhj.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://kh.panjiajie.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://jy.yuntaijiaju.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ym.gzmigu.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://ww.huixiangedu.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hg.wgjwhj.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ve.huixiangedu.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://pq.lnxyls.cn


<!-- 参考信息 -->