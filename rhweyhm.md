代发 wailian999

[U21] Py：自定义上下文管理器
来源：http://zm.colortex.cn

@contextlib.contextmanager
来源：http://ec.huanxung.cn

[U22] Py：矩阵转置
来源：http://ln.huixinmuqiang.cn

list(zip(*m))
来源：http://un.9csxet.cn

[U23] Py：分块读取大文件
来源：http://nf.bjjhwx.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ug.shxzskj.cn

[U24] Py：路径操作
来源：http://xo.gzmigu.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://kv.yuexingan06.cn

[U25] Py：CSV 按字典读
来源：http://pj.huixinmuqiang.cn

csv.DictReader(f)
来源：http://qs.wgjwhj.cn

[U26] Py：并发下载
来源：http://bi.shxzukj.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://lx.521024.cn

[U27] Py：异步 HTTP
来源：http://xe.wgjwhj.cn

aiohttp.ClientSession() 配合 async with
来源：http://ut.huixinmuqiang.cn

[U28] Py：类型别名
来源：http://bu.bookmarksfly.cn

UserId = int
来源：http://ol.newstarts.cn

[U29] Py：属性校验
来源：http://yf.hahajie.cn

@property 与 @x.setter 配合
来源：http://il.nicolike.cn

[U30] Py：数据类
来源：http://bh.nicolike.cn

@dataclass(slots=True)
来源：http://qn.szsharing.cn

[U31] Py：单测
来源：http://xc.9csxet.cn

python -m pytest -q
来源：http://jh.huanxung.cn

[U32] Py：代码格式化
来源：http://ed.wgjwhj.cn

ruff format . && ruff check --fix .
来源：http://ml.521024.cn

[U33] Py：打包发布
来源：http://fb.521024.cn

python -m build  （依赖 pyproject.toml）
来源：http://tl.muxihuayi.cn

[U34] Py：判断编码
来源：http://wd.szsharing.cn

chardet.detect(raw)
来源：http://sq.jianghongdianzi.cn

[U35] Py：发送邮件
来源：http://nt.hnjuh.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://zd.panjiajie.cn

[U36] Py：定时任务
来源：http://sm.huanxung.cn

schedule.every(10).minutes.do(job)
来源：http://gy.newstarts.cn

[U37] Py：读写 Excel
来源：http://lp.shtwfgs.cn

pandas.read_excel / DataFrame.to_excel
来源：http://rx.haigaiapp.cn

[U38] Py：获取脚本所在目录
来源：http://pl.gzmigu.cn

Path(__file__).resolve().parent
来源：http://pl.hnjuh.cn

[U39] Py：判断是否在交互环境
来源：http://ds.szsharing.cn

sys.stdout.isatty()
来源：http://sk.521024.cn

[U40] Py：打印到标准错误
来源：http://uq.shtwfgs.cn

print("err", file=sys.stderr)
来源：http://rj.haigaiapp.cn

[U41] PHP：初始化 Composer 项目
来源：http://nm.lnxyls.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://xj.521024.cn

[U42] PHP：PSR-4 自动加载
来源：http://kf.asd995.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://al.hnjuh.cn

[U43] PHP：声明命名空间
来源：http://xc.lnxyls.cn

namespace App\Http;
来源：http://wn.nicolike.cn

[U44] PHP：开启严格类型
来源：http://tt.shtwfgs.cn

declare(strict_types=1);
来源：http://sb.chemitech.net.cn

[U45] PHP：类型声明与返回类型
来源：http://xu.haigaiapp.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://og.bookmarksfly.cn

[U46] PHP：可空类型
来源：http://ci.lnxyls.cn

?string $name = null
来源：http://zt.muxihuayi.cn

[U47] PHP：联合类型
来源：http://vp.jianghongdianzi.cn

int|string $id
来源：http://da.szxytkj.cn

[U48] PHP：纯枚举
来源：http://ns.szxytkj.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://jx.szxytkj.cn

[U49] PHP：只读属性
来源：http://dp.gzmigu.cn

public readonly string $name
来源：http://aj.huixinmuqiang.cn

[U50] PHP：构造器属性提升
来源：http://jn.huixiangedu.cn

public function __construct(private int $id) {}
来源：http://uq.bjjhwx.cn

[U51] PHP：数组解构
来源：http://du.haigaiapp.cn

[$a, $b] = $arr;
来源：http://qj.colortex.cn

[U52] PHP：箭头函数
来源：http://lw.gzmigu.cn

$double = fn($x) => $x * 2;
来源：http://rr.huixinmuqiang.cn

[U53] PHP：空合并运算符
来源：http://ga.hnjuh.cn

$v = $a ?? $b ?? "default";
来源：http://qv.bookmarksfly.cn

[U54] PHP：空安全调用
来源：http://fa.bjjhwx.cn

$obj?->method()
来源：http://og.bookmarksfly.cn

[U55] PHP：match 表达式
来源：http://kr.yuexingan06.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://je.shxzukj.cn

[U56] PHP：命名参数
来源：http://hz.szxytkj.cn

f(a: 1, b: 2)
来源：http://ml.panjiajie.cn

[U57] PHP：字符串插值
来源：http://fl.nszjky.cn

"值: {$a}"
来源：http://rk.colortex.cn

[U58] PHP：数组三件套
来源：http://uh.hnjuh.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mo.huixiangedu.cn

[U59] PHP：自定义排序
来源：http://tc.bookmarksfly.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://up.9csxet.cn

[U60] PHP：JSON 编解码
来源：http://lx.asd995.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://fv.nicolike.cn

[U61] PHP：正则
来源：http://vc.gzmigu.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ct.chemitech.net.cn

[U62] PHP：日期对象
来源：http://mi.nicolike.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ld.shxzskj.cn

[U63] PHP：文件读写
来源：http://rg.nszjky.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://kj.muxihuayi.cn

[U64] PHP：目录遍历
来源：http://eo.szsharing.cn

glob("dir/*.php");  scandir("dir");
来源：http://qq.szsharing.cn

[U65] PHP：会话
来源：http://ik.colortex.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://ka.asd995.cn

[U66] PHP：设置 Cookie
来源：http://qa.asd995.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://km.bookmarksfly.cn

[U67] PHP：处理文件上传
来源：http://gr.muxihuayi.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://lh.9csxet.cn

[U68] PHP：PDO 连接
来源：http://mx.chemitech.net.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://rw.bjjhwx.cn

[U69] PHP：PDO 预处理
来源：http://kd.bjjhwx.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://op.panjiajie.cn

[U70] PHP：PDO 事务
来源：http://hu.jianghongdianzi.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://td.asd995.cn

[U71] PHP：抛出异常
来源：http://uq.huixiangedu.cn

throw new RuntimeException("失败", 500);
来源：http://ry.newstarts.cn

[U72] PHP：写错误日志
来源：http://jy.yuntaijiaju.cn

error_log("失败: " . $e->getMessage());
来源：http://wu.nszjky.cn

[U73] PHP：读取 ini 配置
来源：http://vd.colortex.cn

parse_ini_file("config.ini", true)
来源：http://hm.yuexingan06.cn

[U74] PHP：读取环境变量
来源：http://td.yuntaijiaju.cn

getenv("APP_ENV") ?: "production"
来源：http://bg.haigaiapp.cn

[U75] PHP：依赖注入
来源：http://ua.hnjuh.cn

composer require psr/container
来源：http://rb.gzmigu.cn

[U76] PHP：简单路由
来源：http://cn.colortex.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://jy.yuexingan06.cn

[U77] PHP：模板渲染
来源：http://ry.asd995.cn

composer require twig/twig
来源：http://tb.bookmarksfly.cn

[U78] PHP：单元测试
来源：http://zp.gzmigu.cn

composer require --dev phpunit/phpunit
来源：http://ct.gzmigu.cn

[U79] PHP：静态分析
来源：http://on.jianghongdianzi.cn

composer require --dev phpstan/phpstan
来源：http://cs.huixiangedu.cn

[U80] PHP：代码规范修复
来源：http://ad.yuntaijiaju.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://lc.shxzskj.cn

[U81] JS：初始化项目
来源：http://mk.chemitech.net.cn

npm init -y;  npm i express
来源：http://mx.shxzukj.cn

[U82] JS：package.json 脚本
来源：http://rc.newstarts.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://cm.asd995.cn

[U83] JS：ES Module 导入导出
来源：http://gx.colortex.cn

export const a = 1;  import { a } from "./m.js";
来源：http://oe.haigaiapp.cn

[U84] JS：CommonJS 写法
来源：http://do.colortex.cn

module.exports = { a };  const { a } = require("./m");
来源：http://eu.521024.cn

[U85] JS：可选链
来源：http://rc.bookmarksfly.cn

a?.b?.c
来源：http://sa.9csxet.cn

[U86] JS：空值合并
来源：http://ja.hahajie.cn

a ?? b
来源：http://lt.huixinmuqiang.cn

[U87] JS：解构默认值
来源：http://cs.hahajie.cn

const { a = 1, b = 2 } = obj;
来源：http://bi.huanxung.cn

[U88] JS：对象展开合并
来源：http://pd.colortex.cn

{ ...a, ...b }
来源：http://ry.asd995.cn

[U89] JS：数组去重
来源：http://aw.jianghongdianzi.cn

[...new Set(arr)]
来源：http://rw.bookmarksfly.cn

[U90] JS：数字数组排序
来源：http://df.huixiangedu.cn

[...arr].sort((a, b) => a - b)
来源：http://ch.shxzukj.cn

[U91] JS：对象键值遍历
来源：http://dz.hnjuh.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://id.hahajie.cn

[U92] JS：深拷贝
来源：http://tc.newstarts.cn

structuredClone(obj)
来源：http://hl.gzmigu.cn

[U93] JS：模板字符串
来源：http://zk.jianghongdianzi.cn

`共 ${n} 条`
来源：http://oc.szsharing.cn

[U94] JS：箭头函数
来源：http://op.huixinmuqiang.cn

const double = x => x * 2;
来源：http://jx.szsharing.cn

[U95] JS：Promise 包装
来源：http://ob.521024.cn

new Promise((resolve, reject) => {})
来源：http://bv.lnxyls.cn

[U96] JS：async/await 与异常
来源：http://by.yuexingan06.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://te.wgjwhj.cn

[U97] JS：并发请求
来源：http://ks.lnxyls.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://af.szsharing.cn

[U98] JS：fetch 带 JSON
来源：http://ge.hahajie.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://st.muxihuayi.cn

[U99] JS：事件监听
来源：http://th.haigaiapp.cn

el.addEventListener("click", e => {})
来源：http://di.lnxyls.cn

[U100] JS：DOM 查询
来源：http://ff.asd995.cn

document.querySelector(".item")
来源：http://tq.bjjhwx.cn

[U101] JS：classList 操作
来源：http://gj.muxihuayi.cn

el.classList.toggle("active")
来源：http://bj.bookmarksfly.cn

[U102] JS：本地存储
来源：http://lv.chemitech.net.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://kt.huanxung.cn

[U103] JS：定时器
来源：http://jg.newstarts.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://aa.huixiangedu.cn

[U104] JS：防抖
来源：http://kc.wgjwhj.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cp.nicolike.cn

[U105] JS：节流
来源：http://xz.shxzskj.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://oc.bookmarksfly.cn

[U106] JS：日期格式化
来源：http://ov.9csxet.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://lp.panjiajie.cn

[U107] JS：数字千分位
来源：http://tu.jctech888.com.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://po.chemitech.net.cn

[U108] JS：随机整数
来源：http://oz.asd995.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://cm.bookmarksfly.cn

[U109] JS：数组分组
来源：http://gy.huixiangedu.cn

Object.groupBy(arr, x => x.type)
来源：http://uc.9csxet.cn

[U110] JS：数组分块
来源：http://zb.lnxyls.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://fh.yuntaijiaju.cn

[U111] JS：对象转 Map
来源：http://zs.hnjuh.cn

new Map(Object.entries(obj))
来源：http://tx.shxzskj.cn

[U112] JS：字符串补位
来源：http://as.nszjky.cn

"7".padStart(3, "0")
来源：http://hy.521024.cn

[U113] JS：正则替换全部
来源：http://cd.chemitech.net.cn

s.replaceAll("a", "b")
来源：http://fn.hahajie.cn

[U114] JS：JSON 深比较
来源：http://fm.jianghongdianzi.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://xv.nicolike.cn

[U115] JS：生成 UUID
来源：http://gk.nicolike.cn

crypto.randomUUID()
来源：http://ct.lnxyls.cn

[U116] JS：类型检查（JSDoc）
来源：http://pq.nicolike.cn

/** @param {string} name */ function f(name) {}
来源：http://kq.9csxet.cn

[U117] JS：单元测试
来源：http://ja.jianghongdianzi.cn

npm i -D vitest;  npx vitest
来源：http://ot.muxihuayi.cn

[U118] JS：开发服务器
来源：http://fr.9csxet.cn

npm i -D vite;  npx vite
来源：http://ll.huixinmuqiang.cn

[U119] JS：生产构建
来源：http://cp.9csxet.cn

npx vite build
来源：http://ed.wgjwhj.cn

[U120] JS：读取环境变量（Vite）
来源：http://oc.colortex.cn

import.meta.env.VITE_API_URL
来源：http://nn.panjiajie.cn

================================================================================
来源：http://da.jianghongdianzi.cn

统计汇总
来源：http://kc.yuexingan06.cn

================================================================================
来源：http://gd.bjjhwx.cn

按语言统计（条）：
来源：http://bt.521024.cn

Python ......... 252
来源：http://fb.hahajie.cn

PHP ............ 252
来源：http://lf.wgjwhj.cn

JavaScript ..... 252
来源：http://wv.wgjwhj.cn

TypeScript ..... 212
来源：http://rv.shtwfgs.cn

Java ........... 212
来源：http://lm.shxzskj.cn

Go ............. 212
来源：http://zi.huanxung.cn

Ruby ........... 212
来源：http://ax.szsharing.cn

C# ............. 212
来源：http://xq.szsharing.cn

C .............. 30
来源：http://qv.huixiangedu.cn

C++ ............ 30
来源：http://cv.haigaiapp.cn

SQL ............ 90
来源：http://gn.bjjhwx.cn

Bash ........... 80
来源：http://ee.bjjhwx.cn

Kotlin ......... 15
来源：http://aw.bjjhwx.cn

Swift .......... 15
来源：http://cq.panjiajie.cn

Lua ............ 10
来源：http://ag.hahajie.cn

Perl ........... 10
来源：http://qc.muxihuayi.cn

Scala .......... 10
来源：http://fx.521024.cn

------------------------------------
来源：http://nm.haigaiapp.cn

合计 ........... 2106 条
来源：http://ls.jctech888.com.cn

按章节统计：
来源：http://dh.521024.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://gr.521024.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://tq.szxytkj.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mi.haigaiapp.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ns.haigaiapp.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://qs.huixinmuqiang.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://dj.chemitech.net.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ew.newstarts.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://od.9csxet.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://qk.huixiangedu.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://kp.yuexingan06.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mr.lnxyls.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://le.nicolike.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://zy.jianghongdianzi.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://he.9csxet.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://rl.panjiajie.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ho.wgjwhj.cn

Q SQL 专题                              90
来源：http://gx.9csxet.cn

R Bash 专题                             80
来源：http://wh.shxzskj.cn

S C / C++ 专题                          60
来源：http://ww.szsharing.cn

T 其他语言补充                          60
来源：http://yj.haigaiapp.cn

U 高频实用片段                         120
来源：http://nu.lnxyls.cn

------------------------------------
来源：http://no.colortex.cn

合计                                  2106 条
来源：http://vb.haigaiapp.cn

--------------------------------------------------------------------------------
来源：http://kp.bookmarksfly.cn

使用提醒
来源：http://yi.jianghongdianzi.cn

--------------------------------------------------------------------------------
来源：http://cu.lnxyls.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://rf.yuntaijiaju.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ai.lnxyls.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://db.nicolike.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://kx.shxzskj.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wl.szsharing.cn

—— 文件结束 ——
来源：http://fn.yuexingan06.cn

================================================================================
来源：http://sh.shxzskj.cn

程序语言常见例子速查手册（2024 版）
来源：http://ud.gzmigu.cn

Common Programming Examples Cheat Book
来源：http://wj.gzmigu.cn

================================================================================
来源：http://aw.szsharing.cn

【收录内容】
来源：http://go.yuntaijiaju.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://bl.shxzskj.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://nq.asd995.cn

SQL · Bash · C · C++
来源：http://cx.muxihuayi.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://sd.hahajie.cn

【使用说明】
来源：http://vw.jctech888.com.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://pr.lnxyls.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ju.gzmigu.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://al.shxzskj.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://uc.bjjhwx.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://ys.huixiangedu.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ht.hahajie.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://vh.shtwfgs.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://wr.szxytkj.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ur.jianghongdianzi.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://zm.jianghongdianzi.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://bi.shxzukj.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://yp.jctech888.com.cn

【文件统计】
来源：http://ry.lnxyls.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://kf.gzmigu.cn

--------------------------------------------------------------------------------
来源：http://zx.shtwfgs.cn

目  录
来源：http://io.nicolike.cn

--------------------------------------------------------------------------------
来源：http://to.wgjwhj.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://wv.shxzukj.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://qu.wgjwhj.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://jz.szxytkj.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://rt.newstarts.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://zj.panjiajie.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://lb.wgjwhj.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://cx.521024.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://vj.huixiangedu.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ad.jianghongdianzi.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://aa.chemitech.net.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://sc.newstarts.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hd.huixinmuqiang.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://qg.9csxet.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://iy.shtwfgs.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://fu.shxzskj.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://wg.newstarts.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://cy.huixiangedu.cn


<!-- 参考信息 -->