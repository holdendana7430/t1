代发 wailian999

[U15] Py：高精度计时
来源：http://dp.szxytkj.cn

t = time.perf_counter()
来源：http://pn.shtwfgs.cn

[U16] Py：命令行参数解析
来源：http://de.newstarts.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ml.yuexingan06.cn

[U17] Py：初始化日志
来源：http://jq.szsharing.cn

logging.basicConfig(level=logging.INFO)
来源：http://ot.gzmigu.cn

[U18] Py：预编译正则
来源：http://an.asd995.cn

pat = re.compile(r"\d+")
来源：http://iv.wgjwhj.cn

[U19] Py：正则替换带回调
来源：http://lx.gzmigu.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://cd.yuexingan06.cn

[U20] Py：缓存函数结果
来源：http://hm.nszjky.cn

@functools.lru_cache(maxsize=None)
来源：http://sz.lnxyls.cn

[U21] Py：自定义上下文管理器
来源：http://ql.yuexingan06.cn

@contextlib.contextmanager
来源：http://wb.panjiajie.cn

[U22] Py：矩阵转置
来源：http://ry.wgjwhj.cn

list(zip(*m))
来源：http://rs.szxytkj.cn

[U23] Py：分块读取大文件
来源：http://cw.asd995.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://sn.gzmigu.cn

[U24] Py：路径操作
来源：http://vj.chemitech.net.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ib.nszjky.cn

[U25] Py：CSV 按字典读
来源：http://fg.muxihuayi.cn

csv.DictReader(f)
来源：http://na.szsharing.cn

[U26] Py：并发下载
来源：http://rm.huixinmuqiang.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ax.bjjhwx.cn

[U27] Py：异步 HTTP
来源：http://zl.panjiajie.cn

aiohttp.ClientSession() 配合 async with
来源：http://mm.shxzskj.cn

[U28] Py：类型别名
来源：http://ui.bookmarksfly.cn

UserId = int
来源：http://ld.bookmarksfly.cn

[U29] Py：属性校验
来源：http://it.huixinmuqiang.cn

@property 与 @x.setter 配合
来源：http://nu.newstarts.cn

[U30] Py：数据类
来源：http://cj.colortex.cn

@dataclass(slots=True)
来源：http://sd.nszjky.cn

[U31] Py：单测
来源：http://ha.nicolike.cn

python -m pytest -q
来源：http://vd.colortex.cn

[U32] Py：代码格式化
来源：http://ye.szsharing.cn

ruff format . && ruff check --fix .
来源：http://ae.shxzskj.cn

[U33] Py：打包发布
来源：http://dv.jianghongdianzi.cn

python -m build  （依赖 pyproject.toml）
来源：http://ie.yuntaijiaju.cn

[U34] Py：判断编码
来源：http://cy.chemitech.net.cn

chardet.detect(raw)
来源：http://nm.lnxyls.cn

[U35] Py：发送邮件
来源：http://wn.colortex.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ge.wgjwhj.cn

[U36] Py：定时任务
来源：http://mv.newstarts.cn

schedule.every(10).minutes.do(job)
来源：http://du.nicolike.cn

[U37] Py：读写 Excel
来源：http://in.hahajie.cn

pandas.read_excel / DataFrame.to_excel
来源：http://he.hnjuh.cn

[U38] Py：获取脚本所在目录
来源：http://yz.hnjuh.cn

Path(__file__).resolve().parent
来源：http://wp.nszjky.cn

[U39] Py：判断是否在交互环境
来源：http://cy.wgjwhj.cn

sys.stdout.isatty()
来源：http://md.huixinmuqiang.cn

[U40] Py：打印到标准错误
来源：http://az.huixinmuqiang.cn

print("err", file=sys.stderr)
来源：http://ed.nicolike.cn

[U41] PHP：初始化 Composer 项目
来源：http://ts.haigaiapp.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://ci.9csxet.cn

[U42] PHP：PSR-4 自动加载
来源：http://cr.9csxet.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://za.521024.cn

[U43] PHP：声明命名空间
来源：http://yk.shxzukj.cn

namespace App\Http;
来源：http://ez.bookmarksfly.cn

[U44] PHP：开启严格类型
来源：http://dc.bookmarksfly.cn

declare(strict_types=1);
来源：http://hn.shxzskj.cn

[U45] PHP：类型声明与返回类型
来源：http://ng.hnjuh.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://os.yuexingan06.cn

[U46] PHP：可空类型
来源：http://bs.szxytkj.cn

?string $name = null
来源：http://nr.hahajie.cn

[U47] PHP：联合类型
来源：http://cx.huanxung.cn

int|string $id
来源：http://qi.huanxung.cn

[U48] PHP：纯枚举
来源：http://zt.szsharing.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://kf.nicolike.cn

[U49] PHP：只读属性
来源：http://eb.haigaiapp.cn

public readonly string $name
来源：http://wa.wgjwhj.cn

[U50] PHP：构造器属性提升
来源：http://df.yuntaijiaju.cn

public function __construct(private int $id) {}
来源：http://mt.panjiajie.cn

[U51] PHP：数组解构
来源：http://oz.gzmigu.cn

[$a, $b] = $arr;
来源：http://cl.9csxet.cn

[U52] PHP：箭头函数
来源：http://zb.nszjky.cn

$double = fn($x) => $x * 2;
来源：http://ig.bjjhwx.cn

[U53] PHP：空合并运算符
来源：http://am.gzmigu.cn

$v = $a ?? $b ?? "default";
来源：http://bm.huixinmuqiang.cn

[U54] PHP：空安全调用
来源：http://tz.huixiangedu.cn

$obj?->method()
来源：http://ff.szxytkj.cn

[U55] PHP：match 表达式
来源：http://ug.jianghongdianzi.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://aa.nszjky.cn

[U56] PHP：命名参数
来源：http://ya.panjiajie.cn

f(a: 1, b: 2)
来源：http://sv.gzmigu.cn

[U57] PHP：字符串插值
来源：http://dg.haigaiapp.cn

"值: {$a}"
来源：http://hm.bjjhwx.cn

[U58] PHP：数组三件套
来源：http://re.colortex.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://gp.szxytkj.cn

[U59] PHP：自定义排序
来源：http://ho.colortex.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ls.hnjuh.cn

[U60] PHP：JSON 编解码
来源：http://mm.hahajie.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://sv.hahajie.cn

[U61] PHP：正则
来源：http://vu.lnxyls.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mc.yuexingan06.cn

[U62] PHP：日期对象
来源：http://tb.bookmarksfly.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wm.hnjuh.cn

[U63] PHP：文件读写
来源：http://ff.colortex.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://fh.muxihuayi.cn

[U64] PHP：目录遍历
来源：http://uk.nicolike.cn

glob("dir/*.php");  scandir("dir");
来源：http://go.asd995.cn

[U65] PHP：会话
来源：http://pm.huanxung.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://wj.lnxyls.cn

[U66] PHP：设置 Cookie
来源：http://ko.hnjuh.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ak.panjiajie.cn

[U67] PHP：处理文件上传
来源：http://vp.huixinmuqiang.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://cp.huanxung.cn

[U68] PHP：PDO 连接
来源：http://ml.hahajie.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://uf.panjiajie.cn

[U69] PHP：PDO 预处理
来源：http://rc.yuexingan06.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://gr.9csxet.cn

[U70] PHP：PDO 事务
来源：http://ex.huixinmuqiang.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://sc.hahajie.cn

[U71] PHP：抛出异常
来源：http://wj.wgjwhj.cn

throw new RuntimeException("失败", 500);
来源：http://hq.wgjwhj.cn

[U72] PHP：写错误日志
来源：http://gy.hnjuh.cn

error_log("失败: " . $e->getMessage());
来源：http://om.jctech888.com.cn

[U73] PHP：读取 ini 配置
来源：http://xa.gzmigu.cn

parse_ini_file("config.ini", true)
来源：http://qk.shtwfgs.cn

[U74] PHP：读取环境变量
来源：http://ly.huanxung.cn

getenv("APP_ENV") ?: "production"
来源：http://vs.chemitech.net.cn

[U75] PHP：依赖注入
来源：http://pf.yuntaijiaju.cn

composer require psr/container
来源：http://tz.nicolike.cn

[U76] PHP：简单路由
来源：http://ah.521024.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://qz.gzmigu.cn

[U77] PHP：模板渲染
来源：http://jo.wgjwhj.cn

composer require twig/twig
来源：http://qb.shxzskj.cn

[U78] PHP：单元测试
来源：http://yw.asd995.cn

composer require --dev phpunit/phpunit
来源：http://se.bjjhwx.cn

[U79] PHP：静态分析
来源：http://ia.jctech888.com.cn

composer require --dev phpstan/phpstan
来源：http://gs.huanxung.cn

[U80] PHP：代码规范修复
来源：http://sq.lnxyls.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://yh.huixiangedu.cn

[U81] JS：初始化项目
来源：http://rc.bookmarksfly.cn

npm init -y;  npm i express
来源：http://cw.521024.cn

[U82] JS：package.json 脚本
来源：http://cy.huanxung.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://kx.jctech888.com.cn

[U83] JS：ES Module 导入导出
来源：http://da.9csxet.cn

export const a = 1;  import { a } from "./m.js";
来源：http://bi.panjiajie.cn

[U84] JS：CommonJS 写法
来源：http://wj.huixinmuqiang.cn

module.exports = { a };  const { a } = require("./m");
来源：http://ox.asd995.cn

[U85] JS：可选链
来源：http://gk.yuexingan06.cn

a?.b?.c
来源：http://gp.szsharing.cn

[U86] JS：空值合并
来源：http://ta.huanxung.cn

a ?? b
来源：http://qk.huixiangedu.cn

[U87] JS：解构默认值
来源：http://ud.nicolike.cn

const { a = 1, b = 2 } = obj;
来源：http://yr.gzmigu.cn

[U88] JS：对象展开合并
来源：http://tx.yuexingan06.cn

{ ...a, ...b }
来源：http://rw.huixinmuqiang.cn

[U89] JS：数组去重
来源：http://wy.asd995.cn

[...new Set(arr)]
来源：http://lx.szxytkj.cn

[U90] JS：数字数组排序
来源：http://sb.hahajie.cn

[...arr].sort((a, b) => a - b)
来源：http://kz.huixinmuqiang.cn

[U91] JS：对象键值遍历
来源：http://ha.colortex.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://oz.shtwfgs.cn

[U92] JS：深拷贝
来源：http://zr.newstarts.cn

structuredClone(obj)
来源：http://vn.muxihuayi.cn

[U93] JS：模板字符串
来源：http://bq.nicolike.cn

`共 ${n} 条`
来源：http://cj.asd995.cn

[U94] JS：箭头函数
来源：http://ua.jianghongdianzi.cn

const double = x => x * 2;
来源：http://qr.huixiangedu.cn

[U95] JS：Promise 包装
来源：http://ey.huixinmuqiang.cn

new Promise((resolve, reject) => {})
来源：http://kz.lnxyls.cn

[U96] JS：async/await 与异常
来源：http://od.muxihuayi.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wo.huanxung.cn

[U97] JS：并发请求
来源：http://nq.jianghongdianzi.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://ae.nszjky.cn

[U98] JS：fetch 带 JSON
来源：http://kb.chemitech.net.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ys.lnxyls.cn

[U99] JS：事件监听
来源：http://tx.jianghongdianzi.cn

el.addEventListener("click", e => {})
来源：http://oy.huixiangedu.cn

[U100] JS：DOM 查询
来源：http://tf.chemitech.net.cn

document.querySelector(".item")
来源：http://ow.szxytkj.cn

[U101] JS：classList 操作
来源：http://nl.haigaiapp.cn

el.classList.toggle("active")
来源：http://gi.jianghongdianzi.cn

[U102] JS：本地存储
来源：http://ny.jctech888.com.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://qt.chemitech.net.cn

[U103] JS：定时器
来源：http://xh.bookmarksfly.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://nh.yuexingan06.cn

[U104] JS：防抖
来源：http://rf.wgjwhj.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pm.nicolike.cn

[U105] JS：节流
来源：http://kg.shxzukj.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://bk.bookmarksfly.cn

[U106] JS：日期格式化
来源：http://on.huanxung.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://vo.jianghongdianzi.cn

[U107] JS：数字千分位
来源：http://kn.bjjhwx.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mu.wgjwhj.cn

[U108] JS：随机整数
来源：http://ig.huanxung.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://sz.bjjhwx.cn

[U109] JS：数组分组
来源：http://vd.szsharing.cn

Object.groupBy(arr, x => x.type)
来源：http://je.9csxet.cn

[U110] JS：数组分块
来源：http://aq.shxzskj.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://og.hnjuh.cn

[U111] JS：对象转 Map
来源：http://oz.colortex.cn

new Map(Object.entries(obj))
来源：http://lg.panjiajie.cn

[U112] JS：字符串补位
来源：http://rq.nicolike.cn

"7".padStart(3, "0")
来源：http://sm.haigaiapp.cn

[U113] JS：正则替换全部
来源：http://ri.shxzskj.cn

s.replaceAll("a", "b")
来源：http://jg.yuexingan06.cn

[U114] JS：JSON 深比较
来源：http://vo.yuexingan06.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://qv.muxihuayi.cn

[U115] JS：生成 UUID
来源：http://bt.szxytkj.cn

crypto.randomUUID()
来源：http://ld.gzmigu.cn

[U116] JS：类型检查（JSDoc）
来源：http://ro.colortex.cn

/** @param {string} name */ function f(name) {}
来源：http://qw.jianghongdianzi.cn

[U117] JS：单元测试
来源：http://af.bjjhwx.cn

npm i -D vitest;  npx vitest
来源：http://jg.gzmigu.cn

[U118] JS：开发服务器
来源：http://be.521024.cn

npm i -D vite;  npx vite
来源：http://de.asd995.cn

[U119] JS：生产构建
来源：http://pv.bookmarksfly.cn

npx vite build
来源：http://yr.bookmarksfly.cn

[U120] JS：读取环境变量（Vite）
来源：http://wl.newstarts.cn

import.meta.env.VITE_API_URL
来源：http://tn.gzmigu.cn

================================================================================
来源：http://ir.bookmarksfly.cn

统计汇总
来源：http://ii.hahajie.cn

================================================================================
来源：http://rm.yuexingan06.cn

按语言统计（条）：
来源：http://iz.muxihuayi.cn

Python ......... 252
来源：http://as.wgjwhj.cn

PHP ............ 252
来源：http://na.szsharing.cn

JavaScript ..... 252
来源：http://bi.nszjky.cn

TypeScript ..... 212
来源：http://up.newstarts.cn

Java ........... 212
来源：http://if.nszjky.cn

Go ............. 212
来源：http://lp.szxytkj.cn

Ruby ........... 212
来源：http://yw.huanxung.cn

C# ............. 212
来源：http://yf.panjiajie.cn

C .............. 30
来源：http://hj.nszjky.cn

C++ ............ 30
来源：http://dw.lnxyls.cn

SQL ............ 90
来源：http://bn.nicolike.cn

Bash ........... 80
来源：http://gl.jianghongdianzi.cn

Kotlin ......... 15
来源：http://ul.haigaiapp.cn

Swift .......... 15
来源：http://if.muxihuayi.cn

Lua ............ 10
来源：http://ma.lnxyls.cn

Perl ........... 10
来源：http://ki.colortex.cn

Scala .......... 10
来源：http://ly.shtwfgs.cn

------------------------------------
来源：http://bb.colortex.cn

合计 ........... 2106 条
来源：http://jl.hnjuh.cn

按章节统计：
来源：http://ey.chemitech.net.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://oo.bjjhwx.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://be.asd995.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://cf.hahajie.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://zv.huanxung.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://fu.chemitech.net.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://pq.jctech888.com.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://dm.hahajie.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ru.huixinmuqiang.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://yq.huixinmuqiang.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://iv.jianghongdianzi.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://lw.huixinmuqiang.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://gf.yuntaijiaju.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://xj.newstarts.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://jm.wgjwhj.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ez.bookmarksfly.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://cc.huixiangedu.cn

Q SQL 专题                              90
来源：http://nq.colortex.cn

R Bash 专题                             80
来源：http://jx.newstarts.cn

S C / C++ 专题                          60
来源：http://hb.9csxet.cn

T 其他语言补充                          60
来源：http://vn.panjiajie.cn

U 高频实用片段                         120
来源：http://nk.jianghongdianzi.cn

------------------------------------
来源：http://nc.bookmarksfly.cn

合计                                  2106 条
来源：http://mu.colortex.cn

--------------------------------------------------------------------------------
来源：http://rc.huixinmuqiang.cn

使用提醒
来源：http://fq.szsharing.cn

--------------------------------------------------------------------------------
来源：http://ck.nszjky.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://sl.szsharing.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://fu.haigaiapp.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://xa.huixiangedu.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://fx.huanxung.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://la.hnjuh.cn

—— 文件结束 ——
来源：http://gs.gzmigu.cn

================================================================================
来源：http://fk.yuexingan06.cn

程序语言常见例子速查手册（2024 版）
来源：http://so.nszjky.cn

Common Programming Examples Cheat Book
来源：http://ca.asd995.cn

================================================================================
来源：http://rj.haigaiapp.cn

【收录内容】
来源：http://de.hnjuh.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://um.hnjuh.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://zo.szxytkj.cn

SQL · Bash · C · C++
来源：http://hp.yuntaijiaju.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://mr.huixinmuqiang.cn

【使用说明】
来源：http://op.shxzskj.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://do.muxihuayi.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://zd.shxzukj.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://dg.hahajie.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://re.gzmigu.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://wm.shxzskj.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://rm.9csxet.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://gw.nicolike.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://gn.nicolike.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://yi.lnxyls.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://te.haigaiapp.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://sd.9csxet.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://yk.lnxyls.cn

【文件统计】
来源：http://wh.szsharing.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ro.szsharing.cn

--------------------------------------------------------------------------------
来源：http://xu.asd995.cn

目  录
来源：http://yf.shtwfgs.cn

--------------------------------------------------------------------------------
来源：http://kz.huanxung.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://zj.jianghongdianzi.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://uv.jianghongdianzi.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://is.yuexingan06.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ww.huanxung.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://jv.huanxung.cn


<!-- 参考信息 -->