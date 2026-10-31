代发 wailian999

[U13] Py：固定长度队列
来源：http://cb.nszjky.cn

deque(maxlen=10)
来源：http://nb.jctech888.com.cn

[U14] Py：分组收集到列表
来源：http://pa.nszjky.cn

defaultdict(list)
来源：http://fm.huanxung.cn

[U15] Py：高精度计时
来源：http://jk.shxzukj.cn

t = time.perf_counter()
来源：http://it.muxihuayi.cn

[U16] Py：命令行参数解析
来源：http://fi.nicolike.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://um.9csxet.cn

[U17] Py：初始化日志
来源：http://ul.chemitech.net.cn

logging.basicConfig(level=logging.INFO)
来源：http://pq.szsharing.cn

[U18] Py：预编译正则
来源：http://nq.haigaiapp.cn

pat = re.compile(r"\d+")
来源：http://xw.panjiajie.cn

[U19] Py：正则替换带回调
来源：http://xa.gzmigu.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://nw.bookmarksfly.cn

[U20] Py：缓存函数结果
来源：http://kj.newstarts.cn

@functools.lru_cache(maxsize=None)
来源：http://rl.haigaiapp.cn

[U21] Py：自定义上下文管理器
来源：http://lx.nszjky.cn

@contextlib.contextmanager
来源：http://mp.lnxyls.cn

[U22] Py：矩阵转置
来源：http://oy.gzmigu.cn

list(zip(*m))
来源：http://jk.nicolike.cn

[U23] Py：分块读取大文件
来源：http://in.yuntaijiaju.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://jb.huanxung.cn

[U24] Py：路径操作
来源：http://is.newstarts.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://fu.huanxung.cn

[U25] Py：CSV 按字典读
来源：http://iq.huixinmuqiang.cn

csv.DictReader(f)
来源：http://ad.lnxyls.cn

[U26] Py：并发下载
来源：http://bh.nszjky.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://vz.bjjhwx.cn

[U27] Py：异步 HTTP
来源：http://br.521024.cn

aiohttp.ClientSession() 配合 async with
来源：http://fn.gzmigu.cn

[U28] Py：类型别名
来源：http://tz.bookmarksfly.cn

UserId = int
来源：http://vc.wgjwhj.cn

[U29] Py：属性校验
来源：http://cz.muxihuayi.cn

@property 与 @x.setter 配合
来源：http://rl.jctech888.com.cn

[U30] Py：数据类
来源：http://pk.wgjwhj.cn

@dataclass(slots=True)
来源：http://dh.hnjuh.cn

[U31] Py：单测
来源：http://nu.panjiajie.cn

python -m pytest -q
来源：http://cm.panjiajie.cn

[U32] Py：代码格式化
来源：http://vm.jianghongdianzi.cn

ruff format . && ruff check --fix .
来源：http://qu.hnjuh.cn

[U33] Py：打包发布
来源：http://ty.asd995.cn

python -m build  （依赖 pyproject.toml）
来源：http://ce.nszjky.cn

[U34] Py：判断编码
来源：http://zj.huixinmuqiang.cn

chardet.detect(raw)
来源：http://zr.9csxet.cn

[U35] Py：发送邮件
来源：http://oc.wgjwhj.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ve.chemitech.net.cn

[U36] Py：定时任务
来源：http://fv.jianghongdianzi.cn

schedule.every(10).minutes.do(job)
来源：http://fb.nicolike.cn

[U37] Py：读写 Excel
来源：http://fo.gzmigu.cn

pandas.read_excel / DataFrame.to_excel
来源：http://wr.shtwfgs.cn

[U38] Py：获取脚本所在目录
来源：http://nf.panjiajie.cn

Path(__file__).resolve().parent
来源：http://qe.shxzukj.cn

[U39] Py：判断是否在交互环境
来源：http://vr.haigaiapp.cn

sys.stdout.isatty()
来源：http://id.jianghongdianzi.cn

[U40] Py：打印到标准错误
来源：http://qw.gzmigu.cn

print("err", file=sys.stderr)
来源：http://el.szsharing.cn

[U41] PHP：初始化 Composer 项目
来源：http://fi.shxzukj.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://di.bookmarksfly.cn

[U42] PHP：PSR-4 自动加载
来源：http://ws.huixinmuqiang.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://tf.colortex.cn

[U43] PHP：声明命名空间
来源：http://ms.521024.cn

namespace App\Http;
来源：http://aw.shxzskj.cn

[U44] PHP：开启严格类型
来源：http://zl.bookmarksfly.cn

declare(strict_types=1);
来源：http://er.shxzukj.cn

[U45] PHP：类型声明与返回类型
来源：http://gu.huanxung.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://is.huixiangedu.cn

[U46] PHP：可空类型
来源：http://pt.muxihuayi.cn

?string $name = null
来源：http://fr.panjiajie.cn

[U47] PHP：联合类型
来源：http://py.gzmigu.cn

int|string $id
来源：http://bl.szxytkj.cn

[U48] PHP：纯枚举
来源：http://my.huanxung.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://di.yuntaijiaju.cn

[U49] PHP：只读属性
来源：http://zo.wgjwhj.cn

public readonly string $name
来源：http://mp.jianghongdianzi.cn

[U50] PHP：构造器属性提升
来源：http://st.yuntaijiaju.cn

public function __construct(private int $id) {}
来源：http://pd.lnxyls.cn

[U51] PHP：数组解构
来源：http://se.9csxet.cn

[$a, $b] = $arr;
来源：http://aq.huixinmuqiang.cn

[U52] PHP：箭头函数
来源：http://do.yuntaijiaju.cn

$double = fn($x) => $x * 2;
来源：http://fi.szsharing.cn

[U53] PHP：空合并运算符
来源：http://ox.colortex.cn

$v = $a ?? $b ?? "default";
来源：http://kq.shtwfgs.cn

[U54] PHP：空安全调用
来源：http://yt.shxzukj.cn

$obj?->method()
来源：http://yf.bjjhwx.cn

[U55] PHP：match 表达式
来源：http://sz.szsharing.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://di.9csxet.cn

[U56] PHP：命名参数
来源：http://kb.huanxung.cn

f(a: 1, b: 2)
来源：http://xt.hnjuh.cn

[U57] PHP：字符串插值
来源：http://em.jianghongdianzi.cn

"值: {$a}"
来源：http://wo.muxihuayi.cn

[U58] PHP：数组三件套
来源：http://ss.muxihuayi.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://uq.huixiangedu.cn

[U59] PHP：自定义排序
来源：http://uk.huanxung.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://dr.szsharing.cn

[U60] PHP：JSON 编解码
来源：http://qz.bjjhwx.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://sf.bjjhwx.cn

[U61] PHP：正则
来源：http://cn.bookmarksfly.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://uh.shtwfgs.cn

[U62] PHP：日期对象
来源：http://sb.gzmigu.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://sa.chemitech.net.cn

[U63] PHP：文件读写
来源：http://rj.wgjwhj.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ma.hnjuh.cn

[U64] PHP：目录遍历
来源：http://io.newstarts.cn

glob("dir/*.php");  scandir("dir");
来源：http://qh.bookmarksfly.cn

[U65] PHP：会话
来源：http://tv.521024.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://nr.muxihuayi.cn

[U66] PHP：设置 Cookie
来源：http://kp.nszjky.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ow.newstarts.cn

[U67] PHP：处理文件上传
来源：http://yu.colortex.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ba.nszjky.cn

[U68] PHP：PDO 连接
来源：http://xj.jianghongdianzi.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://fw.muxihuayi.cn

[U69] PHP：PDO 预处理
来源：http://un.huixiangedu.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://vl.hnjuh.cn

[U70] PHP：PDO 事务
来源：http://nu.521024.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://sl.huixinmuqiang.cn

[U71] PHP：抛出异常
来源：http://iq.szsharing.cn

throw new RuntimeException("失败", 500);
来源：http://fb.muxihuayi.cn

[U72] PHP：写错误日志
来源：http://tq.huixinmuqiang.cn

error_log("失败: " . $e->getMessage());
来源：http://ce.shxzskj.cn

[U73] PHP：读取 ini 配置
来源：http://uy.nicolike.cn

parse_ini_file("config.ini", true)
来源：http://lf.szsharing.cn

[U74] PHP：读取环境变量
来源：http://fv.muxihuayi.cn

getenv("APP_ENV") ?: "production"
来源：http://mb.shtwfgs.cn

[U75] PHP：依赖注入
来源：http://wl.chemitech.net.cn

composer require psr/container
来源：http://dm.shtwfgs.cn

[U76] PHP：简单路由
来源：http://li.yuexingan06.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://oi.shxzukj.cn

[U77] PHP：模板渲染
来源：http://wy.yuntaijiaju.cn

composer require twig/twig
来源：http://kv.muxihuayi.cn

[U78] PHP：单元测试
来源：http://jg.szxytkj.cn

composer require --dev phpunit/phpunit
来源：http://er.huixiangedu.cn

[U79] PHP：静态分析
来源：http://ou.newstarts.cn

composer require --dev phpstan/phpstan
来源：http://oq.wgjwhj.cn

[U80] PHP：代码规范修复
来源：http://ae.hnjuh.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://vr.bjjhwx.cn

[U81] JS：初始化项目
来源：http://ek.haigaiapp.cn

npm init -y;  npm i express
来源：http://li.panjiajie.cn

[U82] JS：package.json 脚本
来源：http://em.hahajie.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://br.newstarts.cn

[U83] JS：ES Module 导入导出
来源：http://vx.szsharing.cn

export const a = 1;  import { a } from "./m.js";
来源：http://tg.hahajie.cn

[U84] JS：CommonJS 写法
来源：http://xo.9csxet.cn

module.exports = { a };  const { a } = require("./m");
来源：http://lu.nicolike.cn

[U85] JS：可选链
来源：http://qe.panjiajie.cn

a?.b?.c
来源：http://xf.haigaiapp.cn

[U86] JS：空值合并
来源：http://fi.muxihuayi.cn

a ?? b
来源：http://ia.521024.cn

[U87] JS：解构默认值
来源：http://sw.521024.cn

const { a = 1, b = 2 } = obj;
来源：http://ea.jianghongdianzi.cn

[U88] JS：对象展开合并
来源：http://cq.wgjwhj.cn

{ ...a, ...b }
来源：http://um.chemitech.net.cn

[U89] JS：数组去重
来源：http://yh.nicolike.cn

[...new Set(arr)]
来源：http://du.szsharing.cn

[U90] JS：数字数组排序
来源：http://mj.nicolike.cn

[...arr].sort((a, b) => a - b)
来源：http://xk.shxzukj.cn

[U91] JS：对象键值遍历
来源：http://rh.wgjwhj.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ec.colortex.cn

[U92] JS：深拷贝
来源：http://bh.asd995.cn

structuredClone(obj)
来源：http://et.gzmigu.cn

[U93] JS：模板字符串
来源：http://st.hnjuh.cn

`共 ${n} 条`
来源：http://hx.haigaiapp.cn

[U94] JS：箭头函数
来源：http://px.yuexingan06.cn

const double = x => x * 2;
来源：http://kd.shtwfgs.cn

[U95] JS：Promise 包装
来源：http://cc.huixiangedu.cn

new Promise((resolve, reject) => {})
来源：http://fv.521024.cn

[U96] JS：async/await 与异常
来源：http://bt.szsharing.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ol.newstarts.cn

[U97] JS：并发请求
来源：http://eh.panjiajie.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://oy.gzmigu.cn

[U98] JS：fetch 带 JSON
来源：http://ap.shxzskj.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://sx.shxzskj.cn

[U99] JS：事件监听
来源：http://zg.nszjky.cn

el.addEventListener("click", e => {})
来源：http://lg.huixiangedu.cn

[U100] JS：DOM 查询
来源：http://bp.bookmarksfly.cn

document.querySelector(".item")
来源：http://vs.chemitech.net.cn

[U101] JS：classList 操作
来源：http://yv.lnxyls.cn

el.classList.toggle("active")
来源：http://kz.wgjwhj.cn

[U102] JS：本地存储
来源：http://qy.muxihuayi.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://fg.hnjuh.cn

[U103] JS：定时器
来源：http://za.huixiangedu.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://go.chemitech.net.cn

[U104] JS：防抖
来源：http://as.huixinmuqiang.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jx.panjiajie.cn

[U105] JS：节流
来源：http://rv.shtwfgs.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://im.haigaiapp.cn

[U106] JS：日期格式化
来源：http://zx.chemitech.net.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://td.gzmigu.cn

[U107] JS：数字千分位
来源：http://zy.huixiangedu.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ji.jctech888.com.cn

[U108] JS：随机整数
来源：http://ip.newstarts.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://pj.bookmarksfly.cn

[U109] JS：数组分组
来源：http://vq.shxzskj.cn

Object.groupBy(arr, x => x.type)
来源：http://jt.colortex.cn

[U110] JS：数组分块
来源：http://es.yuexingan06.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://im.szsharing.cn

[U111] JS：对象转 Map
来源：http://gn.hnjuh.cn

new Map(Object.entries(obj))
来源：http://qs.huixinmuqiang.cn

[U112] JS：字符串补位
来源：http://za.shxzskj.cn

"7".padStart(3, "0")
来源：http://yl.jctech888.com.cn

[U113] JS：正则替换全部
来源：http://su.newstarts.cn

s.replaceAll("a", "b")
来源：http://kc.haigaiapp.cn

[U114] JS：JSON 深比较
来源：http://rv.yuntaijiaju.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://jk.huanxung.cn

[U115] JS：生成 UUID
来源：http://sx.yuexingan06.cn

crypto.randomUUID()
来源：http://lw.521024.cn

[U116] JS：类型检查（JSDoc）
来源：http://mw.hahajie.cn

/** @param {string} name */ function f(name) {}
来源：http://mz.jctech888.com.cn

[U117] JS：单元测试
来源：http://po.hahajie.cn

npm i -D vitest;  npx vitest
来源：http://xh.hahajie.cn

[U118] JS：开发服务器
来源：http://zv.jianghongdianzi.cn

npm i -D vite;  npx vite
来源：http://fk.newstarts.cn

[U119] JS：生产构建
来源：http://pf.newstarts.cn

npx vite build
来源：http://tp.nszjky.cn

[U120] JS：读取环境变量（Vite）
来源：http://wk.huixinmuqiang.cn

import.meta.env.VITE_API_URL
来源：http://nk.muxihuayi.cn

================================================================================
来源：http://vh.colortex.cn

统计汇总
来源：http://dj.huixinmuqiang.cn

================================================================================
来源：http://wi.shxzskj.cn

按语言统计（条）：
来源：http://bt.jianghongdianzi.cn

Python ......... 252
来源：http://yd.jianghongdianzi.cn

PHP ............ 252
来源：http://pp.gzmigu.cn

JavaScript ..... 252
来源：http://by.huixiangedu.cn

TypeScript ..... 212
来源：http://jv.gzmigu.cn

Java ........... 212
来源：http://bs.huixiangedu.cn

Go ............. 212
来源：http://yq.bjjhwx.cn

Ruby ........... 212
来源：http://xs.nicolike.cn

C# ............. 212
来源：http://gl.huixiangedu.cn

C .............. 30
来源：http://yw.szxytkj.cn

C++ ............ 30
来源：http://yk.newstarts.cn

SQL ............ 90
来源：http://lh.jctech888.com.cn

Bash ........... 80
来源：http://ih.huixiangedu.cn

Kotlin ......... 15
来源：http://mw.shtwfgs.cn

Swift .......... 15
来源：http://ho.jianghongdianzi.cn

Lua ............ 10
来源：http://so.muxihuayi.cn

Perl ........... 10
来源：http://tm.shtwfgs.cn

Scala .......... 10
来源：http://ll.nicolike.cn

------------------------------------
来源：http://zl.bjjhwx.cn

合计 ........... 2106 条
来源：http://eq.newstarts.cn

按章节统计：
来源：http://nf.szsharing.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://xn.shxzskj.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://iw.huixiangedu.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ir.shxzukj.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://rm.521024.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wa.newstarts.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hj.521024.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wd.shxzukj.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://pe.bjjhwx.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://lq.yuntaijiaju.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ob.huixinmuqiang.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://rr.panjiajie.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://kp.szxytkj.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://os.nszjky.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ks.nszjky.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hx.newstarts.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://rf.haigaiapp.cn

Q SQL 专题                              90
来源：http://wn.bookmarksfly.cn

R Bash 专题                             80
来源：http://yl.huanxung.cn

S C / C++ 专题                          60
来源：http://me.9csxet.cn

T 其他语言补充                          60
来源：http://by.shxzskj.cn

U 高频实用片段                         120
来源：http://sd.panjiajie.cn

------------------------------------
来源：http://hs.haigaiapp.cn

合计                                  2106 条
来源：http://nr.shxzukj.cn

--------------------------------------------------------------------------------
来源：http://lz.jianghongdianzi.cn

使用提醒
来源：http://rh.9csxet.cn

--------------------------------------------------------------------------------
来源：http://bd.huixiangedu.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://mi.shxzskj.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://tj.shxzukj.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://pu.bookmarksfly.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://rc.muxihuayi.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://vp.521024.cn

—— 文件结束 ——
来源：http://qh.szxytkj.cn

================================================================================
来源：http://qn.gzmigu.cn

程序语言常见例子速查手册（2024 版）
来源：http://bo.jctech888.com.cn

Common Programming Examples Cheat Book
来源：http://ii.chemitech.net.cn

================================================================================
来源：http://ex.nicolike.cn

【收录内容】
来源：http://de.gzmigu.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://et.muxihuayi.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://fu.chemitech.net.cn

SQL · Bash · C · C++
来源：http://zc.hahajie.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://yo.chemitech.net.cn

【使用说明】
来源：http://ld.jctech888.com.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://yn.newstarts.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://qu.newstarts.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://la.521024.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://io.bjjhwx.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://be.shxzskj.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://lj.9csxet.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ww.muxihuayi.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://gf.hnjuh.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://xt.huixinmuqiang.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ft.bookmarksfly.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://nt.szsharing.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://dv.szsharing.cn

【文件统计】
来源：http://jq.hnjuh.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://xg.hnjuh.cn

--------------------------------------------------------------------------------
来源：http://xl.yuexingan06.cn

目  录
来源：http://tl.shtwfgs.cn

--------------------------------------------------------------------------------
来源：http://ns.521024.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://qk.jctech888.com.cn


<!-- 参考信息 -->