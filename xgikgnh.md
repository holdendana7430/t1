代发 wailian999

[U15] Py：高精度计时
来源：http://jc.huanxung.cn

t = time.perf_counter()
来源：http://pn.asd995.cn

[U16] Py：命令行参数解析
来源：http://fd.9csxet.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://lz.bookmarksfly.cn

[U17] Py：初始化日志
来源：http://wa.521024.cn

logging.basicConfig(level=logging.INFO)
来源：http://cg.lnxyls.cn

[U18] Py：预编译正则
来源：http://yf.yuntaijiaju.cn

pat = re.compile(r"\d+")
来源：http://hk.jianghongdianzi.cn

[U19] Py：正则替换带回调
来源：http://bf.shtwfgs.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://nt.bookmarksfly.cn

[U20] Py：缓存函数结果
来源：http://zn.shxzukj.cn

@functools.lru_cache(maxsize=None)
来源：http://wz.hahajie.cn

[U21] Py：自定义上下文管理器
来源：http://xl.nszjky.cn

@contextlib.contextmanager
来源：http://yu.chemitech.net.cn

[U22] Py：矩阵转置
来源：http://ew.newstarts.cn

list(zip(*m))
来源：http://am.huixiangedu.cn

[U23] Py：分块读取大文件
来源：http://js.shtwfgs.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://jo.colortex.cn

[U24] Py：路径操作
来源：http://tc.nszjky.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://gi.shxzukj.cn

[U25] Py：CSV 按字典读
来源：http://uc.9csxet.cn

csv.DictReader(f)
来源：http://qt.szxytkj.cn

[U26] Py：并发下载
来源：http://do.nicolike.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://aw.shxzukj.cn

[U27] Py：异步 HTTP
来源：http://wm.szxytkj.cn

aiohttp.ClientSession() 配合 async with
来源：http://rz.wgjwhj.cn

[U28] Py：类型别名
来源：http://fl.lnxyls.cn

UserId = int
来源：http://eg.lnxyls.cn

[U29] Py：属性校验
来源：http://xi.9csxet.cn

@property 与 @x.setter 配合
来源：http://td.shxzukj.cn

[U30] Py：数据类
来源：http://ja.wgjwhj.cn

@dataclass(slots=True)
来源：http://jr.9csxet.cn

[U31] Py：单测
来源：http://lj.bjjhwx.cn

python -m pytest -q
来源：http://fw.yuntaijiaju.cn

[U32] Py：代码格式化
来源：http://xg.gzmigu.cn

ruff format . && ruff check --fix .
来源：http://gp.9csxet.cn

[U33] Py：打包发布
来源：http://hi.huanxung.cn

python -m build  （依赖 pyproject.toml）
来源：http://jx.yuntaijiaju.cn

[U34] Py：判断编码
来源：http://qp.bjjhwx.cn

chardet.detect(raw)
来源：http://mj.hnjuh.cn

[U35] Py：发送邮件
来源：http://qw.bjjhwx.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://tg.jctech888.com.cn

[U36] Py：定时任务
来源：http://ul.bjjhwx.cn

schedule.every(10).minutes.do(job)
来源：http://yc.shxzukj.cn

[U37] Py：读写 Excel
来源：http://dx.szsharing.cn

pandas.read_excel / DataFrame.to_excel
来源：http://my.szxytkj.cn

[U38] Py：获取脚本所在目录
来源：http://mc.szsharing.cn

Path(__file__).resolve().parent
来源：http://vj.bjjhwx.cn

[U39] Py：判断是否在交互环境
来源：http://on.hahajie.cn

sys.stdout.isatty()
来源：http://wb.colortex.cn

[U40] Py：打印到标准错误
来源：http://de.bookmarksfly.cn

print("err", file=sys.stderr)
来源：http://wv.szsharing.cn

[U41] PHP：初始化 Composer 项目
来源：http://jb.chemitech.net.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://iw.yuexingan06.cn

[U42] PHP：PSR-4 自动加载
来源：http://pm.wgjwhj.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://tm.yuexingan06.cn

[U43] PHP：声明命名空间
来源：http://fn.huixinmuqiang.cn

namespace App\Http;
来源：http://sk.shxzskj.cn

[U44] PHP：开启严格类型
来源：http://op.gzmigu.cn

declare(strict_types=1);
来源：http://wi.shxzskj.cn

[U45] PHP：类型声明与返回类型
来源：http://oa.huixinmuqiang.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://zk.colortex.cn

[U46] PHP：可空类型
来源：http://gy.asd995.cn

?string $name = null
来源：http://qu.hnjuh.cn

[U47] PHP：联合类型
来源：http://qd.hnjuh.cn

int|string $id
来源：http://pt.nicolike.cn

[U48] PHP：纯枚举
来源：http://kn.chemitech.net.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ca.jctech888.com.cn

[U49] PHP：只读属性
来源：http://nj.bjjhwx.cn

public readonly string $name
来源：http://jy.huixiangedu.cn

[U50] PHP：构造器属性提升
来源：http://em.nszjky.cn

public function __construct(private int $id) {}
来源：http://lm.hahajie.cn

[U51] PHP：数组解构
来源：http://xy.szsharing.cn

[$a, $b] = $arr;
来源：http://cq.lnxyls.cn

[U52] PHP：箭头函数
来源：http://kk.nszjky.cn

$double = fn($x) => $x * 2;
来源：http://qc.shtwfgs.cn

[U53] PHP：空合并运算符
来源：http://xg.huanxung.cn

$v = $a ?? $b ?? "default";
来源：http://so.shxzukj.cn

[U54] PHP：空安全调用
来源：http://ea.colortex.cn

$obj?->method()
来源：http://et.newstarts.cn

[U55] PHP：match 表达式
来源：http://wo.shtwfgs.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wo.jctech888.com.cn

[U56] PHP：命名参数
来源：http://cr.yuexingan06.cn

f(a: 1, b: 2)
来源：http://zu.jianghongdianzi.cn

[U57] PHP：字符串插值
来源：http://cy.nszjky.cn

"值: {$a}"
来源：http://as.szsharing.cn

[U58] PHP：数组三件套
来源：http://qo.jctech888.com.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hd.szxytkj.cn

[U59] PHP：自定义排序
来源：http://di.shxzukj.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://pn.yuexingan06.cn

[U60] PHP：JSON 编解码
来源：http://tm.jctech888.com.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://la.bjjhwx.cn

[U61] PHP：正则
来源：http://rb.colortex.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mz.colortex.cn

[U62] PHP：日期对象
来源：http://zj.colortex.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://yc.newstarts.cn

[U63] PHP：文件读写
来源：http://bc.shtwfgs.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://oi.gzmigu.cn

[U64] PHP：目录遍历
来源：http://bf.nszjky.cn

glob("dir/*.php");  scandir("dir");
来源：http://ix.yuexingan06.cn

[U65] PHP：会话
来源：http://gt.yuntaijiaju.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://rj.panjiajie.cn

[U66] PHP：设置 Cookie
来源：http://gw.gzmigu.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://xd.bookmarksfly.cn

[U67] PHP：处理文件上传
来源：http://sd.gzmigu.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://zf.gzmigu.cn

[U68] PHP：PDO 连接
来源：http://oy.lnxyls.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://rs.wgjwhj.cn

[U69] PHP：PDO 预处理
来源：http://hi.shxzskj.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://cv.shxzukj.cn

[U70] PHP：PDO 事务
来源：http://nw.nicolike.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ls.jianghongdianzi.cn

[U71] PHP：抛出异常
来源：http://fp.nszjky.cn

throw new RuntimeException("失败", 500);
来源：http://fv.shxzukj.cn

[U72] PHP：写错误日志
来源：http://kf.huixiangedu.cn

error_log("失败: " . $e->getMessage());
来源：http://eh.gzmigu.cn

[U73] PHP：读取 ini 配置
来源：http://ey.bjjhwx.cn

parse_ini_file("config.ini", true)
来源：http://ko.yuntaijiaju.cn

[U74] PHP：读取环境变量
来源：http://kx.haigaiapp.cn

getenv("APP_ENV") ?: "production"
来源：http://rh.colortex.cn

[U75] PHP：依赖注入
来源：http://xc.asd995.cn

composer require psr/container
来源：http://zn.haigaiapp.cn

[U76] PHP：简单路由
来源：http://wi.huixiangedu.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://km.521024.cn

[U77] PHP：模板渲染
来源：http://jk.asd995.cn

composer require twig/twig
来源：http://fd.nszjky.cn

[U78] PHP：单元测试
来源：http://oy.newstarts.cn

composer require --dev phpunit/phpunit
来源：http://pz.shxzskj.cn

[U79] PHP：静态分析
来源：http://bd.haigaiapp.cn

composer require --dev phpstan/phpstan
来源：http://le.chemitech.net.cn

[U80] PHP：代码规范修复
来源：http://nu.lnxyls.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://ug.521024.cn

[U81] JS：初始化项目
来源：http://ly.nicolike.cn

npm init -y;  npm i express
来源：http://dk.huanxung.cn

[U82] JS：package.json 脚本
来源：http://ha.shxzskj.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://yl.bjjhwx.cn

[U83] JS：ES Module 导入导出
来源：http://xn.jianghongdianzi.cn

export const a = 1;  import { a } from "./m.js";
来源：http://cj.szsharing.cn

[U84] JS：CommonJS 写法
来源：http://aj.hahajie.cn

module.exports = { a };  const { a } = require("./m");
来源：http://vu.chemitech.net.cn

[U85] JS：可选链
来源：http://wl.nszjky.cn

a?.b?.c
来源：http://xp.muxihuayi.cn

[U86] JS：空值合并
来源：http://tg.bjjhwx.cn

a ?? b
来源：http://hz.haigaiapp.cn

[U87] JS：解构默认值
来源：http://su.bookmarksfly.cn

const { a = 1, b = 2 } = obj;
来源：http://yc.yuntaijiaju.cn

[U88] JS：对象展开合并
来源：http://tf.jianghongdianzi.cn

{ ...a, ...b }
来源：http://wx.colortex.cn

[U89] JS：数组去重
来源：http://pl.9csxet.cn

[...new Set(arr)]
来源：http://ic.szsharing.cn

[U90] JS：数字数组排序
来源：http://nv.wgjwhj.cn

[...arr].sort((a, b) => a - b)
来源：http://lx.huixinmuqiang.cn

[U91] JS：对象键值遍历
来源：http://bv.yuntaijiaju.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://nd.9csxet.cn

[U92] JS：深拷贝
来源：http://zi.huixinmuqiang.cn

structuredClone(obj)
来源：http://cq.newstarts.cn

[U93] JS：模板字符串
来源：http://iu.jianghongdianzi.cn

`共 ${n} 条`
来源：http://vy.szxytkj.cn

[U94] JS：箭头函数
来源：http://ga.colortex.cn

const double = x => x * 2;
来源：http://ps.asd995.cn

[U95] JS：Promise 包装
来源：http://xe.9csxet.cn

new Promise((resolve, reject) => {})
来源：http://ae.9csxet.cn

[U96] JS：async/await 与异常
来源：http://gb.jctech888.com.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://qh.hahajie.cn

[U97] JS：并发请求
来源：http://mj.chemitech.net.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://zc.jctech888.com.cn

[U98] JS：fetch 带 JSON
来源：http://ce.huixiangedu.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://rr.521024.cn

[U99] JS：事件监听
来源：http://ek.panjiajie.cn

el.addEventListener("click", e => {})
来源：http://ac.jctech888.com.cn

[U100] JS：DOM 查询
来源：http://xu.hnjuh.cn

document.querySelector(".item")
来源：http://mp.hnjuh.cn

[U101] JS：classList 操作
来源：http://dp.shxzskj.cn

el.classList.toggle("active")
来源：http://ql.yuntaijiaju.cn

[U102] JS：本地存储
来源：http://tq.huixinmuqiang.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://vt.jianghongdianzi.cn

[U103] JS：定时器
来源：http://cs.hahajie.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://rd.huanxung.cn

[U104] JS：防抖
来源：http://uu.lnxyls.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nm.jianghongdianzi.cn

[U105] JS：节流
来源：http://dk.muxihuayi.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://be.shxzukj.cn

[U106] JS：日期格式化
来源：http://wc.yuexingan06.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ek.chemitech.net.cn

[U107] JS：数字千分位
来源：http://sl.9csxet.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ee.huixiangedu.cn

[U108] JS：随机整数
来源：http://yf.asd995.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://zk.gzmigu.cn

[U109] JS：数组分组
来源：http://hh.muxihuayi.cn

Object.groupBy(arr, x => x.type)
来源：http://ai.lnxyls.cn

[U110] JS：数组分块
来源：http://ve.colortex.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://vf.lnxyls.cn

[U111] JS：对象转 Map
来源：http://to.huanxung.cn

new Map(Object.entries(obj))
来源：http://dr.hnjuh.cn

[U112] JS：字符串补位
来源：http://xl.hahajie.cn

"7".padStart(3, "0")
来源：http://eh.huixiangedu.cn

[U113] JS：正则替换全部
来源：http://yf.shxzukj.cn

s.replaceAll("a", "b")
来源：http://ex.panjiajie.cn

[U114] JS：JSON 深比较
来源：http://sh.colortex.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://rh.gzmigu.cn

[U115] JS：生成 UUID
来源：http://oo.jianghongdianzi.cn

crypto.randomUUID()
来源：http://ow.huixiangedu.cn

[U116] JS：类型检查（JSDoc）
来源：http://zu.shxzskj.cn

/** @param {string} name */ function f(name) {}
来源：http://px.jianghongdianzi.cn

[U117] JS：单元测试
来源：http://wt.bjjhwx.cn

npm i -D vitest;  npx vitest
来源：http://zq.9csxet.cn

[U118] JS：开发服务器
来源：http://ek.shxzukj.cn

npm i -D vite;  npx vite
来源：http://ei.9csxet.cn

[U119] JS：生产构建
来源：http://fb.szsharing.cn

npx vite build
来源：http://cq.shxzukj.cn

[U120] JS：读取环境变量（Vite）
来源：http://jy.hnjuh.cn

import.meta.env.VITE_API_URL
来源：http://wz.szxytkj.cn

================================================================================
来源：http://zm.jctech888.com.cn

统计汇总
来源：http://zv.chemitech.net.cn

================================================================================
来源：http://ju.shxzukj.cn

按语言统计（条）：
来源：http://bm.huixinmuqiang.cn

Python ......... 252
来源：http://zh.bjjhwx.cn

PHP ............ 252
来源：http://zp.wgjwhj.cn

JavaScript ..... 252
来源：http://mg.bookmarksfly.cn

TypeScript ..... 212
来源：http://ld.asd995.cn

Java ........... 212
来源：http://xp.shxzskj.cn

Go ............. 212
来源：http://dk.yuexingan06.cn

Ruby ........... 212
来源：http://ls.nicolike.cn

C# ............. 212
来源：http://vp.nszjky.cn

C .............. 30
来源：http://rl.huixinmuqiang.cn

C++ ............ 30
来源：http://vo.huixiangedu.cn

SQL ............ 90
来源：http://sr.bjjhwx.cn

Bash ........... 80
来源：http://td.hahajie.cn

Kotlin ......... 15
来源：http://xv.hnjuh.cn

Swift .......... 15
来源：http://cz.nszjky.cn

Lua ............ 10
来源：http://ey.newstarts.cn

Perl ........... 10
来源：http://jr.szsharing.cn

Scala .......... 10
来源：http://uj.jianghongdianzi.cn

------------------------------------
来源：http://ya.gzmigu.cn

合计 ........... 2106 条
来源：http://ob.nicolike.cn

按章节统计：
来源：http://fy.huixiangedu.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://uf.hnjuh.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://re.nicolike.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ig.asd995.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://pl.jctech888.com.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://bn.szsharing.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://qf.bookmarksfly.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://yz.jctech888.com.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ox.521024.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hj.shxzskj.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://rq.huixinmuqiang.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://qy.szsharing.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://we.jctech888.com.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://nn.colortex.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://qe.shxzskj.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://dr.nicolike.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://zx.yuntaijiaju.cn

Q SQL 专题                              90
来源：http://ej.shxzukj.cn

R Bash 专题                             80
来源：http://jh.yuntaijiaju.cn

S C / C++ 专题                          60
来源：http://qv.szsharing.cn

T 其他语言补充                          60
来源：http://pk.asd995.cn

U 高频实用片段                         120
来源：http://kc.9csxet.cn

------------------------------------
来源：http://pu.nicolike.cn

合计                                  2106 条
来源：http://kw.panjiajie.cn

--------------------------------------------------------------------------------
来源：http://rm.hnjuh.cn

使用提醒
来源：http://aw.shxzukj.cn

--------------------------------------------------------------------------------
来源：http://gv.gzmigu.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ab.panjiajie.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://zy.yuexingan06.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://aa.newstarts.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://cn.panjiajie.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://jp.bookmarksfly.cn

—— 文件结束 ——
来源：http://ko.huixinmuqiang.cn

================================================================================
来源：http://pn.haigaiapp.cn

程序语言常见例子速查手册（2024 版）
来源：http://sd.shxzskj.cn

Common Programming Examples Cheat Book
来源：http://cl.bjjhwx.cn

================================================================================
来源：http://gz.gzmigu.cn

【收录内容】
来源：http://jw.yuntaijiaju.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://yo.jctech888.com.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://og.jctech888.com.cn

SQL · Bash · C · C++
来源：http://ez.huanxung.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ad.nszjky.cn

【使用说明】
来源：http://hh.yuexingan06.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://sp.panjiajie.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://kb.bookmarksfly.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://kg.yuexingan06.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://pr.bjjhwx.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://zk.chemitech.net.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://cz.szsharing.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://jn.wgjwhj.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://nc.shtwfgs.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://wt.muxihuayi.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://fh.nicolike.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://qf.muxihuayi.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://zx.huanxung.cn

【文件统计】
来源：http://nd.colortex.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://sx.jianghongdianzi.cn

--------------------------------------------------------------------------------
来源：http://jj.jianghongdianzi.cn

目  录
来源：http://nq.9csxet.cn

--------------------------------------------------------------------------------
来源：http://pv.chemitech.net.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ry.hahajie.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://tk.muxihuayi.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://gx.asd995.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://kx.szxytkj.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://yl.wgjwhj.cn


<!-- 参考信息 -->