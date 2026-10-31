代发 wailian999

[U13] Py：固定长度队列
来源：http://xx.521024.cn

deque(maxlen=10)
来源：http://be.yuexingan06.cn

[U14] Py：分组收集到列表
来源：http://dl.huixiangedu.cn

defaultdict(list)
来源：http://lk.bookmarksfly.cn

[U15] Py：高精度计时
来源：http://we.521024.cn

t = time.perf_counter()
来源：http://rk.huixinmuqiang.cn

[U16] Py：命令行参数解析
来源：http://cv.bookmarksfly.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://dx.newstarts.cn

[U17] Py：初始化日志
来源：http://sl.nicolike.cn

logging.basicConfig(level=logging.INFO)
来源：http://ht.jianghongdianzi.cn

[U18] Py：预编译正则
来源：http://de.jctech888.com.cn

pat = re.compile(r"\d+")
来源：http://sn.haigaiapp.cn

[U19] Py：正则替换带回调
来源：http://gr.yuntaijiaju.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://in.shxzskj.cn

[U20] Py：缓存函数结果
来源：http://sh.yuexingan06.cn

@functools.lru_cache(maxsize=None)
来源：http://vm.nszjky.cn

[U21] Py：自定义上下文管理器
来源：http://bl.9csxet.cn

@contextlib.contextmanager
来源：http://lo.nszjky.cn

[U22] Py：矩阵转置
来源：http://wq.bjjhwx.cn

list(zip(*m))
来源：http://tf.colortex.cn

[U23] Py：分块读取大文件
来源：http://ed.muxihuayi.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ag.jianghongdianzi.cn

[U24] Py：路径操作
来源：http://du.shtwfgs.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://qc.shxzukj.cn

[U25] Py：CSV 按字典读
来源：http://ku.huixinmuqiang.cn

csv.DictReader(f)
来源：http://cu.bjjhwx.cn

[U26] Py：并发下载
来源：http://mj.chemitech.net.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ma.chemitech.net.cn

[U27] Py：异步 HTTP
来源：http://wv.bjjhwx.cn

aiohttp.ClientSession() 配合 async with
来源：http://xf.muxihuayi.cn

[U28] Py：类型别名
来源：http://am.hahajie.cn

UserId = int
来源：http://kf.nicolike.cn

[U29] Py：属性校验
来源：http://qi.9csxet.cn

@property 与 @x.setter 配合
来源：http://sg.bookmarksfly.cn

[U30] Py：数据类
来源：http://jq.huixinmuqiang.cn

@dataclass(slots=True)
来源：http://cr.colortex.cn

[U31] Py：单测
来源：http://ww.colortex.cn

python -m pytest -q
来源：http://bd.muxihuayi.cn

[U32] Py：代码格式化
来源：http://tz.bookmarksfly.cn

ruff format . && ruff check --fix .
来源：http://ad.muxihuayi.cn

[U33] Py：打包发布
来源：http://qt.gzmigu.cn

python -m build  （依赖 pyproject.toml）
来源：http://ck.hahajie.cn

[U34] Py：判断编码
来源：http://rp.gzmigu.cn

chardet.detect(raw)
来源：http://dh.9csxet.cn

[U35] Py：发送邮件
来源：http://uv.nicolike.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://vu.chemitech.net.cn

[U36] Py：定时任务
来源：http://ar.wgjwhj.cn

schedule.every(10).minutes.do(job)
来源：http://yc.chemitech.net.cn

[U37] Py：读写 Excel
来源：http://qd.shtwfgs.cn

pandas.read_excel / DataFrame.to_excel
来源：http://qe.haigaiapp.cn

[U38] Py：获取脚本所在目录
来源：http://bu.szsharing.cn

Path(__file__).resolve().parent
来源：http://wq.yuntaijiaju.cn

[U39] Py：判断是否在交互环境
来源：http://hb.chemitech.net.cn

sys.stdout.isatty()
来源：http://le.chemitech.net.cn

[U40] Py：打印到标准错误
来源：http://qj.hnjuh.cn

print("err", file=sys.stderr)
来源：http://tp.haigaiapp.cn

[U41] PHP：初始化 Composer 项目
来源：http://gy.huixinmuqiang.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://oi.wgjwhj.cn

[U42] PHP：PSR-4 自动加载
来源：http://gg.nicolike.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://pj.huixiangedu.cn

[U43] PHP：声明命名空间
来源：http://na.shxzukj.cn

namespace App\Http;
来源：http://ux.shtwfgs.cn

[U44] PHP：开启严格类型
来源：http://pe.nicolike.cn

declare(strict_types=1);
来源：http://dm.lnxyls.cn

[U45] PHP：类型声明与返回类型
来源：http://yh.hnjuh.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://iq.hnjuh.cn

[U46] PHP：可空类型
来源：http://mr.nszjky.cn

?string $name = null
来源：http://ki.szsharing.cn

[U47] PHP：联合类型
来源：http://ph.nszjky.cn

int|string $id
来源：http://ls.nszjky.cn

[U48] PHP：纯枚举
来源：http://vr.huixinmuqiang.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://aq.huanxung.cn

[U49] PHP：只读属性
来源：http://ip.yuexingan06.cn

public readonly string $name
来源：http://vw.panjiajie.cn

[U50] PHP：构造器属性提升
来源：http://ee.panjiajie.cn

public function __construct(private int $id) {}
来源：http://ph.jctech888.com.cn

[U51] PHP：数组解构
来源：http://sd.bookmarksfly.cn

[$a, $b] = $arr;
来源：http://jt.huixinmuqiang.cn

[U52] PHP：箭头函数
来源：http://uo.jctech888.com.cn

$double = fn($x) => $x * 2;
来源：http://es.haigaiapp.cn

[U53] PHP：空合并运算符
来源：http://xi.haigaiapp.cn

$v = $a ?? $b ?? "default";
来源：http://uw.bookmarksfly.cn

[U54] PHP：空安全调用
来源：http://fi.hnjuh.cn

$obj?->method()
来源：http://vm.huixiangedu.cn

[U55] PHP：match 表达式
来源：http://fd.lnxyls.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://xp.hahajie.cn

[U56] PHP：命名参数
来源：http://rf.hahajie.cn

f(a: 1, b: 2)
来源：http://er.wgjwhj.cn

[U57] PHP：字符串插值
来源：http://ag.yuntaijiaju.cn

"值: {$a}"
来源：http://rv.521024.cn

[U58] PHP：数组三件套
来源：http://cu.szsharing.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://nr.jctech888.com.cn

[U59] PHP：自定义排序
来源：http://mg.newstarts.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ya.bookmarksfly.cn

[U60] PHP：JSON 编解码
来源：http://dn.nicolike.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://iq.hahajie.cn

[U61] PHP：正则
来源：http://lo.szsharing.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://nj.yuntaijiaju.cn

[U62] PHP：日期对象
来源：http://qw.panjiajie.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://qm.shxzskj.cn

[U63] PHP：文件读写
来源：http://xv.bookmarksfly.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://vg.shxzskj.cn

[U64] PHP：目录遍历
来源：http://sk.muxihuayi.cn

glob("dir/*.php");  scandir("dir");
来源：http://qm.shxzukj.cn

[U65] PHP：会话
来源：http://yh.muxihuayi.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://mn.nszjky.cn

[U66] PHP：设置 Cookie
来源：http://lr.shxzukj.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://xv.newstarts.cn

[U67] PHP：处理文件上传
来源：http://tw.chemitech.net.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://jp.nszjky.cn

[U68] PHP：PDO 连接
来源：http://fj.chemitech.net.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://xn.shxzukj.cn

[U69] PHP：PDO 预处理
来源：http://rq.newstarts.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ox.newstarts.cn

[U70] PHP：PDO 事务
来源：http://xl.521024.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://dm.lnxyls.cn

[U71] PHP：抛出异常
来源：http://gd.huixiangedu.cn

throw new RuntimeException("失败", 500);
来源：http://jj.newstarts.cn

[U72] PHP：写错误日志
来源：http://yd.huixiangedu.cn

error_log("失败: " . $e->getMessage());
来源：http://bm.hnjuh.cn

[U73] PHP：读取 ini 配置
来源：http://iw.huanxung.cn

parse_ini_file("config.ini", true)
来源：http://vd.newstarts.cn

[U74] PHP：读取环境变量
来源：http://ix.521024.cn

getenv("APP_ENV") ?: "production"
来源：http://la.huixinmuqiang.cn

[U75] PHP：依赖注入
来源：http://uc.lnxyls.cn

composer require psr/container
来源：http://em.hnjuh.cn

[U76] PHP：简单路由
来源：http://om.wgjwhj.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wt.szsharing.cn

[U77] PHP：模板渲染
来源：http://zz.9csxet.cn

composer require twig/twig
来源：http://wh.szxytkj.cn

[U78] PHP：单元测试
来源：http://hs.wgjwhj.cn

composer require --dev phpunit/phpunit
来源：http://zu.hahajie.cn

[U79] PHP：静态分析
来源：http://wq.bjjhwx.cn

composer require --dev phpstan/phpstan
来源：http://yg.asd995.cn

[U80] PHP：代码规范修复
来源：http://uv.chemitech.net.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://ni.yuntaijiaju.cn

[U81] JS：初始化项目
来源：http://uc.yuntaijiaju.cn

npm init -y;  npm i express
来源：http://ww.huanxung.cn

[U82] JS：package.json 脚本
来源：http://al.panjiajie.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://tu.shxzskj.cn

[U83] JS：ES Module 导入导出
来源：http://gf.colortex.cn

export const a = 1;  import { a } from "./m.js";
来源：http://sl.nicolike.cn

[U84] JS：CommonJS 写法
来源：http://lt.shxzukj.cn

module.exports = { a };  const { a } = require("./m");
来源：http://pg.shxzukj.cn

[U85] JS：可选链
来源：http://hv.huixiangedu.cn

a?.b?.c
来源：http://js.muxihuayi.cn

[U86] JS：空值合并
来源：http://kw.huixinmuqiang.cn

a ?? b
来源：http://wt.bjjhwx.cn

[U87] JS：解构默认值
来源：http://am.hnjuh.cn

const { a = 1, b = 2 } = obj;
来源：http://be.9csxet.cn

[U88] JS：对象展开合并
来源：http://hn.asd995.cn

{ ...a, ...b }
来源：http://ac.nszjky.cn

[U89] JS：数组去重
来源：http://dx.colortex.cn

[...new Set(arr)]
来源：http://nu.gzmigu.cn

[U90] JS：数字数组排序
来源：http://fd.yuexingan06.cn

[...arr].sort((a, b) => a - b)
来源：http://bq.bookmarksfly.cn

[U91] JS：对象键值遍历
来源：http://zp.asd995.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://jk.yuntaijiaju.cn

[U92] JS：深拷贝
来源：http://vd.newstarts.cn

structuredClone(obj)
来源：http://dd.huixinmuqiang.cn

[U93] JS：模板字符串
来源：http://zi.bookmarksfly.cn

`共 ${n} 条`
来源：http://ai.newstarts.cn

[U94] JS：箭头函数
来源：http://pi.hnjuh.cn

const double = x => x * 2;
来源：http://ym.chemitech.net.cn

[U95] JS：Promise 包装
来源：http://gj.huanxung.cn

new Promise((resolve, reject) => {})
来源：http://cb.huixinmuqiang.cn

[U96] JS：async/await 与异常
来源：http://kv.szxytkj.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://nr.huixiangedu.cn

[U97] JS：并发请求
来源：http://xu.521024.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://ql.gzmigu.cn

[U98] JS：fetch 带 JSON
来源：http://ac.huanxung.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://nw.haigaiapp.cn

[U99] JS：事件监听
来源：http://ah.haigaiapp.cn

el.addEventListener("click", e => {})
来源：http://za.muxihuayi.cn

[U100] JS：DOM 查询
来源：http://yz.hahajie.cn

document.querySelector(".item")
来源：http://za.shtwfgs.cn

[U101] JS：classList 操作
来源：http://en.shxzukj.cn

el.classList.toggle("active")
来源：http://yl.hnjuh.cn

[U102] JS：本地存储
来源：http://vc.newstarts.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://xf.wgjwhj.cn

[U103] JS：定时器
来源：http://rr.haigaiapp.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://et.yuexingan06.cn

[U104] JS：防抖
来源：http://yd.jctech888.com.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://na.521024.cn

[U105] JS：节流
来源：http://aq.hahajie.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://my.szsharing.cn

[U106] JS：日期格式化
来源：http://wt.jianghongdianzi.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://gg.asd995.cn

[U107] JS：数字千分位
来源：http://ti.hnjuh.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://zt.bjjhwx.cn

[U108] JS：随机整数
来源：http://vt.shtwfgs.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://pn.jctech888.com.cn

[U109] JS：数组分组
来源：http://ei.9csxet.cn

Object.groupBy(arr, x => x.type)
来源：http://na.lnxyls.cn

[U110] JS：数组分块
来源：http://qk.chemitech.net.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ht.nicolike.cn

[U111] JS：对象转 Map
来源：http://ix.hnjuh.cn

new Map(Object.entries(obj))
来源：http://vx.yuntaijiaju.cn

[U112] JS：字符串补位
来源：http://kh.jianghongdianzi.cn

"7".padStart(3, "0")
来源：http://xr.colortex.cn

[U113] JS：正则替换全部
来源：http://du.bookmarksfly.cn

s.replaceAll("a", "b")
来源：http://yq.huanxung.cn

[U114] JS：JSON 深比较
来源：http://xl.szxytkj.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://zj.chemitech.net.cn

[U115] JS：生成 UUID
来源：http://jz.newstarts.cn

crypto.randomUUID()
来源：http://hc.bookmarksfly.cn

[U116] JS：类型检查（JSDoc）
来源：http://ik.huanxung.cn

/** @param {string} name */ function f(name) {}
来源：http://uz.muxihuayi.cn

[U117] JS：单元测试
来源：http://oi.asd995.cn

npm i -D vitest;  npx vitest
来源：http://lg.jctech888.com.cn

[U118] JS：开发服务器
来源：http://uh.panjiajie.cn

npm i -D vite;  npx vite
来源：http://nf.nicolike.cn

[U119] JS：生产构建
来源：http://qf.bjjhwx.cn

npx vite build
来源：http://au.gzmigu.cn

[U120] JS：读取环境变量（Vite）
来源：http://dt.jctech888.com.cn

import.meta.env.VITE_API_URL
来源：http://wm.hnjuh.cn

================================================================================
来源：http://jp.jianghongdianzi.cn

统计汇总
来源：http://sc.muxihuayi.cn

================================================================================
来源：http://ea.nszjky.cn

按语言统计（条）：
来源：http://uz.521024.cn

Python ......... 252
来源：http://ou.9csxet.cn

PHP ............ 252
来源：http://ob.gzmigu.cn

JavaScript ..... 252
来源：http://wc.521024.cn

TypeScript ..... 212
来源：http://om.bookmarksfly.cn

Java ........... 212
来源：http://pn.jianghongdianzi.cn

Go ............. 212
来源：http://zn.bookmarksfly.cn

Ruby ........... 212
来源：http://vf.asd995.cn

C# ............. 212
来源：http://tb.bjjhwx.cn

C .............. 30
来源：http://ef.muxihuayi.cn

C++ ............ 30
来源：http://xu.shxzukj.cn

SQL ............ 90
来源：http://wa.muxihuayi.cn

Bash ........... 80
来源：http://fh.nicolike.cn

Kotlin ......... 15
来源：http://pi.yuntaijiaju.cn

Swift .......... 15
来源：http://cl.lnxyls.cn

Lua ............ 10
来源：http://ho.hnjuh.cn

Perl ........... 10
来源：http://ab.colortex.cn

Scala .......... 10
来源：http://ff.wgjwhj.cn

------------------------------------
来源：http://bb.muxihuayi.cn

合计 ........... 2106 条
来源：http://qt.newstarts.cn

按章节统计：
来源：http://tg.nicolike.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://gk.yuntaijiaju.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://bx.yuntaijiaju.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ew.huixinmuqiang.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wn.huixinmuqiang.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://pb.chemitech.net.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://uf.huixinmuqiang.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ej.jctech888.com.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://fa.hnjuh.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hc.haigaiapp.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://pm.bjjhwx.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://xd.yuntaijiaju.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://vb.newstarts.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://zx.lnxyls.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://dh.szxytkj.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://gl.muxihuayi.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://jo.bookmarksfly.cn

Q SQL 专题                              90
来源：http://uq.szxytkj.cn

R Bash 专题                             80
来源：http://jx.chemitech.net.cn

S C / C++ 专题                          60
来源：http://yp.yuexingan06.cn

T 其他语言补充                          60
来源：http://ur.jianghongdianzi.cn

U 高频实用片段                         120
来源：http://cx.colortex.cn

------------------------------------
来源：http://yk.newstarts.cn

合计                                  2106 条
来源：http://hh.bjjhwx.cn

--------------------------------------------------------------------------------
来源：http://tu.shxzukj.cn

使用提醒
来源：http://zt.haigaiapp.cn

--------------------------------------------------------------------------------
来源：http://fe.jianghongdianzi.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://fa.muxihuayi.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ob.shxzskj.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://vv.gzmigu.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://gg.colortex.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://qg.521024.cn

—— 文件结束 ——
来源：http://pd.chemitech.net.cn

================================================================================
来源：http://fb.nszjky.cn

程序语言常见例子速查手册（2024 版）
来源：http://wi.wgjwhj.cn

Common Programming Examples Cheat Book
来源：http://hq.hnjuh.cn

================================================================================
来源：http://cp.nszjky.cn

【收录内容】
来源：http://nq.szxytkj.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://xm.gzmigu.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ib.shxzukj.cn

SQL · Bash · C · C++
来源：http://tz.bjjhwx.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://fi.bjjhwx.cn

【使用说明】
来源：http://rv.szsharing.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://te.gzmigu.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ut.lnxyls.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://tj.haigaiapp.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://nv.huanxung.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://qy.asd995.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hy.bjjhwx.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://fy.nicolike.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://en.asd995.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://zl.panjiajie.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://jx.asd995.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://vn.muxihuayi.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://bc.huixiangedu.cn

【文件统计】
来源：http://if.shtwfgs.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://bu.huanxung.cn

--------------------------------------------------------------------------------
来源：http://yg.nszjky.cn

目  录
来源：http://po.wgjwhj.cn

--------------------------------------------------------------------------------
来源：http://yh.shxzukj.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://lj.gzmigu.cn


<!-- 参考信息 -->