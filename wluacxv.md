代发 wailian999

[U15] Py：高精度计时
来源：http://km.huanxung.cn

t = time.perf_counter()
来源：http://bf.panjiajie.cn

[U16] Py：命令行参数解析
来源：http://kx.shxzskj.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wm.haigaiapp.cn

[U17] Py：初始化日志
来源：http://ol.muxihuayi.cn

logging.basicConfig(level=logging.INFO)
来源：http://zi.asd995.cn

[U18] Py：预编译正则
来源：http://gu.9csxet.cn

pat = re.compile(r"\d+")
来源：http://bv.521024.cn

[U19] Py：正则替换带回调
来源：http://pv.huixiangedu.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ns.hahajie.cn

[U20] Py：缓存函数结果
来源：http://hn.shtwfgs.cn

@functools.lru_cache(maxsize=None)
来源：http://ul.bookmarksfly.cn

[U21] Py：自定义上下文管理器
来源：http://tb.huixiangedu.cn

@contextlib.contextmanager
来源：http://mf.panjiajie.cn

[U22] Py：矩阵转置
来源：http://zz.chemitech.net.cn

list(zip(*m))
来源：http://va.szxytkj.cn

[U23] Py：分块读取大文件
来源：http://cg.bookmarksfly.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://tn.muxihuayi.cn

[U24] Py：路径操作
来源：http://ug.hnjuh.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://qi.newstarts.cn

[U25] Py：CSV 按字典读
来源：http://ij.szsharing.cn

csv.DictReader(f)
来源：http://vf.yuexingan06.cn

[U26] Py：并发下载
来源：http://mx.szxytkj.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://zr.asd995.cn

[U27] Py：异步 HTTP
来源：http://qo.hahajie.cn

aiohttp.ClientSession() 配合 async with
来源：http://hh.chemitech.net.cn

[U28] Py：类型别名
来源：http://rr.yuexingan06.cn

UserId = int
来源：http://yd.hahajie.cn

[U29] Py：属性校验
来源：http://xy.hahajie.cn

@property 与 @x.setter 配合
来源：http://bu.521024.cn

[U30] Py：数据类
来源：http://ks.wgjwhj.cn

@dataclass(slots=True)
来源：http://mq.gzmigu.cn

[U31] Py：单测
来源：http://gp.gzmigu.cn

python -m pytest -q
来源：http://io.wgjwhj.cn

[U32] Py：代码格式化
来源：http://zt.521024.cn

ruff format . && ruff check --fix .
来源：http://yo.bjjhwx.cn

[U33] Py：打包发布
来源：http://ah.chemitech.net.cn

python -m build  （依赖 pyproject.toml）
来源：http://vs.huanxung.cn

[U34] Py：判断编码
来源：http://eq.jctech888.com.cn

chardet.detect(raw)
来源：http://bj.haigaiapp.cn

[U35] Py：发送邮件
来源：http://ye.521024.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://tc.yuexingan06.cn

[U36] Py：定时任务
来源：http://fj.gzmigu.cn

schedule.every(10).minutes.do(job)
来源：http://js.wgjwhj.cn

[U37] Py：读写 Excel
来源：http://cu.asd995.cn

pandas.read_excel / DataFrame.to_excel
来源：http://rq.asd995.cn

[U38] Py：获取脚本所在目录
来源：http://bt.haigaiapp.cn

Path(__file__).resolve().parent
来源：http://ae.huixinmuqiang.cn

[U39] Py：判断是否在交互环境
来源：http://cz.nicolike.cn

sys.stdout.isatty()
来源：http://og.szsharing.cn

[U40] Py：打印到标准错误
来源：http://iu.colortex.cn

print("err", file=sys.stderr)
来源：http://fc.9csxet.cn

[U41] PHP：初始化 Composer 项目
来源：http://od.muxihuayi.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://ph.huixinmuqiang.cn

[U42] PHP：PSR-4 自动加载
来源：http://zl.521024.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://jo.muxihuayi.cn

[U43] PHP：声明命名空间
来源：http://sf.huixiangedu.cn

namespace App\Http;
来源：http://lx.bjjhwx.cn

[U44] PHP：开启严格类型
来源：http://ak.haigaiapp.cn

declare(strict_types=1);
来源：http://ud.asd995.cn

[U45] PHP：类型声明与返回类型
来源：http://ej.asd995.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://ed.shtwfgs.cn

[U46] PHP：可空类型
来源：http://dc.jianghongdianzi.cn

?string $name = null
来源：http://sa.szxytkj.cn

[U47] PHP：联合类型
来源：http://zn.shtwfgs.cn

int|string $id
来源：http://kp.hahajie.cn

[U48] PHP：纯枚举
来源：http://nj.wgjwhj.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://qd.newstarts.cn

[U49] PHP：只读属性
来源：http://rt.chemitech.net.cn

public readonly string $name
来源：http://sx.hnjuh.cn

[U50] PHP：构造器属性提升
来源：http://lf.nszjky.cn

public function __construct(private int $id) {}
来源：http://wj.lnxyls.cn

[U51] PHP：数组解构
来源：http://od.chemitech.net.cn

[$a, $b] = $arr;
来源：http://ce.yuntaijiaju.cn

[U52] PHP：箭头函数
来源：http://zf.521024.cn

$double = fn($x) => $x * 2;
来源：http://wi.yuexingan06.cn

[U53] PHP：空合并运算符
来源：http://ye.hahajie.cn

$v = $a ?? $b ?? "default";
来源：http://ii.yuntaijiaju.cn

[U54] PHP：空安全调用
来源：http://fx.haigaiapp.cn

$obj?->method()
来源：http://nw.asd995.cn

[U55] PHP：match 表达式
来源：http://ty.jianghongdianzi.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://qe.jianghongdianzi.cn

[U56] PHP：命名参数
来源：http://ad.nszjky.cn

f(a: 1, b: 2)
来源：http://lx.gzmigu.cn

[U57] PHP：字符串插值
来源：http://xv.jctech888.com.cn

"值: {$a}"
来源：http://xp.hnjuh.cn

[U58] PHP：数组三件套
来源：http://ug.szxytkj.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ui.asd995.cn

[U59] PHP：自定义排序
来源：http://jo.nicolike.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ek.gzmigu.cn

[U60] PHP：JSON 编解码
来源：http://ix.shxzukj.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://jr.shxzukj.cn

[U61] PHP：正则
来源：http://ys.521024.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://jm.shtwfgs.cn

[U62] PHP：日期对象
来源：http://pk.colortex.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://bw.huixinmuqiang.cn

[U63] PHP：文件读写
来源：http://ow.huixinmuqiang.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://jj.jianghongdianzi.cn

[U64] PHP：目录遍历
来源：http://tc.shxzukj.cn

glob("dir/*.php");  scandir("dir");
来源：http://qk.bjjhwx.cn

[U65] PHP：会话
来源：http://tk.chemitech.net.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://pu.szxytkj.cn

[U66] PHP：设置 Cookie
来源：http://gv.9csxet.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://cf.newstarts.cn

[U67] PHP：处理文件上传
来源：http://ee.hahajie.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://vy.haigaiapp.cn

[U68] PHP：PDO 连接
来源：http://sh.asd995.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://pl.gzmigu.cn

[U69] PHP：PDO 预处理
来源：http://pg.hnjuh.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ia.bjjhwx.cn

[U70] PHP：PDO 事务
来源：http://hf.shtwfgs.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://oo.shxzskj.cn

[U71] PHP：抛出异常
来源：http://pm.shtwfgs.cn

throw new RuntimeException("失败", 500);
来源：http://ci.shxzukj.cn

[U72] PHP：写错误日志
来源：http://po.nicolike.cn

error_log("失败: " . $e->getMessage());
来源：http://gm.huanxung.cn

[U73] PHP：读取 ini 配置
来源：http://jl.yuexingan06.cn

parse_ini_file("config.ini", true)
来源：http://gp.jctech888.com.cn

[U74] PHP：读取环境变量
来源：http://tg.jctech888.com.cn

getenv("APP_ENV") ?: "production"
来源：http://to.gzmigu.cn

[U75] PHP：依赖注入
来源：http://yw.muxihuayi.cn

composer require psr/container
来源：http://fl.huixiangedu.cn

[U76] PHP：简单路由
来源：http://ps.yuntaijiaju.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://jb.shxzukj.cn

[U77] PHP：模板渲染
来源：http://fv.jctech888.com.cn

composer require twig/twig
来源：http://ur.szxytkj.cn

[U78] PHP：单元测试
来源：http://nb.huixiangedu.cn

composer require --dev phpunit/phpunit
来源：http://oz.nszjky.cn

[U79] PHP：静态分析
来源：http://ja.huixinmuqiang.cn

composer require --dev phpstan/phpstan
来源：http://ht.yuexingan06.cn

[U80] PHP：代码规范修复
来源：http://ml.nicolike.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://vk.huixiangedu.cn

[U81] JS：初始化项目
来源：http://kk.colortex.cn

npm init -y;  npm i express
来源：http://mx.colortex.cn

[U82] JS：package.json 脚本
来源：http://pn.szxytkj.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hq.lnxyls.cn

[U83] JS：ES Module 导入导出
来源：http://lo.huixinmuqiang.cn

export const a = 1;  import { a } from "./m.js";
来源：http://vr.szsharing.cn

[U84] JS：CommonJS 写法
来源：http://en.bookmarksfly.cn

module.exports = { a };  const { a } = require("./m");
来源：http://cf.huixinmuqiang.cn

[U85] JS：可选链
来源：http://jp.chemitech.net.cn

a?.b?.c
来源：http://eu.colortex.cn

[U86] JS：空值合并
来源：http://ky.colortex.cn

a ?? b
来源：http://ru.gzmigu.cn

[U87] JS：解构默认值
来源：http://ga.huixiangedu.cn

const { a = 1, b = 2 } = obj;
来源：http://za.hahajie.cn

[U88] JS：对象展开合并
来源：http://fq.jianghongdianzi.cn

{ ...a, ...b }
来源：http://xc.shxzskj.cn

[U89] JS：数组去重
来源：http://ib.jianghongdianzi.cn

[...new Set(arr)]
来源：http://iw.asd995.cn

[U90] JS：数字数组排序
来源：http://mg.huixiangedu.cn

[...arr].sort((a, b) => a - b)
来源：http://yu.jianghongdianzi.cn

[U91] JS：对象键值遍历
来源：http://nj.szsharing.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://cn.nszjky.cn

[U92] JS：深拷贝
来源：http://qy.haigaiapp.cn

structuredClone(obj)
来源：http://bg.shxzukj.cn

[U93] JS：模板字符串
来源：http://ue.yuntaijiaju.cn

`共 ${n} 条`
来源：http://gu.gzmigu.cn

[U94] JS：箭头函数
来源：http://tr.hahajie.cn

const double = x => x * 2;
来源：http://gp.521024.cn

[U95] JS：Promise 包装
来源：http://uv.colortex.cn

new Promise((resolve, reject) => {})
来源：http://ct.yuntaijiaju.cn

[U96] JS：async/await 与异常
来源：http://ry.nicolike.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://kg.yuexingan06.cn

[U97] JS：并发请求
来源：http://tk.521024.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://vv.haigaiapp.cn

[U98] JS：fetch 带 JSON
来源：http://ly.szxytkj.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://tt.huanxung.cn

[U99] JS：事件监听
来源：http://ym.lnxyls.cn

el.addEventListener("click", e => {})
来源：http://vw.colortex.cn

[U100] JS：DOM 查询
来源：http://hy.huixinmuqiang.cn

document.querySelector(".item")
来源：http://jz.huixinmuqiang.cn

[U101] JS：classList 操作
来源：http://gc.huanxung.cn

el.classList.toggle("active")
来源：http://vc.chemitech.net.cn

[U102] JS：本地存储
来源：http://xy.wgjwhj.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://hd.nicolike.cn

[U103] JS：定时器
来源：http://kl.chemitech.net.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://lt.asd995.cn

[U104] JS：防抖
来源：http://ne.huixiangedu.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vb.521024.cn

[U105] JS：节流
来源：http://ut.nicolike.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://pe.newstarts.cn

[U106] JS：日期格式化
来源：http://bt.shxzskj.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://na.szsharing.cn

[U107] JS：数字千分位
来源：http://fo.asd995.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://kp.shxzskj.cn

[U108] JS：随机整数
来源：http://kx.521024.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ps.shtwfgs.cn

[U109] JS：数组分组
来源：http://yy.muxihuayi.cn

Object.groupBy(arr, x => x.type)
来源：http://rr.shtwfgs.cn

[U110] JS：数组分块
来源：http://td.huixiangedu.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ty.panjiajie.cn

[U111] JS：对象转 Map
来源：http://bb.haigaiapp.cn

new Map(Object.entries(obj))
来源：http://gv.colortex.cn

[U112] JS：字符串补位
来源：http://dm.nicolike.cn

"7".padStart(3, "0")
来源：http://py.521024.cn

[U113] JS：正则替换全部
来源：http://yw.panjiajie.cn

s.replaceAll("a", "b")
来源：http://xv.hnjuh.cn

[U114] JS：JSON 深比较
来源：http://oz.521024.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://yh.jianghongdianzi.cn

[U115] JS：生成 UUID
来源：http://uh.yuexingan06.cn

crypto.randomUUID()
来源：http://jy.jctech888.com.cn

[U116] JS：类型检查（JSDoc）
来源：http://as.hnjuh.cn

/** @param {string} name */ function f(name) {}
来源：http://pm.chemitech.net.cn

[U117] JS：单元测试
来源：http://zl.bookmarksfly.cn

npm i -D vitest;  npx vitest
来源：http://dq.521024.cn

[U118] JS：开发服务器
来源：http://ju.yuntaijiaju.cn

npm i -D vite;  npx vite
来源：http://nr.asd995.cn

[U119] JS：生产构建
来源：http://zh.bookmarksfly.cn

npx vite build
来源：http://ob.wgjwhj.cn

[U120] JS：读取环境变量（Vite）
来源：http://kp.haigaiapp.cn

import.meta.env.VITE_API_URL
来源：http://hd.huixiangedu.cn

================================================================================
来源：http://xv.asd995.cn

统计汇总
来源：http://jj.shtwfgs.cn

================================================================================
来源：http://nv.jianghongdianzi.cn

按语言统计（条）：
来源：http://yi.jctech888.com.cn

Python ......... 252
来源：http://ko.newstarts.cn

PHP ............ 252
来源：http://bf.newstarts.cn

JavaScript ..... 252
来源：http://uh.jianghongdianzi.cn

TypeScript ..... 212
来源：http://ve.newstarts.cn

Java ........... 212
来源：http://nc.hahajie.cn

Go ............. 212
来源：http://gx.shxzskj.cn

Ruby ........... 212
来源：http://rs.huixiangedu.cn

C# ............. 212
来源：http://la.yuexingan06.cn

C .............. 30
来源：http://id.huixiangedu.cn

C++ ............ 30
来源：http://pt.9csxet.cn

SQL ............ 90
来源：http://gt.gzmigu.cn

Bash ........... 80
来源：http://ec.gzmigu.cn

Kotlin ......... 15
来源：http://jt.muxihuayi.cn

Swift .......... 15
来源：http://ya.yuexingan06.cn

Lua ............ 10
来源：http://gs.nszjky.cn

Perl ........... 10
来源：http://ux.hahajie.cn

Scala .......... 10
来源：http://bv.wgjwhj.cn

------------------------------------
来源：http://up.yuntaijiaju.cn

合计 ........... 2106 条
来源：http://ka.huixinmuqiang.cn

按章节统计：
来源：http://yx.newstarts.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://oj.szxytkj.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ui.hahajie.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hj.shxzukj.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wx.huixinmuqiang.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://al.9csxet.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://go.nicolike.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://bw.yuexingan06.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://kj.yuntaijiaju.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://eo.nszjky.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ig.huixinmuqiang.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://dv.hnjuh.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://dk.nszjky.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ci.shxzukj.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://qs.colortex.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://pt.hahajie.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://st.shxzskj.cn

Q SQL 专题                              90
来源：http://st.jianghongdianzi.cn

R Bash 专题                             80
来源：http://hx.yuexingan06.cn

S C / C++ 专题                          60
来源：http://hn.521024.cn

T 其他语言补充                          60
来源：http://uy.huixiangedu.cn

U 高频实用片段                         120
来源：http://os.shxzskj.cn

------------------------------------
来源：http://gq.gzmigu.cn

合计                                  2106 条
来源：http://da.nicolike.cn

--------------------------------------------------------------------------------
来源：http://xp.9csxet.cn

使用提醒
来源：http://ag.521024.cn

--------------------------------------------------------------------------------
来源：http://uq.gzmigu.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://kh.muxihuayi.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://al.bjjhwx.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ha.huixinmuqiang.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://iw.colortex.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://bo.bookmarksfly.cn

—— 文件结束 ——
来源：http://ew.newstarts.cn

================================================================================
来源：http://fr.hnjuh.cn

程序语言常见例子速查手册（2024 版）
来源：http://pb.asd995.cn

Common Programming Examples Cheat Book
来源：http://wr.panjiajie.cn

================================================================================
来源：http://iw.yuntaijiaju.cn

【收录内容】
来源：http://df.shxzukj.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://ac.jianghongdianzi.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://cr.bookmarksfly.cn

SQL · Bash · C · C++
来源：http://ip.huixinmuqiang.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://oo.hahajie.cn

【使用说明】
来源：http://kd.wgjwhj.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hp.shtwfgs.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://fy.wgjwhj.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hs.shxzukj.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://wd.chemitech.net.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://hv.huanxung.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ps.yuexingan06.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ih.gzmigu.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://af.shxzskj.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://wa.yuexingan06.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://fn.nicolike.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ny.bjjhwx.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://uy.newstarts.cn

【文件统计】
来源：http://gh.szsharing.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://kj.shxzukj.cn

--------------------------------------------------------------------------------
来源：http://wm.bookmarksfly.cn

目  录
来源：http://hr.yuntaijiaju.cn

--------------------------------------------------------------------------------
来源：http://db.lnxyls.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://lb.huanxung.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://xf.bjjhwx.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://va.szsharing.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://tc.hnjuh.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://xr.muxihuayi.cn


<!-- 参考信息 -->