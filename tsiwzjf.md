代发 wailian999

[U17] Py：初始化日志
来源：http://ht.521024.cn

logging.basicConfig(level=logging.INFO)
来源：http://ez.szsharing.cn

[U18] Py：预编译正则
来源：http://kj.yuexingan06.cn

pat = re.compile(r"\d+")
来源：http://ih.bookmarksfly.cn

[U19] Py：正则替换带回调
来源：http://rb.gzmigu.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ps.huixinmuqiang.cn

[U20] Py：缓存函数结果
来源：http://ar.newstarts.cn

@functools.lru_cache(maxsize=None)
来源：http://oi.panjiajie.cn

[U21] Py：自定义上下文管理器
来源：http://ip.lnxyls.cn

@contextlib.contextmanager
来源：http://jk.jctech888.com.cn

[U22] Py：矩阵转置
来源：http://wx.haigaiapp.cn

list(zip(*m))
来源：http://iz.shtwfgs.cn

[U23] Py：分块读取大文件
来源：http://ir.bookmarksfly.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wi.colortex.cn

[U24] Py：路径操作
来源：http://ae.asd995.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ax.bookmarksfly.cn

[U25] Py：CSV 按字典读
来源：http://lv.jianghongdianzi.cn

csv.DictReader(f)
来源：http://eh.yuexingan06.cn

[U26] Py：并发下载
来源：http://pa.hnjuh.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ck.yuntaijiaju.cn

[U27] Py：异步 HTTP
来源：http://hd.bookmarksfly.cn

aiohttp.ClientSession() 配合 async with
来源：http://nu.bjjhwx.cn

[U28] Py：类型别名
来源：http://ed.yuexingan06.cn

UserId = int
来源：http://lt.haigaiapp.cn

[U29] Py：属性校验
来源：http://hb.gzmigu.cn

@property 与 @x.setter 配合
来源：http://rb.bjjhwx.cn

[U30] Py：数据类
来源：http://iv.521024.cn

@dataclass(slots=True)
来源：http://pm.muxihuayi.cn

[U31] Py：单测
来源：http://us.yuntaijiaju.cn

python -m pytest -q
来源：http://et.szsharing.cn

[U32] Py：代码格式化
来源：http://gj.szxytkj.cn

ruff format . && ruff check --fix .
来源：http://or.huixinmuqiang.cn

[U33] Py：打包发布
来源：http://bw.lnxyls.cn

python -m build  （依赖 pyproject.toml）
来源：http://dr.chemitech.net.cn

[U34] Py：判断编码
来源：http://el.bookmarksfly.cn

chardet.detect(raw)
来源：http://jr.chemitech.net.cn

[U35] Py：发送邮件
来源：http://cz.shtwfgs.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ra.shtwfgs.cn

[U36] Py：定时任务
来源：http://kc.colortex.cn

schedule.every(10).minutes.do(job)
来源：http://pg.lnxyls.cn

[U37] Py：读写 Excel
来源：http://mo.hahajie.cn

pandas.read_excel / DataFrame.to_excel
来源：http://ni.panjiajie.cn

[U38] Py：获取脚本所在目录
来源：http://ha.chemitech.net.cn

Path(__file__).resolve().parent
来源：http://rv.hnjuh.cn

[U39] Py：判断是否在交互环境
来源：http://kl.newstarts.cn

sys.stdout.isatty()
来源：http://hn.gzmigu.cn

[U40] Py：打印到标准错误
来源：http://vr.bjjhwx.cn

print("err", file=sys.stderr)
来源：http://sr.nszjky.cn

[U41] PHP：初始化 Composer 项目
来源：http://pw.gzmigu.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://mh.bjjhwx.cn

[U42] PHP：PSR-4 自动加载
来源：http://ko.panjiajie.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hl.yuntaijiaju.cn

[U43] PHP：声明命名空间
来源：http://ih.521024.cn

namespace App\Http;
来源：http://wg.nszjky.cn

[U44] PHP：开启严格类型
来源：http://ik.huixinmuqiang.cn

declare(strict_types=1);
来源：http://kk.huixiangedu.cn

[U45] PHP：类型声明与返回类型
来源：http://zi.chemitech.net.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://jo.bookmarksfly.cn

[U46] PHP：可空类型
来源：http://bx.nicolike.cn

?string $name = null
来源：http://xj.9csxet.cn

[U47] PHP：联合类型
来源：http://yu.panjiajie.cn

int|string $id
来源：http://pk.newstarts.cn

[U48] PHP：纯枚举
来源：http://gn.huanxung.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://qr.nicolike.cn

[U49] PHP：只读属性
来源：http://jp.lnxyls.cn

public readonly string $name
来源：http://pn.yuntaijiaju.cn

[U50] PHP：构造器属性提升
来源：http://bg.9csxet.cn

public function __construct(private int $id) {}
来源：http://nm.szsharing.cn

[U51] PHP：数组解构
来源：http://tl.bookmarksfly.cn

[$a, $b] = $arr;
来源：http://ss.panjiajie.cn

[U52] PHP：箭头函数
来源：http://ka.newstarts.cn

$double = fn($x) => $x * 2;
来源：http://fk.huanxung.cn

[U53] PHP：空合并运算符
来源：http://aj.haigaiapp.cn

$v = $a ?? $b ?? "default";
来源：http://lw.shtwfgs.cn

[U54] PHP：空安全调用
来源：http://rr.szsharing.cn

$obj?->method()
来源：http://ek.muxihuayi.cn

[U55] PHP：match 表达式
来源：http://xr.yuexingan06.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://uu.9csxet.cn

[U56] PHP：命名参数
来源：http://gd.chemitech.net.cn

f(a: 1, b: 2)
来源：http://rt.panjiajie.cn

[U57] PHP：字符串插值
来源：http://de.jctech888.com.cn

"值: {$a}"
来源：http://bg.wgjwhj.cn

[U58] PHP：数组三件套
来源：http://kw.colortex.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://um.newstarts.cn

[U59] PHP：自定义排序
来源：http://to.521024.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://rr.jianghongdianzi.cn

[U60] PHP：JSON 编解码
来源：http://dz.jianghongdianzi.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mv.bookmarksfly.cn

[U61] PHP：正则
来源：http://ko.jianghongdianzi.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://nq.colortex.cn

[U62] PHP：日期对象
来源：http://rw.nszjky.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://pl.nszjky.cn

[U63] PHP：文件读写
来源：http://nr.shxzskj.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ki.huixinmuqiang.cn

[U64] PHP：目录遍历
来源：http://fg.asd995.cn

glob("dir/*.php");  scandir("dir");
来源：http://ch.yuntaijiaju.cn

[U65] PHP：会话
来源：http://ce.jianghongdianzi.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://bv.jianghongdianzi.cn

[U66] PHP：设置 Cookie
来源：http://jc.chemitech.net.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://pr.haigaiapp.cn

[U67] PHP：处理文件上传
来源：http://hg.yuntaijiaju.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://zd.shxzskj.cn

[U68] PHP：PDO 连接
来源：http://mr.wgjwhj.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://pm.bookmarksfly.cn

[U69] PHP：PDO 预处理
来源：http://oi.hnjuh.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ux.chemitech.net.cn

[U70] PHP：PDO 事务
来源：http://nh.huixiangedu.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wh.lnxyls.cn

[U71] PHP：抛出异常
来源：http://ne.asd995.cn

throw new RuntimeException("失败", 500);
来源：http://mm.huixiangedu.cn

[U72] PHP：写错误日志
来源：http://ps.9csxet.cn

error_log("失败: " . $e->getMessage());
来源：http://bb.hahajie.cn

[U73] PHP：读取 ini 配置
来源：http://yo.nszjky.cn

parse_ini_file("config.ini", true)
来源：http://pu.szsharing.cn

[U74] PHP：读取环境变量
来源：http://lu.szxytkj.cn

getenv("APP_ENV") ?: "production"
来源：http://ya.bookmarksfly.cn

[U75] PHP：依赖注入
来源：http://gr.yuntaijiaju.cn

composer require psr/container
来源：http://wn.panjiajie.cn

[U76] PHP：简单路由
来源：http://pj.panjiajie.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://fn.huanxung.cn

[U77] PHP：模板渲染
来源：http://uu.haigaiapp.cn

composer require twig/twig
来源：http://fv.shxzskj.cn

[U78] PHP：单元测试
来源：http://gs.huixinmuqiang.cn

composer require --dev phpunit/phpunit
来源：http://cv.gzmigu.cn

[U79] PHP：静态分析
来源：http://nl.shxzskj.cn

composer require --dev phpstan/phpstan
来源：http://kq.asd995.cn

[U80] PHP：代码规范修复
来源：http://gl.jianghongdianzi.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://cb.hnjuh.cn

[U81] JS：初始化项目
来源：http://we.huanxung.cn

npm init -y;  npm i express
来源：http://lc.lnxyls.cn

[U82] JS：package.json 脚本
来源：http://lb.colortex.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://jf.muxihuayi.cn

[U83] JS：ES Module 导入导出
来源：http://cr.jctech888.com.cn

export const a = 1;  import { a } from "./m.js";
来源：http://zg.jianghongdianzi.cn

[U84] JS：CommonJS 写法
来源：http://bs.521024.cn

module.exports = { a };  const { a } = require("./m");
来源：http://xd.bookmarksfly.cn

[U85] JS：可选链
来源：http://bu.shxzskj.cn

a?.b?.c
来源：http://co.asd995.cn

[U86] JS：空值合并
来源：http://jh.huixiangedu.cn

a ?? b
来源：http://rh.bjjhwx.cn

[U87] JS：解构默认值
来源：http://br.hahajie.cn

const { a = 1, b = 2 } = obj;
来源：http://ka.bjjhwx.cn

[U88] JS：对象展开合并
来源：http://ps.huixinmuqiang.cn

{ ...a, ...b }
来源：http://nq.nicolike.cn

[U89] JS：数组去重
来源：http://iy.shtwfgs.cn

[...new Set(arr)]
来源：http://xp.gzmigu.cn

[U90] JS：数字数组排序
来源：http://kf.yuntaijiaju.cn

[...arr].sort((a, b) => a - b)
来源：http://ko.szxytkj.cn

[U91] JS：对象键值遍历
来源：http://gj.asd995.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://fo.shxzukj.cn

[U92] JS：深拷贝
来源：http://fw.yuntaijiaju.cn

structuredClone(obj)
来源：http://rh.szsharing.cn

[U93] JS：模板字符串
来源：http://sy.lnxyls.cn

`共 ${n} 条`
来源：http://ib.nicolike.cn

[U94] JS：箭头函数
来源：http://lh.huixinmuqiang.cn

const double = x => x * 2;
来源：http://cb.9csxet.cn

[U95] JS：Promise 包装
来源：http://kl.szsharing.cn

new Promise((resolve, reject) => {})
来源：http://gz.panjiajie.cn

[U96] JS：async/await 与异常
来源：http://cf.huanxung.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://cr.yuexingan06.cn

[U97] JS：并发请求
来源：http://dp.gzmigu.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://ij.colortex.cn

[U98] JS：fetch 带 JSON
来源：http://wz.asd995.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://qn.colortex.cn

[U99] JS：事件监听
来源：http://xq.szxytkj.cn

el.addEventListener("click", e => {})
来源：http://pz.newstarts.cn

[U100] JS：DOM 查询
来源：http://uj.shtwfgs.cn

document.querySelector(".item")
来源：http://ju.yuexingan06.cn

[U101] JS：classList 操作
来源：http://cp.newstarts.cn

el.classList.toggle("active")
来源：http://fs.wgjwhj.cn

[U102] JS：本地存储
来源：http://yu.bjjhwx.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://rf.newstarts.cn

[U103] JS：定时器
来源：http://vu.shtwfgs.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ng.shxzukj.cn

[U104] JS：防抖
来源：http://lx.panjiajie.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qv.jctech888.com.cn

[U105] JS：节流
来源：http://cj.panjiajie.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://rh.jctech888.com.cn

[U106] JS：日期格式化
来源：http://cn.shxzukj.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://yv.wgjwhj.cn

[U107] JS：数字千分位
来源：http://gm.yuntaijiaju.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://zm.nszjky.cn

[U108] JS：随机整数
来源：http://kd.9csxet.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://xw.asd995.cn

[U109] JS：数组分组
来源：http://cp.nicolike.cn

Object.groupBy(arr, x => x.type)
来源：http://bo.huixinmuqiang.cn

[U110] JS：数组分块
来源：http://ve.colortex.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://tm.newstarts.cn

[U111] JS：对象转 Map
来源：http://ly.panjiajie.cn

new Map(Object.entries(obj))
来源：http://rc.shxzukj.cn

[U112] JS：字符串补位
来源：http://vb.muxihuayi.cn

"7".padStart(3, "0")
来源：http://ze.huixiangedu.cn

[U113] JS：正则替换全部
来源：http://tc.szsharing.cn

s.replaceAll("a", "b")
来源：http://wc.hnjuh.cn

[U114] JS：JSON 深比较
来源：http://te.shxzukj.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://dc.bookmarksfly.cn

[U115] JS：生成 UUID
来源：http://dp.asd995.cn

crypto.randomUUID()
来源：http://da.shxzskj.cn

[U116] JS：类型检查（JSDoc）
来源：http://ae.jianghongdianzi.cn

/** @param {string} name */ function f(name) {}
来源：http://gk.szsharing.cn

[U117] JS：单元测试
来源：http://su.shxzskj.cn

npm i -D vitest;  npx vitest
来源：http://vp.newstarts.cn

[U118] JS：开发服务器
来源：http://zz.colortex.cn

npm i -D vite;  npx vite
来源：http://zc.shxzukj.cn

[U119] JS：生产构建
来源：http://lt.lnxyls.cn

npx vite build
来源：http://pp.jctech888.com.cn

[U120] JS：读取环境变量（Vite）
来源：http://wt.shxzskj.cn

import.meta.env.VITE_API_URL
来源：http://ru.bookmarksfly.cn

================================================================================
来源：http://ek.muxihuayi.cn

统计汇总
来源：http://hi.shxzskj.cn

================================================================================
来源：http://hf.haigaiapp.cn

按语言统计（条）：
来源：http://gb.colortex.cn

Python ......... 252
来源：http://wy.szsharing.cn

PHP ............ 252
来源：http://jn.jctech888.com.cn

JavaScript ..... 252
来源：http://lb.szsharing.cn

TypeScript ..... 212
来源：http://hz.panjiajie.cn

Java ........... 212
来源：http://rw.shxzskj.cn

Go ............. 212
来源：http://ew.jianghongdianzi.cn

Ruby ........... 212
来源：http://vc.9csxet.cn

C# ............. 212
来源：http://ko.chemitech.net.cn

C .............. 30
来源：http://wf.gzmigu.cn

C++ ............ 30
来源：http://ql.huixiangedu.cn

SQL ............ 90
来源：http://vc.hnjuh.cn

Bash ........... 80
来源：http://bs.bjjhwx.cn

Kotlin ......... 15
来源：http://ak.huanxung.cn

Swift .......... 15
来源：http://uw.szsharing.cn

Lua ............ 10
来源：http://gs.shxzskj.cn

Perl ........... 10
来源：http://rz.jianghongdianzi.cn

Scala .......... 10
来源：http://xc.lnxyls.cn

------------------------------------
来源：http://xw.newstarts.cn

合计 ........... 2106 条
来源：http://so.panjiajie.cn

按章节统计：
来源：http://ee.gzmigu.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://fq.yuexingan06.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ny.szxytkj.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://yn.lnxyls.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://yb.asd995.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://fd.haigaiapp.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://nz.huixiangedu.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://um.nicolike.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mh.shxzukj.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://si.szsharing.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://nw.hahajie.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wy.yuntaijiaju.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://my.yuntaijiaju.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://yt.521024.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://yj.shtwfgs.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://gj.huanxung.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://na.panjiajie.cn

Q SQL 专题                              90
来源：http://nk.lnxyls.cn

R Bash 专题                             80
来源：http://fa.521024.cn

S C / C++ 专题                          60
来源：http://hn.nicolike.cn

T 其他语言补充                          60
来源：http://xl.shxzskj.cn

U 高频实用片段                         120
来源：http://qm.9csxet.cn

------------------------------------
来源：http://ig.gzmigu.cn

合计                                  2106 条
来源：http://pl.huixiangedu.cn

--------------------------------------------------------------------------------
来源：http://aw.newstarts.cn

使用提醒
来源：http://sn.hnjuh.cn

--------------------------------------------------------------------------------
来源：http://sh.jianghongdianzi.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://rn.hnjuh.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://vc.yuexingan06.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ew.huixinmuqiang.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://ks.wgjwhj.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://cn.panjiajie.cn

—— 文件结束 ——
来源：http://os.hnjuh.cn

================================================================================
来源：http://rj.shtwfgs.cn

程序语言常见例子速查手册（2024 版）
来源：http://rm.chemitech.net.cn

Common Programming Examples Cheat Book
来源：http://er.muxihuayi.cn

================================================================================
来源：http://zc.panjiajie.cn

【收录内容】
来源：http://up.521024.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://uh.huixinmuqiang.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://re.nszjky.cn

SQL · Bash · C · C++
来源：http://nv.asd995.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://gf.huanxung.cn

【使用说明】
来源：http://xv.newstarts.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://cj.nszjky.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hg.521024.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://yd.yuntaijiaju.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://mb.nszjky.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://vm.colortex.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wn.yuexingan06.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://xv.jianghongdianzi.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://wn.muxihuayi.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ic.yuntaijiaju.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://tm.bookmarksfly.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://xn.lnxyls.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://tj.asd995.cn

【文件统计】
来源：http://wb.yuexingan06.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://fz.gzmigu.cn

--------------------------------------------------------------------------------
来源：http://te.shxzukj.cn

目  录
来源：http://cu.521024.cn

--------------------------------------------------------------------------------
来源：http://gc.hahajie.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://xc.wgjwhj.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ln.hahajie.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://rg.chemitech.net.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://rc.szxytkj.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://eu.chemitech.net.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://ms.haigaiapp.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://yq.bjjhwx.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://zu.hnjuh.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ua.hahajie.cn


<!-- 参考信息 -->