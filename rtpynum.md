代发 wailian999

[U15] Py：高精度计时
来源：http://mp.muxihuayi.cn

t = time.perf_counter()
来源：http://as.nszjky.cn

[U16] Py：命令行参数解析
来源：http://aa.nszjky.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wp.nicolike.cn

[U17] Py：初始化日志
来源：http://ve.bookmarksfly.cn

logging.basicConfig(level=logging.INFO)
来源：http://wz.bookmarksfly.cn

[U18] Py：预编译正则
来源：http://as.nicolike.cn

pat = re.compile(r"\d+")
来源：http://th.jctech888.com.cn

[U19] Py：正则替换带回调
来源：http://rd.yuexingan06.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://rw.panjiajie.cn

[U20] Py：缓存函数结果
来源：http://re.szxytkj.cn

@functools.lru_cache(maxsize=None)
来源：http://qh.muxihuayi.cn

[U21] Py：自定义上下文管理器
来源：http://xq.521024.cn

@contextlib.contextmanager
来源：http://um.huixiangedu.cn

[U22] Py：矩阵转置
来源：http://zh.haigaiapp.cn

list(zip(*m))
来源：http://ck.yuntaijiaju.cn

[U23] Py：分块读取大文件
来源：http://ev.yuntaijiaju.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://dr.chemitech.net.cn

[U24] Py：路径操作
来源：http://ls.yuexingan06.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://kv.9csxet.cn

[U25] Py：CSV 按字典读
来源：http://mq.lnxyls.cn

csv.DictReader(f)
来源：http://ij.shtwfgs.cn

[U26] Py：并发下载
来源：http://cq.yuntaijiaju.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://lg.newstarts.cn

[U27] Py：异步 HTTP
来源：http://ih.panjiajie.cn

aiohttp.ClientSession() 配合 async with
来源：http://ux.yuexingan06.cn

[U28] Py：类型别名
来源：http://kj.haigaiapp.cn

UserId = int
来源：http://jb.colortex.cn

[U29] Py：属性校验
来源：http://yf.nszjky.cn

@property 与 @x.setter 配合
来源：http://mb.bjjhwx.cn

[U30] Py：数据类
来源：http://pb.newstarts.cn

@dataclass(slots=True)
来源：http://cf.shxzukj.cn

[U31] Py：单测
来源：http://gh.shxzukj.cn

python -m pytest -q
来源：http://pn.jctech888.com.cn

[U32] Py：代码格式化
来源：http://zd.shtwfgs.cn

ruff format . && ruff check --fix .
来源：http://ta.lnxyls.cn

[U33] Py：打包发布
来源：http://oa.shxzskj.cn

python -m build  （依赖 pyproject.toml）
来源：http://aj.hahajie.cn

[U34] Py：判断编码
来源：http://gc.haigaiapp.cn

chardet.detect(raw)
来源：http://yg.nszjky.cn

[U35] Py：发送邮件
来源：http://vt.panjiajie.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://fk.hnjuh.cn

[U36] Py：定时任务
来源：http://wv.hahajie.cn

schedule.every(10).minutes.do(job)
来源：http://av.bookmarksfly.cn

[U37] Py：读写 Excel
来源：http://ar.yuntaijiaju.cn

pandas.read_excel / DataFrame.to_excel
来源：http://li.szsharing.cn

[U38] Py：获取脚本所在目录
来源：http://xg.newstarts.cn

Path(__file__).resolve().parent
来源：http://js.wgjwhj.cn

[U39] Py：判断是否在交互环境
来源：http://nu.jianghongdianzi.cn

sys.stdout.isatty()
来源：http://jg.bjjhwx.cn

[U40] Py：打印到标准错误
来源：http://hx.shtwfgs.cn

print("err", file=sys.stderr)
来源：http://kk.hahajie.cn

[U41] PHP：初始化 Composer 项目
来源：http://ar.yuntaijiaju.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://oq.muxihuayi.cn

[U42] PHP：PSR-4 自动加载
来源：http://jf.panjiajie.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://nk.bookmarksfly.cn

[U43] PHP：声明命名空间
来源：http://cr.yuntaijiaju.cn

namespace App\Http;
来源：http://sv.asd995.cn

[U44] PHP：开启严格类型
来源：http://uw.colortex.cn

declare(strict_types=1);
来源：http://mu.shxzskj.cn

[U45] PHP：类型声明与返回类型
来源：http://di.haigaiapp.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://ym.shtwfgs.cn

[U46] PHP：可空类型
来源：http://sw.gzmigu.cn

?string $name = null
来源：http://fu.bjjhwx.cn

[U47] PHP：联合类型
来源：http://oe.bjjhwx.cn

int|string $id
来源：http://lg.colortex.cn

[U48] PHP：纯枚举
来源：http://rm.bookmarksfly.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://bw.521024.cn

[U49] PHP：只读属性
来源：http://vc.bookmarksfly.cn

public readonly string $name
来源：http://de.shxzukj.cn

[U50] PHP：构造器属性提升
来源：http://kx.huanxung.cn

public function __construct(private int $id) {}
来源：http://um.huanxung.cn

[U51] PHP：数组解构
来源：http://ni.yuexingan06.cn

[$a, $b] = $arr;
来源：http://mt.huixiangedu.cn

[U52] PHP：箭头函数
来源：http://ty.hnjuh.cn

$double = fn($x) => $x * 2;
来源：http://ie.yuntaijiaju.cn

[U53] PHP：空合并运算符
来源：http://bv.gzmigu.cn

$v = $a ?? $b ?? "default";
来源：http://wz.asd995.cn

[U54] PHP：空安全调用
来源：http://tk.9csxet.cn

$obj?->method()
来源：http://yh.huixinmuqiang.cn

[U55] PHP：match 表达式
来源：http://qv.jctech888.com.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://if.huixinmuqiang.cn

[U56] PHP：命名参数
来源：http://xe.huixinmuqiang.cn

f(a: 1, b: 2)
来源：http://vj.bookmarksfly.cn

[U57] PHP：字符串插值
来源：http://of.muxihuayi.cn

"值: {$a}"
来源：http://bw.hahajie.cn

[U58] PHP：数组三件套
来源：http://bm.yuexingan06.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://aw.wgjwhj.cn

[U59] PHP：自定义排序
来源：http://ls.jianghongdianzi.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ug.hnjuh.cn

[U60] PHP：JSON 编解码
来源：http://vw.chemitech.net.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://nw.wgjwhj.cn

[U61] PHP：正则
来源：http://ya.yuntaijiaju.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ij.shxzskj.cn

[U62] PHP：日期对象
来源：http://oo.yuexingan06.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://lt.lnxyls.cn

[U63] PHP：文件读写
来源：http://dp.9csxet.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://fi.muxihuayi.cn

[U64] PHP：目录遍历
来源：http://go.chemitech.net.cn

glob("dir/*.php");  scandir("dir");
来源：http://jj.haigaiapp.cn

[U65] PHP：会话
来源：http://gl.nszjky.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://ri.colortex.cn

[U66] PHP：设置 Cookie
来源：http://cu.chemitech.net.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://uk.wgjwhj.cn

[U67] PHP：处理文件上传
来源：http://er.9csxet.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://cm.bookmarksfly.cn

[U68] PHP：PDO 连接
来源：http://iq.szxytkj.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://re.shtwfgs.cn

[U69] PHP：PDO 预处理
来源：http://vg.yuntaijiaju.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ib.shxzskj.cn

[U70] PHP：PDO 事务
来源：http://cx.9csxet.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://zd.bookmarksfly.cn

[U71] PHP：抛出异常
来源：http://fb.chemitech.net.cn

throw new RuntimeException("失败", 500);
来源：http://hk.shxzskj.cn

[U72] PHP：写错误日志
来源：http://ih.asd995.cn

error_log("失败: " . $e->getMessage());
来源：http://cw.shxzskj.cn

[U73] PHP：读取 ini 配置
来源：http://cq.jianghongdianzi.cn

parse_ini_file("config.ini", true)
来源：http://fs.colortex.cn

[U74] PHP：读取环境变量
来源：http://az.jctech888.com.cn

getenv("APP_ENV") ?: "production"
来源：http://tq.shtwfgs.cn

[U75] PHP：依赖注入
来源：http://tn.huixiangedu.cn

composer require psr/container
来源：http://dd.lnxyls.cn

[U76] PHP：简单路由
来源：http://ac.huixinmuqiang.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://gf.szxytkj.cn

[U77] PHP：模板渲染
来源：http://cq.nszjky.cn

composer require twig/twig
来源：http://ft.colortex.cn

[U78] PHP：单元测试
来源：http://pz.huixinmuqiang.cn

composer require --dev phpunit/phpunit
来源：http://kg.huanxung.cn

[U79] PHP：静态分析
来源：http://sn.yuexingan06.cn

composer require --dev phpstan/phpstan
来源：http://jl.shtwfgs.cn

[U80] PHP：代码规范修复
来源：http://gm.haigaiapp.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://wh.shxzukj.cn

[U81] JS：初始化项目
来源：http://qd.szxytkj.cn

npm init -y;  npm i express
来源：http://pv.bookmarksfly.cn

[U82] JS：package.json 脚本
来源：http://xa.nszjky.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://pf.szxytkj.cn

[U83] JS：ES Module 导入导出
来源：http://ex.panjiajie.cn

export const a = 1;  import { a } from "./m.js";
来源：http://hg.muxihuayi.cn

[U84] JS：CommonJS 写法
来源：http://zn.lnxyls.cn

module.exports = { a };  const { a } = require("./m");
来源：http://xo.bjjhwx.cn

[U85] JS：可选链
来源：http://um.yuntaijiaju.cn

a?.b?.c
来源：http://kt.muxihuayi.cn

[U86] JS：空值合并
来源：http://up.lnxyls.cn

a ?? b
来源：http://tf.szsharing.cn

[U87] JS：解构默认值
来源：http://jv.bookmarksfly.cn

const { a = 1, b = 2 } = obj;
来源：http://hg.521024.cn

[U88] JS：对象展开合并
来源：http://cb.gzmigu.cn

{ ...a, ...b }
来源：http://zf.huixinmuqiang.cn

[U89] JS：数组去重
来源：http://rc.chemitech.net.cn

[...new Set(arr)]
来源：http://wc.hahajie.cn

[U90] JS：数字数组排序
来源：http://xm.shxzukj.cn

[...arr].sort((a, b) => a - b)
来源：http://kk.shxzukj.cn

[U91] JS：对象键值遍历
来源：http://ig.9csxet.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://nt.jianghongdianzi.cn

[U92] JS：深拷贝
来源：http://ki.jctech888.com.cn

structuredClone(obj)
来源：http://we.lnxyls.cn

[U93] JS：模板字符串
来源：http://jn.newstarts.cn

`共 ${n} 条`
来源：http://ls.bjjhwx.cn

[U94] JS：箭头函数
来源：http://et.huanxung.cn

const double = x => x * 2;
来源：http://zc.shxzukj.cn

[U95] JS：Promise 包装
来源：http://pw.jianghongdianzi.cn

new Promise((resolve, reject) => {})
来源：http://fi.521024.cn

[U96] JS：async/await 与异常
来源：http://uz.lnxyls.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wy.nicolike.cn

[U97] JS：并发请求
来源：http://de.521024.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://lh.bookmarksfly.cn

[U98] JS：fetch 带 JSON
来源：http://av.shtwfgs.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://fj.newstarts.cn

[U99] JS：事件监听
来源：http://yk.shtwfgs.cn

el.addEventListener("click", e => {})
来源：http://nk.chemitech.net.cn

[U100] JS：DOM 查询
来源：http://gm.jianghongdianzi.cn

document.querySelector(".item")
来源：http://jb.gzmigu.cn

[U101] JS：classList 操作
来源：http://oe.asd995.cn

el.classList.toggle("active")
来源：http://sj.nszjky.cn

[U102] JS：本地存储
来源：http://nn.bjjhwx.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://bo.nicolike.cn

[U103] JS：定时器
来源：http://ja.shxzukj.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ja.shxzukj.cn

[U104] JS：防抖
来源：http://dy.huixiangedu.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://uu.colortex.cn

[U105] JS：节流
来源：http://au.shtwfgs.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://jm.lnxyls.cn

[U106] JS：日期格式化
来源：http://fj.yuntaijiaju.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://zg.haigaiapp.cn

[U107] JS：数字千分位
来源：http://dw.jctech888.com.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://sk.szxytkj.cn

[U108] JS：随机整数
来源：http://gx.hnjuh.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://dq.hahajie.cn

[U109] JS：数组分组
来源：http://ub.gzmigu.cn

Object.groupBy(arr, x => x.type)
来源：http://sm.wgjwhj.cn

[U110] JS：数组分块
来源：http://vc.gzmigu.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://dt.shtwfgs.cn

[U111] JS：对象转 Map
来源：http://jx.lnxyls.cn

new Map(Object.entries(obj))
来源：http://vs.colortex.cn

[U112] JS：字符串补位
来源：http://ta.wgjwhj.cn

"7".padStart(3, "0")
来源：http://wx.colortex.cn

[U113] JS：正则替换全部
来源：http://mn.szsharing.cn

s.replaceAll("a", "b")
来源：http://bk.newstarts.cn

[U114] JS：JSON 深比较
来源：http://hs.shxzukj.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://yw.bookmarksfly.cn

[U115] JS：生成 UUID
来源：http://zp.nszjky.cn

crypto.randomUUID()
来源：http://rv.huanxung.cn

[U116] JS：类型检查（JSDoc）
来源：http://pq.shxzukj.cn

/** @param {string} name */ function f(name) {}
来源：http://mg.521024.cn

[U117] JS：单元测试
来源：http://za.huixiangedu.cn

npm i -D vitest;  npx vitest
来源：http://ko.yuntaijiaju.cn

[U118] JS：开发服务器
来源：http://ki.huixiangedu.cn

npm i -D vite;  npx vite
来源：http://tp.panjiajie.cn

[U119] JS：生产构建
来源：http://ca.hnjuh.cn

npx vite build
来源：http://rf.jctech888.com.cn

[U120] JS：读取环境变量（Vite）
来源：http://we.yuexingan06.cn

import.meta.env.VITE_API_URL
来源：http://st.shxzukj.cn

================================================================================
来源：http://fx.bookmarksfly.cn

统计汇总
来源：http://du.yuexingan06.cn

================================================================================
来源：http://bl.gzmigu.cn

按语言统计（条）：
来源：http://vm.gzmigu.cn

Python ......... 252
来源：http://zg.nszjky.cn

PHP ............ 252
来源：http://rq.bookmarksfly.cn

JavaScript ..... 252
来源：http://lx.9csxet.cn

TypeScript ..... 212
来源：http://km.panjiajie.cn

Java ........... 212
来源：http://yt.asd995.cn

Go ............. 212
来源：http://hu.haigaiapp.cn

Ruby ........... 212
来源：http://zi.szxytkj.cn

C# ............. 212
来源：http://vs.shxzskj.cn

C .............. 30
来源：http://hk.yuntaijiaju.cn

C++ ............ 30
来源：http://em.yuntaijiaju.cn

SQL ............ 90
来源：http://wa.szxytkj.cn

Bash ........... 80
来源：http://ca.hahajie.cn

Kotlin ......... 15
来源：http://vo.hnjuh.cn

Swift .......... 15
来源：http://ob.colortex.cn

Lua ............ 10
来源：http://jh.yuntaijiaju.cn

Perl ........... 10
来源：http://od.jctech888.com.cn

Scala .......... 10
来源：http://hg.shxzukj.cn

------------------------------------
来源：http://ha.huanxung.cn

合计 ........... 2106 条
来源：http://se.shtwfgs.cn

按章节统计：
来源：http://yi.jianghongdianzi.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://my.wgjwhj.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://fs.jianghongdianzi.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wn.jianghongdianzi.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://fq.huanxung.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://iv.szsharing.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ve.shtwfgs.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ld.szsharing.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://tp.nszjky.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://lu.shxzukj.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://gd.bjjhwx.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://sv.jianghongdianzi.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://so.bookmarksfly.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://dp.9csxet.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://gv.bookmarksfly.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://be.nszjky.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://bx.newstarts.cn

Q SQL 专题                              90
来源：http://sq.lnxyls.cn

R Bash 专题                             80
来源：http://xw.muxihuayi.cn

S C / C++ 专题                          60
来源：http://yj.muxihuayi.cn

T 其他语言补充                          60
来源：http://be.shxzukj.cn

U 高频实用片段                         120
来源：http://ed.huanxung.cn

------------------------------------
来源：http://js.huixinmuqiang.cn

合计                                  2106 条
来源：http://ee.muxihuayi.cn

--------------------------------------------------------------------------------
来源：http://fz.lnxyls.cn

使用提醒
来源：http://hl.muxihuayi.cn

--------------------------------------------------------------------------------
来源：http://fz.huixinmuqiang.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ar.colortex.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://jm.colortex.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ve.9csxet.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://wg.chemitech.net.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://se.szxytkj.cn

—— 文件结束 ——
来源：http://iy.newstarts.cn

================================================================================
来源：http://ex.szxytkj.cn

程序语言常见例子速查手册（2024 版）
来源：http://iu.9csxet.cn

Common Programming Examples Cheat Book
来源：http://ut.szxytkj.cn

================================================================================
来源：http://sy.yuexingan06.cn

【收录内容】
来源：http://kp.szxytkj.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://pl.hnjuh.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://bg.9csxet.cn

SQL · Bash · C · C++
来源：http://nh.jctech888.com.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ti.szxytkj.cn

【使用说明】
来源：http://zx.jianghongdianzi.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://qa.9csxet.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://nf.chemitech.net.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://nx.haigaiapp.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://rn.huixinmuqiang.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://my.asd995.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://sp.521024.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ar.muxihuayi.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://vz.szsharing.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://gx.wgjwhj.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://qo.newstarts.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://zn.yuexingan06.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://fd.panjiajie.cn

【文件统计】
来源：http://yf.shtwfgs.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://nq.hnjuh.cn

--------------------------------------------------------------------------------
来源：http://jk.shxzukj.cn

目  录
来源：http://ig.shxzukj.cn

--------------------------------------------------------------------------------
来源：http://kv.lnxyls.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ut.jianghongdianzi.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hs.jctech888.com.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://pu.shxzukj.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://am.nszjky.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://zt.wgjwhj.cn


<!-- 参考信息 -->