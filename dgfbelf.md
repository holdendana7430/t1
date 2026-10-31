代发 wailian999

[U07] Py：反转字典键值
来源：http://ha.muxihuayi.cn

{v: k for k, v in d.items()}
来源：http://bl.huixiangedu.cn

[U08] Py：展平二维列表
来源：http://gh.haigaiapp.cn

[y for x in nested for y in x]
来源：http://kb.hahajie.cn

[U09] Py：字典取最大值的键
来源：http://kz.yuntaijiaju.cn

max(d, key=d.get)
来源：http://ef.huixinmuqiang.cn

[U10] Py：按值排序字典
来源：http://rl.shxzskj.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://be.szsharing.cn

[U11] Py：生成器表达式
来源：http://lh.shxzskj.cn

(x * 2 for x in arr)
来源：http://mo.lnxyls.cn

[U12] Py：取出现最多的 3 个元素
来源：http://tg.newstarts.cn

Counter(arr).most_common(3)
来源：http://jy.haigaiapp.cn

[U13] Py：固定长度队列
来源：http://cz.szsharing.cn

deque(maxlen=10)
来源：http://cy.hahajie.cn

[U14] Py：分组收集到列表
来源：http://ij.hahajie.cn

defaultdict(list)
来源：http://vz.shxzukj.cn

[U15] Py：高精度计时
来源：http://xt.bjjhwx.cn

t = time.perf_counter()
来源：http://hs.jctech888.com.cn

[U16] Py：命令行参数解析
来源：http://la.shxzukj.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ep.lnxyls.cn

[U17] Py：初始化日志
来源：http://zo.wgjwhj.cn

logging.basicConfig(level=logging.INFO)
来源：http://yn.bjjhwx.cn

[U18] Py：预编译正则
来源：http://ni.huixiangedu.cn

pat = re.compile(r"\d+")
来源：http://wq.haigaiapp.cn

[U19] Py：正则替换带回调
来源：http://fz.9csxet.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://nq.wgjwhj.cn

[U20] Py：缓存函数结果
来源：http://fn.gzmigu.cn

@functools.lru_cache(maxsize=None)
来源：http://zo.jctech888.com.cn

[U21] Py：自定义上下文管理器
来源：http://dm.bookmarksfly.cn

@contextlib.contextmanager
来源：http://wq.nicolike.cn

[U22] Py：矩阵转置
来源：http://xk.hahajie.cn

list(zip(*m))
来源：http://nv.bookmarksfly.cn

[U23] Py：分块读取大文件
来源：http://xe.huanxung.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://xi.yuexingan06.cn

[U24] Py：路径操作
来源：http://my.muxihuayi.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hj.wgjwhj.cn

[U25] Py：CSV 按字典读
来源：http://fa.yuexingan06.cn

csv.DictReader(f)
来源：http://mt.nicolike.cn

[U26] Py：并发下载
来源：http://vm.szsharing.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://jz.asd995.cn

[U27] Py：异步 HTTP
来源：http://uq.yuntaijiaju.cn

aiohttp.ClientSession() 配合 async with
来源：http://yo.huixiangedu.cn

[U28] Py：类型别名
来源：http://nn.jctech888.com.cn

UserId = int
来源：http://cn.muxihuayi.cn

[U29] Py：属性校验
来源：http://tv.lnxyls.cn

@property 与 @x.setter 配合
来源：http://ak.haigaiapp.cn

[U30] Py：数据类
来源：http://lo.panjiajie.cn

@dataclass(slots=True)
来源：http://tc.huanxung.cn

[U31] Py：单测
来源：http://zf.szxytkj.cn

python -m pytest -q
来源：http://ec.lnxyls.cn

[U32] Py：代码格式化
来源：http://uw.hnjuh.cn

ruff format . && ruff check --fix .
来源：http://no.bjjhwx.cn

[U33] Py：打包发布
来源：http://dd.chemitech.net.cn

python -m build  （依赖 pyproject.toml）
来源：http://cv.nicolike.cn

[U34] Py：判断编码
来源：http://ub.hahajie.cn

chardet.detect(raw)
来源：http://fp.asd995.cn

[U35] Py：发送邮件
来源：http://nf.9csxet.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mx.yuntaijiaju.cn

[U36] Py：定时任务
来源：http://zx.jctech888.com.cn

schedule.every(10).minutes.do(job)
来源：http://ei.chemitech.net.cn

[U37] Py：读写 Excel
来源：http://vb.szxytkj.cn

pandas.read_excel / DataFrame.to_excel
来源：http://dx.szsharing.cn

[U38] Py：获取脚本所在目录
来源：http://nl.yuexingan06.cn

Path(__file__).resolve().parent
来源：http://tv.huixiangedu.cn

[U39] Py：判断是否在交互环境
来源：http://rk.asd995.cn

sys.stdout.isatty()
来源：http://pv.shxzskj.cn

[U40] Py：打印到标准错误
来源：http://ll.wgjwhj.cn

print("err", file=sys.stderr)
来源：http://tk.jianghongdianzi.cn

[U41] PHP：初始化 Composer 项目
来源：http://gm.nszjky.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://qn.szsharing.cn

[U42] PHP：PSR-4 自动加载
来源：http://xb.chemitech.net.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ek.szsharing.cn

[U43] PHP：声明命名空间
来源：http://jc.asd995.cn

namespace App\Http;
来源：http://xe.huixinmuqiang.cn

[U44] PHP：开启严格类型
来源：http://ex.muxihuayi.cn

declare(strict_types=1);
来源：http://cf.521024.cn

[U45] PHP：类型声明与返回类型
来源：http://xb.9csxet.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://ks.hahajie.cn

[U46] PHP：可空类型
来源：http://lo.huanxung.cn

?string $name = null
来源：http://ty.chemitech.net.cn

[U47] PHP：联合类型
来源：http://xe.huixiangedu.cn

int|string $id
来源：http://ze.panjiajie.cn

[U48] PHP：纯枚举
来源：http://fu.nszjky.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://xk.shtwfgs.cn

[U49] PHP：只读属性
来源：http://wd.shxzukj.cn

public readonly string $name
来源：http://mf.gzmigu.cn

[U50] PHP：构造器属性提升
来源：http://bo.wgjwhj.cn

public function __construct(private int $id) {}
来源：http://wc.nszjky.cn

[U51] PHP：数组解构
来源：http://pi.wgjwhj.cn

[$a, $b] = $arr;
来源：http://iz.jianghongdianzi.cn

[U52] PHP：箭头函数
来源：http://dd.muxihuayi.cn

$double = fn($x) => $x * 2;
来源：http://wu.yuntaijiaju.cn

[U53] PHP：空合并运算符
来源：http://jo.9csxet.cn

$v = $a ?? $b ?? "default";
来源：http://hz.huixinmuqiang.cn

[U54] PHP：空安全调用
来源：http://ec.shtwfgs.cn

$obj?->method()
来源：http://qb.yuexingan06.cn

[U55] PHP：match 表达式
来源：http://al.jctech888.com.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://le.nszjky.cn

[U56] PHP：命名参数
来源：http://rq.shxzskj.cn

f(a: 1, b: 2)
来源：http://es.szxytkj.cn

[U57] PHP：字符串插值
来源：http://mh.bookmarksfly.cn

"值: {$a}"
来源：http://gu.nszjky.cn

[U58] PHP：数组三件套
来源：http://wa.chemitech.net.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ht.haigaiapp.cn

[U59] PHP：自定义排序
来源：http://jh.nicolike.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://pf.lnxyls.cn

[U60] PHP：JSON 编解码
来源：http://ss.asd995.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wz.hahajie.cn

[U61] PHP：正则
来源：http://lk.asd995.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://yl.yuexingan06.cn

[U62] PHP：日期对象
来源：http://ht.jianghongdianzi.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://pk.jianghongdianzi.cn

[U63] PHP：文件读写
来源：http://qd.huanxung.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://xw.gzmigu.cn

[U64] PHP：目录遍历
来源：http://mo.bookmarksfly.cn

glob("dir/*.php");  scandir("dir");
来源：http://nx.nszjky.cn

[U65] PHP：会话
来源：http://wk.huixiangedu.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://kp.bookmarksfly.cn

[U66] PHP：设置 Cookie
来源：http://rf.haigaiapp.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://yt.hnjuh.cn

[U67] PHP：处理文件上传
来源：http://ku.szsharing.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://md.lnxyls.cn

[U68] PHP：PDO 连接
来源：http://mp.yuntaijiaju.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ha.bookmarksfly.cn

[U69] PHP：PDO 预处理
来源：http://zp.shxzukj.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://jy.jianghongdianzi.cn

[U70] PHP：PDO 事务
来源：http://db.nszjky.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://vg.9csxet.cn

[U71] PHP：抛出异常
来源：http://qi.nszjky.cn

throw new RuntimeException("失败", 500);
来源：http://ya.colortex.cn

[U72] PHP：写错误日志
来源：http://qa.jianghongdianzi.cn

error_log("失败: " . $e->getMessage());
来源：http://ds.gzmigu.cn

[U73] PHP：读取 ini 配置
来源：http://if.newstarts.cn

parse_ini_file("config.ini", true)
来源：http://lb.yuntaijiaju.cn

[U74] PHP：读取环境变量
来源：http://vw.yuexingan06.cn

getenv("APP_ENV") ?: "production"
来源：http://px.gzmigu.cn

[U75] PHP：依赖注入
来源：http://iu.chemitech.net.cn

composer require psr/container
来源：http://ch.huixinmuqiang.cn

[U76] PHP：简单路由
来源：http://oy.chemitech.net.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ex.hahajie.cn

[U77] PHP：模板渲染
来源：http://xs.shtwfgs.cn

composer require twig/twig
来源：http://as.lnxyls.cn

[U78] PHP：单元测试
来源：http://em.521024.cn

composer require --dev phpunit/phpunit
来源：http://mu.nicolike.cn

[U79] PHP：静态分析
来源：http://gi.chemitech.net.cn

composer require --dev phpstan/phpstan
来源：http://ie.nicolike.cn

[U80] PHP：代码规范修复
来源：http://lm.yuntaijiaju.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://xd.gzmigu.cn

[U81] JS：初始化项目
来源：http://us.haigaiapp.cn

npm init -y;  npm i express
来源：http://tj.hahajie.cn

[U82] JS：package.json 脚本
来源：http://jv.yuntaijiaju.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://vl.huixiangedu.cn

[U83] JS：ES Module 导入导出
来源：http://vp.shtwfgs.cn

export const a = 1;  import { a } from "./m.js";
来源：http://eo.shxzukj.cn

[U84] JS：CommonJS 写法
来源：http://qt.panjiajie.cn

module.exports = { a };  const { a } = require("./m");
来源：http://cc.wgjwhj.cn

[U85] JS：可选链
来源：http://se.huanxung.cn

a?.b?.c
来源：http://md.nicolike.cn

[U86] JS：空值合并
来源：http://wx.bjjhwx.cn

a ?? b
来源：http://fb.wgjwhj.cn

[U87] JS：解构默认值
来源：http://er.huanxung.cn

const { a = 1, b = 2 } = obj;
来源：http://gm.521024.cn

[U88] JS：对象展开合并
来源：http://vx.panjiajie.cn

{ ...a, ...b }
来源：http://mf.muxihuayi.cn

[U89] JS：数组去重
来源：http://oa.nszjky.cn

[...new Set(arr)]
来源：http://kd.hnjuh.cn

[U90] JS：数字数组排序
来源：http://ug.szsharing.cn

[...arr].sort((a, b) => a - b)
来源：http://rr.newstarts.cn

[U91] JS：对象键值遍历
来源：http://qx.newstarts.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://kd.asd995.cn

[U92] JS：深拷贝
来源：http://la.nicolike.cn

structuredClone(obj)
来源：http://he.haigaiapp.cn

[U93] JS：模板字符串
来源：http://wl.asd995.cn

`共 ${n} 条`
来源：http://wy.shxzukj.cn

[U94] JS：箭头函数
来源：http://hu.szsharing.cn

const double = x => x * 2;
来源：http://wo.haigaiapp.cn

[U95] JS：Promise 包装
来源：http://zt.yuexingan06.cn

new Promise((resolve, reject) => {})
来源：http://fp.muxihuayi.cn

[U96] JS：async/await 与异常
来源：http://eu.szsharing.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ho.haigaiapp.cn

[U97] JS：并发请求
来源：http://tm.hahajie.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://ow.yuexingan06.cn

[U98] JS：fetch 带 JSON
来源：http://sw.hnjuh.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ar.colortex.cn

[U99] JS：事件监听
来源：http://ln.chemitech.net.cn

el.addEventListener("click", e => {})
来源：http://ke.colortex.cn

[U100] JS：DOM 查询
来源：http://ri.huixinmuqiang.cn

document.querySelector(".item")
来源：http://gi.521024.cn

[U101] JS：classList 操作
来源：http://sf.szxytkj.cn

el.classList.toggle("active")
来源：http://tz.szsharing.cn

[U102] JS：本地存储
来源：http://gk.jianghongdianzi.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://fk.jctech888.com.cn

[U103] JS：定时器
来源：http://jn.huanxung.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://pd.bookmarksfly.cn

[U104] JS：防抖
来源：http://io.bookmarksfly.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rm.lnxyls.cn

[U105] JS：节流
来源：http://bo.colortex.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ha.jianghongdianzi.cn

[U106] JS：日期格式化
来源：http://oa.nszjky.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://jf.haigaiapp.cn

[U107] JS：数字千分位
来源：http://il.hahajie.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ts.shxzukj.cn

[U108] JS：随机整数
来源：http://je.shxzskj.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://tn.yuexingan06.cn

[U109] JS：数组分组
来源：http://jw.jctech888.com.cn

Object.groupBy(arr, x => x.type)
来源：http://fe.shtwfgs.cn

[U110] JS：数组分块
来源：http://gd.newstarts.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hp.asd995.cn

[U111] JS：对象转 Map
来源：http://kq.colortex.cn

new Map(Object.entries(obj))
来源：http://sd.yuntaijiaju.cn

[U112] JS：字符串补位
来源：http://bm.newstarts.cn

"7".padStart(3, "0")
来源：http://lp.colortex.cn

[U113] JS：正则替换全部
来源：http://gh.lnxyls.cn

s.replaceAll("a", "b")
来源：http://mb.jianghongdianzi.cn

[U114] JS：JSON 深比较
来源：http://gy.chemitech.net.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://pr.hahajie.cn

[U115] JS：生成 UUID
来源：http://ms.bjjhwx.cn

crypto.randomUUID()
来源：http://tv.asd995.cn

[U116] JS：类型检查（JSDoc）
来源：http://wd.colortex.cn

/** @param {string} name */ function f(name) {}
来源：http://hn.shtwfgs.cn

[U117] JS：单元测试
来源：http://km.9csxet.cn

npm i -D vitest;  npx vitest
来源：http://eh.jianghongdianzi.cn

[U118] JS：开发服务器
来源：http://lf.szsharing.cn

npm i -D vite;  npx vite
来源：http://qg.panjiajie.cn

[U119] JS：生产构建
来源：http://vb.lnxyls.cn

npx vite build
来源：http://ag.lnxyls.cn

[U120] JS：读取环境变量（Vite）
来源：http://jr.huanxung.cn

import.meta.env.VITE_API_URL
来源：http://za.colortex.cn

================================================================================
来源：http://yr.chemitech.net.cn

统计汇总
来源：http://vw.szsharing.cn

================================================================================
来源：http://ys.shtwfgs.cn

按语言统计（条）：
来源：http://ph.huixinmuqiang.cn

Python ......... 252
来源：http://lx.huixinmuqiang.cn

PHP ............ 252
来源：http://nt.huanxung.cn

JavaScript ..... 252
来源：http://fi.yuntaijiaju.cn

TypeScript ..... 212
来源：http://ln.szsharing.cn

Java ........... 212
来源：http://nd.huixinmuqiang.cn

Go ............. 212
来源：http://qf.yuexingan06.cn

Ruby ........... 212
来源：http://wg.521024.cn

C# ............. 212
来源：http://kf.bjjhwx.cn

C .............. 30
来源：http://ls.panjiajie.cn

C++ ............ 30
来源：http://yi.hnjuh.cn

SQL ............ 90
来源：http://ct.9csxet.cn

Bash ........... 80
来源：http://yn.yuntaijiaju.cn

Kotlin ......... 15
来源：http://up.yuntaijiaju.cn

Swift .......... 15
来源：http://sh.bjjhwx.cn

Lua ............ 10
来源：http://oj.colortex.cn

Perl ........... 10
来源：http://ix.shtwfgs.cn

Scala .......... 10
来源：http://cn.nszjky.cn

------------------------------------
来源：http://wd.gzmigu.cn

合计 ........... 2106 条
来源：http://em.shxzskj.cn

按章节统计：
来源：http://aa.bookmarksfly.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://bi.huixinmuqiang.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://db.jianghongdianzi.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ey.521024.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://bf.colortex.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ks.muxihuayi.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://pl.panjiajie.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://fx.newstarts.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mo.shxzukj.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://eh.newstarts.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mg.shxzskj.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://lp.shtwfgs.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://td.shxzukj.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://zm.9csxet.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hi.shxzukj.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://bo.nicolike.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://vx.shxzukj.cn

Q SQL 专题                              90
来源：http://by.muxihuayi.cn

R Bash 专题                             80
来源：http://zy.jctech888.com.cn

S C / C++ 专题                          60
来源：http://dr.bjjhwx.cn

T 其他语言补充                          60
来源：http://he.wgjwhj.cn

U 高频实用片段                         120
来源：http://tp.shxzukj.cn

------------------------------------
来源：http://hz.hahajie.cn

合计                                  2106 条
来源：http://ly.yuexingan06.cn

--------------------------------------------------------------------------------
来源：http://oy.colortex.cn

使用提醒
来源：http://ut.yuexingan06.cn

--------------------------------------------------------------------------------
来源：http://np.colortex.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://jo.panjiajie.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://nf.shtwfgs.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://xn.521024.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://po.chemitech.net.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://tk.haigaiapp.cn

—— 文件结束 ——
来源：http://vj.huanxung.cn

================================================================================
来源：http://lg.muxihuayi.cn

程序语言常见例子速查手册（2024 版）
来源：http://xk.nicolike.cn

Common Programming Examples Cheat Book
来源：http://qc.lnxyls.cn

================================================================================
来源：http://yx.jctech888.com.cn

【收录内容】
来源：http://an.gzmigu.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://bu.muxihuayi.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://jx.asd995.cn

SQL · Bash · C · C++
来源：http://gv.hnjuh.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://os.haigaiapp.cn

【使用说明】
来源：http://qa.nicolike.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://do.szxytkj.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://bo.wgjwhj.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hp.asd995.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://rs.huanxung.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://pu.lnxyls.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://du.haigaiapp.cn


<!-- 参考信息 -->